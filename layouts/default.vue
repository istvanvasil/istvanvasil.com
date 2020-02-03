<template>
  <main>
    <Header />
    <nuxt />
  </main>
</template>

<script>
import Header from '~/components/header.vue'

export default {
  components: {
    Header
  }
}
</script>

<style>
:root {
  --off-white: #fffffd;
  --black: #000000;
  --off-black: #222222;
  --grey: #787878;
  --type: 'Lab Grotesque', -apple-system, sans-serif;
}

html {
  font-size: 16px;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  -moz-font-feature-settings: 'kern' 1;
  -ms-font-feature-settings: 'kern' 1;
  -o-font-feature-settings: 'kern' 1;
  -webkit-font-feature-settings: 'kern' 1;
  font-feature-settings: 'kern' 1;
  font-kerning: normal;
  -webkit-text-size-adjust: none;
  background: var(--off-white);
}

*,
*:before,
*:after {
  box-sizing: border-box;
  margin: 0;
}

::-webkit-scrollbar {
  display: none;
}

body {
  background: var(--off-white);
  color: var(--off-black);
  font-family: var(--type);
  font-size: 0.875rem;
  font-weight: 400;
  line-height: 1rem;
  letter-spacing: -0.002em;
}

main {
  max-width: 1600px;
  margin: 0 auto;
}

a {
  color: var(--off-black);
  text-decoration: underline;
  text-decoration-color: rgba(var(--fg), 1);
  opacity: 1;
  transition: color 0.1s;
}

a:hover {
  color: var(--off-black);
  text-decoration: none;
}

@media (hover: none) {
  a:hover {
    color: var(--off-black);
  }
}

.responsive-type {
  font-size: calc((100vw - 3rem) * 0.118);
  line-height: 0.8;
  letter-spacing: -0.05em;
}

@media screen and (max-width: 600px) {
  .responsive-type {
    font-size: calc((100vw - 2rem) * 0.1485);
  }
}

@media screen and (min-width: 1600px) {
  .responsive-type {
    font-size: 183.136px;
  }
}

.break-single {
  margin-top: 1.125em;
}

.break-double {
  margin-top: 2.25em;
}

@font-face {
  font-family: 'Lab Grotesque';
  font-weight: 400;
  src: url('../assets/fonts/LabGrotesque-Regular.woff2') format('woff2'),
    url('../assets/fonts/LabGrotesque-Regular.woff') format('woff');
}

.grid {
  display: grid;
  grid-template-columns: repeat(12, 1fr);
  grid-gap: 1rem;
  align-items: start;
}

img,
video {
  width: 100%;
}
</style>
