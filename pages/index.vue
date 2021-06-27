<template>
  <div class="w-screen h-screen flex justify-center items-center">
    <h1 class="text-7xl font-black"><animated-text text="TEAM ARIAH" /></h1>
  </div>
</template>

<script lang="ts">
import Vue from 'vue'
import AnimatedText from '~/components/animatedText.vue'

export default Vue.extend({
  components: { AnimatedText },
})
</script>
