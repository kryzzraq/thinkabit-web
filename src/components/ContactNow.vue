<template>
  <div class="contact_now__shapes--container">
    <div class="contact_now--container">
      <div class="contact_now--box1">
        <h1 class="contact_now--box1--title">Subscribe Newsletter</h1>
        <div class="contact_now--box1--info">
          I will update good news and promotion service not spam
        </div>
      </div>
      <div class="contact_now--box2">
        <input
          type="email"
          placeholder="Enter your email address.."
          class="contact_now--box2--input"
          :value="modelValue"
          @input="$emit('update:modelValue', $event.target.value)"
        />
        <button class="contact_now--box2--button" @click="sendRequest()">
          Contact Now
        </button>
      </div>
      <div class="contact_now--container--blue-shape"></div>
    </div>
    <img
      class="contact_now__shapes--container--blue-dots"
      src="../assets/images/ornaments/blue-dots-small.png"
    />
    <div class="contact_now__shapes--container--orange-shape"></div>

    <div class="modal" v-if="showModal">
      <div class="modal-dialog">
        <div class="modal-content">
          <div class="modal-body">
            <p>El email se ha enviado correctamente</p>
          </div>
          <div class="modal-footer">
            <button type="button" @click="closeModal()">Close</button>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import axios from "axios";
import { ref } from "vue";
export default {
  components: {},
  props: {
    modelValue: {
      type: String,
      default: "",
    },
  },
  emits: ["update:modelValue", "updateEmailInput"],

  setup(props) {
    const showModal = ref(false);
    const sendRequest = () => {
        // eslint-disable-next-line
      const regex = /^\w+([\.-]?\w+)*@\w+([\.-]?\w+)*(\.\w{2,3})+$/;
      if (props.modelValue != "" && props.modelValue.match(regex)) {
        axios
          .post(
            "https://1a3bdf42-30a3-4c04-bfd4-f1886cc11ae3.mock.pstmn.io/email/send",
            {
              email: props.modelValue,
            }
          )
          .then((response) => {
            console.log(response);

            if (response.status === 200) {
              console.log("El email se ha enviado correctamente");
              showModal.value = true;

              setTimeout(() => {
                showModal.value = false;
              }, 3000);
            }
          });
      }
    };
    const closeModal = () => {
      showModal.value = false;
    };
    return {
      sendRequest,
      showModal,
      closeModal,
    };
  },
};
</script>

<style lang="scss" scoped>
.modal {
  background: rgb(255, 255, 255);
  position: absolute;
  z-index: 10000;
  left: 50%;
  top: 0;
  transform: translateX(-50%);
  box-shadow: 10px 20px 50px rgba(0, 0, 0, 0.5);
  border-radius: 30px;

  &-dialog {
    padding: 30px 60px 10px 60px;
  }

  &-body {
    font-size: 20px;
  }

  &-footer {
    padding-top: 50px;
    text-align: end;
    button {
      font-size: 16px;
      background-color: #2639ed;
      color: white;
      height: 60px;
      width: 187px;
      border: 0;
      border-radius: 60px;
      cursor: pointer;

      &:hover,
      :focus {
        animation: pulse 1s;
        box-shadow: 0 0 0 1em transparent;
      }

      @keyframes pulse {
        0% {
          box-shadow: 0 0 0 0 #5566fa;
        }
      }
    }
  }
}
.contact_now {
  &--container {
    position: relative;
    background-color: #f4f9ff;
    margin: 120px;
    min-height: 290px;
    border-radius: 75px;

    display: flex;
    align-items: center;
    justify-content: space-between;
    z-index: 1;

    &--blue-shape {
      background-image: url("../assets/images/ornaments/blue-trapezoid.png");
      background-repeat: no-repeat;
      position: absolute;
      z-index: -1;
      width: 500px;
      height: 100%;
      right: 0;
    }
  }

  &__shapes--container {
    position: relative;

    &--blue-dots {
      position: absolute;
      z-index: -1;
      top: -50px;
      right: 80px;
    }

    &--orange-shape {
      position: absolute;
      width: 178px;
      height: 178px;
      background-color: #fff5db;

      bottom: -40px;
      left: 80px;
      border-radius: 0px 0px 0px 100px;
      z-index: -1;
    }
  }

  &--box1 {
    padding-left: 60px;
    &--title {
      font-size: 40px;
    }

    &--info {
      font-size: 16px;
      color: #757575;
      padding: 10px 0;
    }
  }

  &--box2 {
    padding-right: 60px;
    position: relative;

    &--input {
      width: 479px;
      height: 80px;
      background: #ffffff;
      border: 1px solid #f1f1f1;

      font-size: 16px;
      padding: 30px;

      box-shadow: 10px 20px 50px rgba(0, 0, 0, 0.15);
      border-radius: 60px;

      &:focus-visible,
      &:focus,
      &:active {
        outline-color: transparent;
      }
    }

    &--button {
      right: 70px;
      top: 10px;
      color: white;
      font-size: 16px;
      position: absolute;
      background-color: #2639ed;
      height: 60px;
      width: 187px;
      border: 0;
      border-radius: 60px;
      cursor: pointer;

      &:hover,
      :focus {
        animation: pulse 1s;
        box-shadow: 0 0 0 1em transparent;
      }

      @keyframes pulse {
        0% {
          box-shadow: 0 0 0 0 #5566fa;
        }
      }
    }
  }
}
@media (max-width: 1080px) {
  .contact_now--container {
    flex-wrap: wrap;
    justify-content: center;
  }
  .contact_now--box1,
  .contact_now--box2 {
    padding: 0;
  }
  .contact_now--box2--button {
    right: 10px;
  }

  .contact_now--container--blue-shape {
    display: none;
  }
}

@media (max-width: 800px) {
  .contact_now--container {
    margin: 30px;
    padding: 30px;
  }
  .contact_now--box2--input {
    height: 1em;
    width: 100%;
  }
  .contact_now--box2--button {
    position: relative;
    right: 0;
  }
}
</style>
