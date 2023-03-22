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
      <div>
        <h2> A Digital Product Agency</h2>
        <div>
          Leading digital agency with solid design and development expertise. We build readymade websites, mobile applications, and elaborate online business services.
        </div>
        <button>
          Contact Now
        </button>
      </div>
      <div>
        <img src="./assets/images/people/briefing2.jpg"
        alt="briefing"
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
