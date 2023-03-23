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
        <li>Home</li>
        <li>Our client</li>
        <li>About us</li>
        <li>Feedback</li>
        <li>Contact</li>
      </ul>
    </section>
  </header>
  <main>
    <section class="section-home">
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
      </div>
    </section>
    <section class="section-client">Our Client</section>
    <section class="section-about">How can we help your Business ?</section>
    <section class="section-feedback">What our happy client say</section>
    <section class="section-contact">Subscribe Newsletter</section>
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
