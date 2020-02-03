<template>
  <header class="grid">
    <div class="column1">
      <p>István Vasil</p>
    </div>
    <div class="column2">
      <p>Graphic designer</p>
      <p>Developer</p>
    </div>
    <div class="column3">
      <p>Stockholm</p>
      <p>Sweden</p>
    </div>
    <div class="column4">
      <p>Focusing on ↓</p>
    </div>
  </header>
</template>

<script>
export default {
  name: 'Header'
}
</script>

<style>
header {
  padding: 1rem 1.5rem 1rem 1.5rem;
}

@media screen and (max-width: 600px) {
  header {
    padding: 1rem;
  }
}

header > div:nth-child(1) {
  grid-column: 1/3;
}

@media screen and (max-width: 600px) {
  header > div:nth-child(1) {
    grid-column: 1/-1;
  }
}

header > div:nth-child(2) {
  grid-column: 4/7;
}

@media screen and (max-width: 600px) {
  header > div:nth-child(2) {
    grid-column: 5/-1;
  }
}

.header > div:nth-child(3) {
  grid-column: 7/10;
}

@media screen and (max-width: 600px) {
  header > div:nth-child(3) {
    grid-column: 9/-1;
  }
}

header > div:nth-child(4) {
  grid-column: 10/-1;
}

@media screen and (max-width: 600px) {
  header > div:nth-child(4) {
    grid-column: 1/-1;
  }
}
</style>
