<template>
  <div class="grid">
    <heading/>
    <nuxt/>
    <footer>
      &copy; 2019 - Joe Benscoter
    </footer>
  </div>
</template>

<script>
import Heading from '~/components/Heading.vue'

export default {
  components: {
    Heading
  }
}
</script>

<style>
html {
  font-family: 'Scada', -apple-system, BlinkMacSystemFont, Roboto,
    'Helvetica Neue', Arial, sans-serif;
  font-size: 16px;
  word-spacing: 1px;
  line-height: 1.5rem;
  -ms-text-size-adjust: 100%;
  -webkit-text-size-adjust: 100%;
  -moz-osx-font-smoothing: grayscale;
  -webkit-font-smoothing: antialiased;
  box-sizing: border-box;
  color: rgb(50, 50, 50);
  padding: 0;
}
h1 {
  font-size: 3rem;
  line-height: 4rem;
  margin-top: 0;
}
body {
  font-family: 'Scada', sans-serif;
  padding: 0;
  margin: 0;
  /* background: #eee; */
}
p {
  padding: 0;
  margin: 0;
}
a {
  text-decoration: none;
  color: rgb(39, 105, 190);
}
a:hover {
  color: rgb(21, 65, 122);
}
.grid {
  display: grid;
  grid-template-columns: 1fr 2fr 1fr 1fr 2fr 1fr;
  grid-column-gap: 1rem;
  grid-row-gap: 0;
  margin: 0;
}

.grid-row {
  grid-column: 1 / -1;
}

footer {
  grid-column: 1 / -1;
  place-self: center center;
  margin: 0.5rem;
}

@media only screen and (max-width: 1400px) {
  .grid {
    grid-template-columns: 0.25fr 2fr 1fr 1fr 2fr 0.25fr;
  }
}
</style>
