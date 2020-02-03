<template>
  <div>
    <Focuses />
    <About />
  </div>
</template>

<script>
import Focuses from '~/components/focuses.vue'
import About from '~/components/about.vue'

export default {
  name: 'Index',

  components: {
    Focuses,
    About
  }
}
</script>
