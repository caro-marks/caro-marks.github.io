<template>
  <div class="typewriter">
    <h1>{{ logo }}</h1>
  </div>
</template>

<script lang="ts">
import Vue from 'vue'
export default Vue.extend({
  data() {
    return {
      logo: 'HELLO WORLD',
    }
  },
})
</script>

<style lang="scss" scoped>
.typewriter {
  width: max-content;
  transition: all 0.5s;
  &:hover {
    transform: scale(1.05);
    border-radius: 10px;
    cursor: pointer;
  }
  h1 {
    // width: 100%;
    overflow: hidden; /* Ensures the content is not revealed until the animation */
    color: color('light', 'lightest');
    font-size: 1.3rem;
    font-family: 'Montserrat';
    white-space: nowrap; /* Keeps the content on a single line */
    margin: 0 auto; /* Gives that scrolling effect as the typing happens */
    letter-spacing: 0.6em; /* Adjust as needed */
    animation: flicker 1.5s infinite alternate;
  }
}
@keyframes flicker {
  0%, 18%, 22%, 25%, 53%, 57%, 100% {
    text-shadow:
      0 0 1px color('light', 'lightest'),
      0 0 2px color('light', 'lightest'),
      0 0 4px color('light', 'lightest'),
      0 0 8px color('light'),
      0 0 16px color('light'),
      0 0 32px color('light'),
      0 0 64px color('light', 'darkest'),
      // 0 0 150px color('light', 'darkest');
  }
  20%, 24%, 55% {       
    text-shadow: none;
  }
}
</style>
