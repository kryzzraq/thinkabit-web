<template>
  <header id="main-header">
    <section class="top-nav">
      <img
        src="./assets/images/icons/thinkabit-logo.png"
        alt="thinkabit-logo"
      />
      <input id="menu-toggle" type="checkbox" />
      <label class="menu-button-container" for="menu-toggle">
        <div class="menu-button"></div>
      </label>
      <ul class="menu">
        <li><a href="#section-home">Home</a></li>
        <li><a href="#section-client">Our client</a></li>
        <li><a href="#section-about">About us</a></li>
        <li><a href="#section-feedback">Feedback</a></li>
        <li><a href="#section-contact">Contact</a></li>
      </ul>
    </section>
  </header>
  <main>
    <section class="section-home" id="section-home">
      <div class="section-home__box1">
        <h1 class="section-home__box1--title">A Digital Product Agency</h1>
        <div class="section-home__box1--info">
          Leading digital agency with solid design and development expertise. We
          build readymade websites, mobile applications, and elaborate online
          business services.
        </div>
        <button class="section-home__box1--button">
          <a href="#section-contact">Contact Now</a>
        </button>
        <img
          class="section-home__box1--dots_ornament"
          src="./assets/images/ornaments/grey-dots.png"
        />
        <div class="section-home__box1--blue-circle"></div>
      </div>
      <div class="section-home__box2">
        <img
          src="./assets/images/people/briefing2.jpg"
          alt="briefing"
          class="section-home__box2--img"
        />
        <div class="section-home__box2--orange-shape"></div>
      </div>
    </section>

    <section class="section-client" id="section-client">
      <div class="section-client__box1">
        <h1 class="section-client__box1--title">Our client</h1>
        <div class="section-client__box1--info">
          Several selected clients, who already believe in our service.
        </div>
      </div>
      <div class="section-client__box2">
        <img
          src="./assets/images/icons/google-logo.png"
          alt="google-logo"
          class="section-client__box2--logo section-client__box2--logo--google"
        />
        <img
          src="./assets/images/icons/airbnb-logo.png"
          alt="airbnb-logo"
          class="section-client__box2--logo section-client__box2--logo--airbnb"
        />
        <img
          src="./assets/images/icons/uber-eats-logo.png"
          alt="uber-eats-logo"
          class="section-client__box2--logo section-client__box2--logo--uber"
        />
        <img
          src="./assets/images/icons/amazon-logo.png"
          alt="amazon-logo"
          class="section-client__box2--logo section-client__box2--logo--amazon"
        />
      </div>
    </section>
    <section class="section-about" id="section-about">
      <div class="section-about__box1">
        <h1 class="section-about__box1--title">
          How can we help your Business ?
        </h1>
        <div class="section-about__box1--info">
          We build readymade websites, mobile applications, and elaborate online
          business services.
        </div>
      </div>
      <div class="section-about__box2">
        <div class="section-about__box2--detail section-about__box2--detail-1">
          <div
            class="section-about__box2--detail--shape section-about__box2--detail--shape-1"
          >
            <img src="./assets/images/icons/box-search.svg" alt="" />
          </div>
          <h3 class="section-about__box2--detail--title">
            Business Idea Planning
          </h3>
          <span class="section-about__box2--detail--info"
            >We present you a proposal and discuss niffty-gritty like</span
          >
        </div>
        <div class="section-about__box2--detail section-about__box2--detail-2">
          <div
            class="section-about__box2--detail--shape section-about__box2--detail--shape-2"
          >
            <img src="./assets/images/icons/empty-wallet.svg" alt="" />
          </div>
          <h3 class="section-about__box2--detail--title">
            Financial Planning System
          </h3>
          <span class="section-about__box2--detail--info"
            >Protocols apart from aengage models, pricing billing</span
          >
        </div>
        <div class="section-about__box2--detail section-about__box2--detail-3">
          <div
            class="section-about__box2--detail--shape section-about__box2--detail--shape-3"
          >
            <img src="./assets/images/icons/calendar.svg" alt="" />
          </div>
          <h3 class="section-about__box2--detail--title">
            Development Website and App
          </h3>
          <span class="section-about__box2--detail--info"
            >Communication protocols apart from engagement models</span
          >
        </div>
        <div class="section-about__box2--detail section-about__box2--detail-4">
          <div
            class="section-about__box2--detail--shape section-about__box2--detail--shape-4"
          >
            <img src="./assets/images/icons/chart-square.svg" alt="" />
          </div>
          <h3 class="section-about__box2--detail--title">
            Market Analysis Project
          </h3>
          <span class="section-about__box2--detail--info"
            >Protocols apart from aengage models, pricing billing</span
          >
        </div>
        <div class="section-about__box2--pink_shape"></div>
      </div>
      <div class="section-about--orange_shape"></div>
      <div class="section-about--blue_shape"></div>
      <img
        class="section-about--dots_ornament"
        src="./assets/images/ornaments/blue-dots.png"
      />
    </section>
    <section class="section-feedback" id="section-feedback">
      <div class="section-feedback__box1">
        <video
          id="video"
          width="650"
          height="350"
          muted
          src="https://www.intermarkit.es/recursos/media/portal/2017/04/21/video-home.mp4"
          poster="./assets/images/people/briefing1.jpg"
        ></video>
        <button
          class="section-feedback__box1--button"
          v-if="!is_playing"
          @click="playVideo()"
        >
          <span class="section-feedback__box1--button-play"></span>
        </button>
        <div class="section-feedback__box1--orange_shape"></div>
      </div>
      <div class="section-feedback__box2">
        <h1 class="section-feedback__box2--title">
          Great Digital Product Agency since 2016
        </h1>
        <div class="section-feedback__box2--info">
          Our Business Plan is a written document describing a company's core
          business activites, Objectives, and how it plans to achieve its goals.
          Our goal is to provide our client high quality Product with modern
          idea accordingly their budgets and according thir reuirements..
        </div>
        <div class="section-feedback__box2--blue_shape"></div>
      </div>
    </section>
    <section class="section-people">
      <div class="section-people__box1">
        <div class="section-people__box1--header">
          <h1 class="section-people__box1--header--title">
            What our happy client say
          </h1>
          <div class="section-people__box1--header--info">
            Several selected clients, who already believe in our service.
          </div>
        </div>
        <div class="section-people__box1--content">
          <div class="section-people__box1--content--1">
            <img
              class="section-people__box1--content--1--photo"
              src="./assets/images/people/guy3.jpg"
            />
            <div class="section-people__box1--content--1--pink_shape"></div>
            <img
              class="section-people__box1--content--1--dots_ornaments"
              src="./assets/images/ornaments/grey-dots-small.png"
            />
          </div>
          <div class="section-people__box1--content--2">
            <h4 class="section-people__box1--content--2--title">
              Matthew Paul
            </h4>
            <div class="section-people__box1--content--2--info">
              Perfect, very good job! Thank you for the amazing design and work.
              Really impressed with the high quality and quick turnaround time.
              Highly recommend.
            </div>
          </div>
          <div class="section-people__box1--content--3">
            <img src="./assets/images/people/people.png" />
            <div class="section-people__box1--content--3--orange_shape"></div>
          </div>
        </div>
      </div>
    </section>
    <section class="section-contact" id="section-contact">
      <contact-now v-model="value" />
    </section>
  </main>
  <footer class="footer">
    <div class="footer__main">
      <div class="footer__main__info">
        <img
          src="./assets/images/icons/thinkabit-logo.png"
          alt="thinkabit-logo"
          class="footer__main__info--title"
        />
        <div class="footer__main__info--info">
          Leading digital agency with solid design and development expertise. We
          build readymade websites, mobile applications, and elaborate online
          business services.
        </div>
        <div>
          <img
            src="./assets/images/icons/twitter-logo.png"
            alt="twitter-logo"
            class="footer__main__info--logo footer__main__info--logo--twitter"
          />
          <img
            src="./assets/images/icons/linked-in-logo.png"
            alt="linked-in-logo"
            class="footer__main__info--logo footer__main__info--logo--linkedin"
          />
        </div>
      </div>
      <div class="footer__main__links--container">
        <div class="footer__main__links">
          <h5 class="footer__main__links--title">What We Do</h5>
          <ul class="footer__main__links--list">
            <li>
              <a href="https://www.thinkabit.es/" target="_blank">Web Design</a>
            </li>
            <li>
              <a href="https://www.thinkabit.es/" target="_blank">App Design</a>
            </li>
            <li>
              <a href="https://www.thinkabit.es/" target="_blank"
                >Social Media Manage</a
              >
            </li>
            <li>
              <a href="https://www.thinkabit.es/" target="_blank"
                >Market Analysis Project</a
              >
            </li>
          </ul>
        </div>
        <div class="footer__main__links">
          <h5 class="footer__main__links--title">Company</h5>
          <ul class="footer__main__links--list">
            <li>
              <a href="https://www.thinkabit.es/" target="_blank">About Us</a>
            </li>
            <li>
              <a href="https://www.thinkabit.es/" target="_blank">Career</a>
            </li>
            <li>
              <a href="https://www.thinkabit.es/" target="_blank"
                >Become Investor</a
              >
            </li>
          </ul>
        </div>
        <div class="footer__main__links">
          <h5 class="footer__main__links--title">Support</h5>
          <ul class="footer__main__links--list">
            <li><a href="https://www.thinkabit.es/" target="_blank">FAQ</a></li>
            <li>
              <a href="https://www.thinkabit.es/" target="_blank">Policy</a>
            </li>
            <li>
              <a href="https://www.thinkabit.es/" target="_blank">Business</a>
            </li>
          </ul>
        </div>
        <div class="footer__main__links">
          <h5 class="footer__main__links--title">Contact</h5>
          <ul class="footer__main__links--list">
            <li>
              <a href="https://www.thinkabit.es/" target="_blank">WhatsApp</a>
            </li>
            <li>
              <a href="https://www.thinkabit.es/" target="_blank">Support 24</a>
            </li>
          </ul>
        </div>
      </div>
    </div>
    <div class="footer__copyright">Copyright © 2023 Thinkabit</div>
  </footer>
</template>

<script>
import { ref } from "vue";
import contactNow from "@/components/ContactNow.vue";

export default {
  name: "App",
  components: {
    contactNow,
  },
  setup() {
    const is_playing = ref(false);

    const value = ref("");

    const playVideo = () => {
      const video = document.getElementById("video");
      video.controls = true;
      video.play();
      is_playing.value = true;
    };

    return {
      is_playing,
      playVideo,
      value,
    };
  },
};
</script>

<style lang="scss">
@import "./assets/styles/main.scss";
</style>
