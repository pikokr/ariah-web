<template>
  <div>
    <span
      v-for="(t, i) in text"
      :key="i"
      :style="{ animationDelay: i * 70 + 'ms' }"
      class="t"
      v-text="t"
    />
  </div>
</template>

<script lang="ts">
export default {
  name: 'AnimatedText',
  props: {
    text: {
      type: String,
      default: '',
    },
  },
}
</script>

<style scoped>
@keyframes text-in {
  0% {
    transform: translateX(80px);
    opacity: 0;
  }
}

.t {
  display: inline-block;
  min-width: 0.3em;
  animation: text-in 0.8s cubic-bezier(0.69, -0.91, 0.35, 1.94) backwards;
}
</style>
