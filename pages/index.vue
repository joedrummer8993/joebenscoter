<template>
  <main class="grid-row grid">
    <section class="grid-row intro">
      <div class="intro-backgroundShape"></div>
      <div class="intro-image">
        <img src="JoeB1.png" class="intro-img" />
      </div>
      <header class="intro-header">
        <h1 class="intro-heading">
          <span class="intro-heading-greeting">Hello, I'm</span>
          <span style="color: rgba(97, 132, 153, 1);">Joe Benscoter.</span>
        </h1>
      </header>
      <div class="intro-body">
        <p>I am a product designer and front-end developer who brings ideas to life through human centered design and accessible development.</p>
        <br />
        <p>My work experience ranges from designing a website for learning in-depth information about specific gemstones to designing and developing the front end of a payment processing dashboard to designing and developing the front-end of a b2b ecommerce platform as a service.</p>
        <br />
        <p>You can read more about these experiences below or <a href="/resume.pdf" target="_blank">view my resume</a> for a brief overview.</p>
        <ul class="list-row">
          <!-- <li class="list-row_item"><a href="#about" class="link">About</a></li> -->
          <!-- <li class="list-row_item"><a href="#work" class="link">Work</a></li> -->
          <li class="list-row_item">
            <!-- <a href="mailto:joe@benscoter.design" class="link">Contact</a> -->
          </li>
        </ul>
      </div>
    </section>
    <header id="work" class="grid-row grid">
      <!-- <h1 class="section-title">
        Work
      </h1>-->
    </header>
    <article class="grid-row work">
      <header class="work-header">
        <h1 class="work-heading work-heading--alps">eParts Platform</h1>
        <ul class="list-row skill-nuggets">
          <li class="list-row_item">Art Direction</li>
          <li class="list-row_item">Personas</li>
          <li class="list-row_item">Prototyping</li>
          <li class="list-row_item">HTML</li>
          <li class="list-row_item">CSS</li>
        </ul>
      </header>
      <section class="work-body">
        <p>From 2016 to present, I've led the redesign and feature development of the customer facing ecommerce platform that eParts licensces to its clients. This was a ground up rewrite and redesign that involved switching to a modern tech stack and design language. I conducted ethnographic interviews in the field in order to create personas that would help us understand user needs and pain points. The new platform has a fresh, re-brandable, mobile responsive interface that is both easier to use and easier on the eyes.</p>
      </section>
      <div class="work-image">
        <div class="work-backgroundShape work-backgroundShape--alps"></div>
        <img src="alpscontros4.PNG" class="work-img" />
      </div>
    </article>
    <article class="grid-row work">
      <header class="work-header">
        <h1 class="work-heading work-heading--taiko">taikocardgame.com</h1>
        <ul class="list-row skill-nuggets">
          <li class="list-row_item">Ui/Ux design</li>
          <li class="list-row_item">Development</li>
        </ul>
      </header>
      <section class="work-body">
        <p>Designed and helped to develop a marketing site to help drive people to back the product on Kickstarter. This involved developing a visual language based on the logo and art in the game.</p>
      </section>
      <div class="work-image">
        <div class="work-backgroundShape work-backgroundShape--taiko"></div>
        <img src="taikoHomePage.jpg" class="work-img" />
      </div>
    </article>
    <article class="grid-row work">
      <header class="work-header">
        <h1 class="work-heading work-heading--eServices">eServices Technology</h1>
        <ul class="list-row skill-nuggets">
          <li class="list-row_item">Ui/Ux design</li>
          <li class="list-row_item">Development</li>
        </ul>
      </header>
      <section class="work-body">
        <p>Designed and developed the front-end of the mobile responsive payment processing and membership management dashboard that powers eServices PaaS. Currently building transaction reporting components using Vue.js.</p>
      </section>
      <div class="work-image">
        <div class="work-backgroundShape work-backgroundShape--eServices"></div>
        <img src="eServices-campaigns.png" class="work-img" />
      </div>
    </article>
    <article class="grid-row work">
      <header class="work-header">
        <h1 class="work-heading" style="color: #2A4980;">Bertus Design</h1>
        <ul class="list-row skill-nuggets">
          <li class="list-row_item">Art Direction</li>
          <li class="list-row_item">Mockups</li>
        </ul>
      </header>
      <section class="work-body">
        <p>There are many eye catching gem stones that people don't know much about. This design was all about presenting information about gemstones to people in a way that matched the beauty of the gemstones themselves.</p>
      </section>
      <div class="work-image">
        <div class="work-backgroundShape work-backgroundShape--bertus"></div>
        <img src="Bertus-details.png" class="work-img" />
      </div>
    </article>
  </main>
</template>

<style>
.intro {
  /* min-height: 40vh; */
  /* padding-bottom: 10vh; */
  padding: 2rem 0;
  position: relative;
  margin-bottom: 15vh;
  grid-column: 2 / 6;
  display: grid;
  grid-template-columns: minmax(10rem, 0.5fr) 0.25fr 2.5fr;
  grid-template-rows: auto 1fr;
  grid-template-areas:
    'image . title'
    'image . body';
}
.intro-backgroundShape {
  background-color: rgba(97, 132, 153, 0.1);
  position: absolute;
  top: 0;
  left: -5%;
  width: 110%;
  height: 100%;
  background-size: cover;
  border-radius: 2px 2px 5rem 2px;
}
.intro-image {
  grid-area: image;
  width: 100%;
}
.intro-img {
  z-index: 2;
  width: 100%;
  background-color: rgba(97, 132, 153, 0.25);
  border-radius: 50%;
  position: relative;
  place-self: start center;
  filter: drop-shadow(8px 4px 15px grey);
  transition: ease 1s;
}
.intro-img:hover {
  filter: drop-shadow(8px 4px 10px grey);
}
.intro-header {
  grid-area: title;
}
.intro-heading {
  font-size: 4rem;
  margin-bottom: 1rem;
  display: flex;
  flex-flow: column;
  font-family: 'Mada';
}
.intro-heading-greeting {
  font-size: 1.5rem;
  line-height: 2rem;
}
.intro-body {
  z-index: 5;
  grid-area: body;
  padding: 2rem 0;
  /* font-size: 1.2rem; */
}
.section-title {
  grid-column: 2 / 6;
  /* border-bottom: 1px solid lightgray; */
  /* background: rgb(240, 240, 240); */
}
.work {
  position: relative;
  margin-bottom: 20vh;
  grid-column: 2 / 6;
  display: grid;
  grid-template-columns: 2fr 1fr;
  grid-template-rows: auto 1fr;
  grid-template-areas:
    'title image'
    'body image';
  grid-column-gap: 10%;
}
.work-backgroundShape {
  grid-area: image;
  background-color: rgba(97, 132, 153, 0.1);
  position: absolute;
  top: -1rem;
  left: -5%;
  width: 105%;
  height: 60%;
  max-height: 300px;
  background-size: cover;
  border-radius: 2px 2px 5rem 2px;
  transform: rotate(3deg);
  transition: ease 0.5s;
}
.work-header {
  grid-area: title;
  overflow: hidden;
  margin-bottom: 1rem;
}
.work-heading {
  font-size: 4rem;
  text-shadow: 2px 2px 2px rgb(160, 160, 160);
  margin-bottom: 2rem;
  overflow-wrap: break-word;
  word-wrap: break-word;
  hyphens: auto;
}
.work-heading--alps {
  color: #e5690b;
}
.work-heading--taiko {
  color: #ff3a36;
}
.work-heading--eServices {
  color: #935e92;
}
.work-heading--bertus {
  color: #2a4980;
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
.work-image {
  grid-area: image;
}
.work-img {
  z-index: 2;
  grid-column: 5 / 6;
  width: 95%;
  max-height: 300px;
  object-fit: cover;
  object-position: 0 0;
  background-color: rgba(97, 132, 153, 0.25);
  border-radius: 5px;
  /* padding-top: 2rem; */
  position: relative;
  place-self: start start;
  /* margin-top: 5rem; */
  filter: drop-shadow(8px 4px 15px grey);
  transform: rotate(5deg);
  transition: ease 0.4s;
}
.work-image:hover .work-img {
  transform: rotate(0deg);
  width: 100%;
}
.work-image:hover .work-backgroundShape {
  transform: rotate(0deg);
  width: 110%;
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
  width: 90%;
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
  grid-area: body;
  z-index: 2;
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
.skill-nuggets li {
  padding: 0.25rem;
  color: rgb(97, 102, 107);
  text-transform: uppercase;
  border: 2px solid rgb(97, 102, 107);
  font-size: 0.7rem;
  line-height: 0.7rem;
  border-radius: 2px;
  display: flex;
  align-content: center;
}
@media only screen and (max-width: 800px) {
  .alps-body {
    grid-column: 2 / 6;
  }
}
@media only screen and (max-width: 1150px) {
  .work {
    grid-template-columns: 1fr 1fr;
    grid-template-areas:
      'title title'
      'body image';
  }
  .work-header {
    margin-bottom: 2rem;
  }
}
@media only screen and (max-width: 600px) {
  .intro {
    grid-template-columns: 0.5fr 1fr 0.5fr;
    grid-template-rows: auto auto auto;
    grid-template-areas:
      '. image .'
      'title title title'
      'body body body';
  }
  .intro-header {
    text-align: center;
    place-content: center center;
  }
  .intro-heading {
    padding-top: 2rem;
    font-size: 2.5rem;
    line-height: 3rem;
    margin-bottom: 0;
  }
  .intro-heading-greeting {
    font-size: 1rem;
    line-height: 1rem;
  }
  .intro-body {
    text-align: center;
  }
  .work {
    grid-template-columns: 1fr;
    grid-template-areas:
      'title'
      'image'
      'body';
  }
  .work-heading {
    font-size: 2rem;
  }
  .work-image {
    margin-bottom: 2rem;
  }
}
</style>
