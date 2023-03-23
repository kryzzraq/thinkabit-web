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
        <button class="section-home__box1--button">Contact Now</button>
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
      <div  class="section-about--orange_shape"></div>
      <div class="section-about--blue_shape"></div>
      <img
        class="section-about--dots_ornament"
        src="./assets/images/ornaments/blue-dots.png"
      />
    </section>
    <section class="section-feedback" id="section-feedback">What our happy client say</section>
    <section class="section-contact" id="section-contact">Subscribe Newsletter</section>
  </main>
  <footer>Footer</footer>
</template>

<script>
export default {
  name: "App",
};
</script>

<style lang="scss">
@import "./assets/styles/main.scss";
</style>
