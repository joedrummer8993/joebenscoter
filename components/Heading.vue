<template>
  <header class="heading grid-row grid">
      <div class="heading__logo">
        <logo/>
      </div>
      <nav class="mainNav">
        <ul class="list-row">
          <li>Home</li>
          <li>Work</li>
          <li>Contact</li>
        </ul>
      </nav>
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
  border-bottom: 1px solid lightgray;
  align-items: center;
  padding: 1rem 0;
}
.heading__logo {
  display: block;
  grid-column: 2 / 3;
  width: 100%;
  max-width: 20rem;
  min-width: 15rem;
  height: auto;
}
.mainNav {
  grid-column: 5 / 6;
  place-self: center end;
  display: none;
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
  margin-right: 1rem;
}
.list-row li:last-child {
  margin-right: 0;
}
</style>
