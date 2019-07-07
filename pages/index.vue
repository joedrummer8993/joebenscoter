<template>
  <main class="grid-row grid">
    <section class="grid-row grid intro">
      <div class="intro-backgroundShape"></div>
      <img src="Joe-Cutout2-square.png" class="intro-img" />
      <div class="intro-body" style="padding-bottom: 5rem;">
        <h1 class="intro-heading">
          Hi.
          <span style="color: rgba(97, 132, 153, 1);">I'm Joe.</span>
        </h1>
        <p>I love the challenge of bringing new ideas to life and thrive in the tension of balancing business goals with customer needs.</p>
        <p>I've been the sole designer on a small, tight knit product team for the past 5 years building the future of B2B eCommerce. I've lead our team through a redesign of our company's core product.</p>
        <p>Learn about some of my previous work below.</p>
        <ul class="list-row">
          <!-- <li class="list-row_item"><a href="#about" class="link">About</a></li> -->
          <!-- <li class="list-row_item"><a href="#work" class="link">Work</a></li> -->
          <li class="list-row_item">
            <a href="mailto:joe@benscoter.design" class="link">Contact</a>
          </li>
        </ul>
      </div>
    </section>
    <section class="grid-row grid work">
      <div class="work-backgroundShape work-backgroundShape--alps"></div>
      <div class="work-body" style="padding-bottom: 5rem;">
        <h1 class="work-heading" style="color: #E5690B;">alpscontrols.com</h1>
        <p>From 2016 to present, I've led the redesign and feature development of the customer facing ecommerce platform that eParts licensces to its clients. This was a ground up rewrite and redesign that involved switching to a modern tech stack and design language. I conducted ethnographic interviews in the field in order to create personas that would help us understand user needs and pain points. The new platform has a fresh, re-brandable, mobile responsive interface that is both easier to use and easier on the eyes.</p>
      </div>
      <img src="alpscontros4.PNG" class="work-img" />
    </section>
    <section class="grid-row grid work">
      <div class="work-backgroundShape work-backgroundShape--taiko"></div>
      <div class="work-body" style="padding-bottom: 5rem;">
        <h1 class="work-heading" style="color: #FF3A36;">taikocardgame.com</h1>
        <p>Designed and helped to develop a marketing site to help drive people to back the product on Kickstarter. This involved developing a visual language based on the logo and art in the game.</p>
      </div>
      <img src="taikoHomePage.jpg" class="work-img" />
    </section>
    <section class="grid-row grid work">
      <div class="work-backgroundShape work-backgroundShape--eServices"></div>
      <div class="work-body" style="padding-bottom: 5rem;">
        <h1 class="work-heading" style="color: #935E92;">eServices Technology</h1>
        <p>Designed and developed the front-end of the mobile responsive payment processing and membership management dashboard that powers eServices PaaS. Currently building transaction reporting components using Vue.js.</p>
      </div>
      <img src="eServices-campaigns.png" class="work-img" />
    </section>
    <section class="grid-row grid work">
      <div class="work-backgroundShape work-backgroundShape--bertus"></div>
      <div class="work-body" style="padding-bottom: 5rem;">
        <h1 class="work-heading" style="color: #2A4980;">Bertus Design</h1>
        <p>There are many eye catching gem stones that people don't know much about. This design was all about presenting information about gemstones to people in a way that matched the beauty of the gemstones themselves.</p>
      </div>
      <img src="Bertus-details.png" class="work-img" />
    </section>
  </main>
</template>

<style>
.intro {
  overflow: hidden;
  position: relative;
  min-height: 60vh;
  /* padding-top: 20px; */
}
.intro-backgroundShape {
  grid-column: 1 / 7;
  background-color: rgba(97, 132, 153, 0.1);
  position: absolute;
  top: 5%;
  left: 5%;
  width: 90%;
  height: 60%;
  background-size: cover;
  border-radius: 2px 2px 5rem 2px;
}
.intro-img {
  z-index: 2;
  grid-column: 2 / 3;
  width: 100%;
  background-color: rgba(97, 132, 153, 0.25);
  border-radius: 50%;
  /* padding-top: 2rem; */
  position: relative;
  place-self: center center;
  filter: drop-shadow(8px 4px 15px grey) grayscale(10%);
}
.intro-img:hover {
  filter: drop-shadow(8px 4px 10px grey) grayscale(0%);
  transition: linear 1s;
}
.intro-heading {
  font-size: 4rem;
}
.intro-body {
  z-index: 5;
  grid-column: 4 / 6;
  padding: 5rem 0;
  /* background: white; */
  position: relative;
  top: 0;
  right: 0;
  place-self: start center;
}
.article-heading {
  grid-column: 2 / 6;
  /* border-bottom: 1px solid lightgray; */
}
.work {
  overflow: hidden;
  position: relative;
  min-height: 60vh;
}
.work-backgroundShape {
  grid-column: 5 / 6;
  background-color: rgba(97, 132, 153, 0.1);
  position: absolute;
  top: 5%;
  left: -10%;
  width: 100%;
  height: 60%;
  background-size: cover;
  border-radius: 2px 2px 5rem 2px;
}
.work-heading {
  font-size: 4rem;
}
.work-backgroundShape--alps {
  background-color: #f8b37e;
}
.work-backgroundShape--taiko {
  background-color: rgba(255, 165, 132, 1);
}
.work-backgroundShape--eServices {
  background-color: rgb(182, 141, 182);
}
.work-backgroundShape--bertus {
  background-color: rgb(183, 209, 224);
}
.work-img {
  z-index: 2;
  grid-column: 5 / 6;
  width: 100%;
  max-height: 400px;
  object-fit: cover;
  object-position: 0 0;
  background-color: rgba(97, 132, 153, 0.25);
  border-radius: 5px;
  /* padding-top: 2rem; */
  position: relative;
  place-self: start center;
  margin-top: 5rem;
  filter: drop-shadow(8px 4px 15px grey) grayscale(10%);
}
.work--bertus {
  /* background-color: rgb(183, 209, 224); */
  /* border: solid 16px rgb(183, 209, 224); */
}
.work--taiko {
  /* background-color: rgb(255, 165, 132); */
  /* border: solid 16px rgb(255, 165, 132); */
}
.work--eservices {
  /* background-color: rgb(182, 141, 182); */
  /* border: solid 16px rgb(182, 141, 182); */
}
.work-background {
  content: '';
  position: absolute;
  top: 0;
  right: 0;
  width: 100%;
  height: 100%;
  transform: rotate(12deg);
  background-size: cover;
  background-repeat: no-repeat;
  opacity: 0.3;
  grid-column: 3 / 6;
}
.work-background--left {
  /* transform: rotate(-12deg); */
  right: unset;
  left: 0;
  grid-column: 2 / 5;
}
.work-background--alps {
  background-image: radial-gradient(
      ellipse closest-side,
      /* rgba(248, 179, 126, 0.25),
      rgba(248, 179, 126, 1) */
        rgba(255, 255, 255, 0.25),
      rgba(255, 255, 255, 1)
    ),
    url('/alpscontros4.PNG');
}
.work-background--bertus {
  background-image: radial-gradient(
      ellipse closest-side,
      /* rgba(183, 209, 224, 0.25),
      rgba(183, 209, 224, 1) */
        rgba(255, 255, 255, 0.25),
      rgba(255, 255, 255, 1)
    ),
    url('/Bertus-details.PNG');
}
.work-background--taiko {
  background-image: radial-gradient(
      ellipse closest-side,
      /* rgba(255, 165, 132, 0.25),
      rgba(255, 165, 132, 1) */
        rgba(255, 255, 255, 0.25),
      rgba(255, 255, 255, 1)
    ),
    url('/taikoHomePage.jpg');
}
.work-background--eservices {
  background-image: radial-gradient(
      ellipse closest-side,
      /* rgba(182, 141, 182, 0.25),
      rgba(182, 141, 182, 1) */
        rgba(255, 255, 255, 0.25),
      rgba(255, 255, 255, 1)
    ),
    url('/eServices-campaigns.png');
}
.work-transition {
  height: 0.5rem;
}
.work-transition--none-alps {
  height: 0.5rem;
  background: rgb(248, 179, 126);
}
.work-transition--alps-taiko {
  background: linear-gradient(
    to bottom,
    rgb(248, 179, 126),
    rgb(255, 165, 132)
  );
  background: rgb(255, 165, 132);
}
.work-transition--taiko-eservices {
  background: linear-gradient(
    to bottom,
    rgb(255, 165, 132),
    rgb(182, 141, 182)
  );
  background: rgb(182, 141, 182);
}
.work-transition--eservices-bertus {
  background: linear-gradient(
    to bottom,
    rgb(182, 141, 182),
    rgb(183, 209, 224)
  );
  background: rgb(183, 209, 224);
}
.work-transition--bertus-none {
  background: rgb(183, 209, 224);
}
.work-body {
  grid-column: 2 / 4;
  z-index: 2;
  padding: 5rem 0;
}
.work-body--right {
  grid-column: 3 / 6;
}
.button {
  padding: 0.5rem 1rem;
  background-color: rgb(206, 112, 40);
  color: white;
  border-radius: 0.5rem;
  border-bottom: 3px solid rgb(138, 75, 27);
}
.button:hover {
  color: white;
  border-bottom: 2px solid rgb(138, 75, 27);
}
@media only screen and (max-width: 800px) {
  .alps-body {
    grid-column: 2 / 6;
  }
}
</style>
