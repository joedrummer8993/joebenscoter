<template>
  <main class="grid-row grid">
    <section class="grid-row grid intro">
      <div class="intro-body" style="padding-bottom: 5rem;">
        <h1>Hi. I'm Joe.</h1>
        <p>I'm passionate about making people's lives better through thoughtful software. I love the challenge of bringing new ideas to life and thrive in the tension of balancing business goals with customer needs.</p>
        <p>I've been the sole designer on a small, tight knit product team for the past 5 years building the future of B2B eCommerce. I've lead our team through a complete redesign of our company's core product. Together, we redefined everything from data structures to art direction. I certainly made mistakes along the way, but am very proud of what we were able to accomplish. We've found that thoughtful and prompt communication makes or breaks great product ideas. I am confident in my skills and am excited at the prospect of having an even bigger impact.</p>
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
    <section class="grid-row grid work work--alps">
      <div class="work-background work-background--alps"></div>
      <div class="work-body">
        <article class="card">
          <div class="card-body">
            <h2>alpscontrols.com Complete Overhaul</h2>
            <h3>Product Design & Front-end Development</h3>
            <p>From 2016 to present, I've led the redesign and feature development of the customer facing ecommerce platform that eParts licensces to its clients. This was a ground up rewrite and redesign that involved switching to a modern tech stack and design language. I conducted ethnographic interviews in the field in order to create personas that would help us understand user needs and pain points. The new platform has a fresh, re-brandable, mobile responsive interface that is both easier to use and easier on the eyes.</p>
            <!-- <a class="link">Read more about my process -></a> -->
          </div>
        </article>
      </div>
    </section>
    <section class="grid-row grid work work--bertus">
      <div class="work-background work-background--bertus"></div>
      <div class="work-body">
        <article class="card">
          <div class="card-body">
            <h2>Educational Jewelry Site Mockup</h2>
            <h3>UI Design</h3>
            <p>There are many eye catching gem stones that people don't know much about. This design was all about presenting information about gemstones to people in a way that matched the beauty of the gemstones themselves.</p>
            <!-- <a class="link">Read more about my process -></a> -->
          </div>
        </article>
      </div>
    </section>
  </main>
</template>

<style>
.intro-body {
  grid-column: 2 / 6;
  padding: 5rem 0;
}
.work {
  overflow: hidden;
  position: relative;
}
.work--alps {
  background-color: #f8b37e;
}
.work--bertus {
  background-color: rgb(183, 209, 224);
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
      rgba(248, 179, 126, 0.25),
      rgba(248, 179, 126, 1)
    ),
    url('~assets/alpscontros4.PNG');
}
.work-background--bertus {
  background-image: radial-gradient(
      ellipse closest-side,
      rgba(183, 209, 224, 0.25),
      rgba(183, 209, 224, 1)
    ),
    url('~assets/Bertus-details.PNG');
}
.work-body {
  grid-column: 2 / 5;
  z-index: 2;
  padding: 5rem 0;
}
.work-body--right {
  grid-column: 3 / 6;
}
@media only screen and (max-width: 800px) {
  .alps-body {
    grid-column: 2 / 6;
  }
}
</style>
