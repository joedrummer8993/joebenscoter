<template>
  <header class="grid-row grid heading">
      
        <logo class="heading__logo"/>

      <!-- <nav class="mainNav">
        <ul class="list-row">
          <li><a href="">Home</a></li>
          <li><a href="#work">Work</a></li>
          <li><a href="">Contact</a></li>
        </ul>
      </nav> -->
  </header>
</template>

<script>
import Logo from '~/components/Logo.vue'

export default {
  components: {
    Logo
  }
}
</script>

<style>
.heading {
  align-items: center;
  padding: 1rem 0;
  position: sticky;
  top: 0;
  background-color: white;
  opacity: 50%;
  z-index: 100;
  /* box-shadow: 2px 2px 4px grey; */
  display: flex;
  justify-content: space-between;
  align-items: center;
  column-span: 2 / 6;
}
.heading__logo {
  display: block;
  grid-column: 2 / 4;
  width: 100%;
  max-width: 10rem;
  /* min-width: 15rem; */
  height: auto;
}
.mainNav {
  grid-column: 4 / 6;
  place-self: center end;
}
.mainNav a {
  color: slategray;
}
.mainNav li a:visited {
  color: slategray;
}
.list-row {
  display: flex;
  list-style-type: none;
  flex-flow: row wrap;
  margin: 0;
  padding: 0;
}
.list-row li {
  flex: 0 0 auto;
  margin-right: 0.5rem;
  margin-bottom: 0.5rem;
}
.list-row li:last-child {
  margin-right: 0;
}
</style>
