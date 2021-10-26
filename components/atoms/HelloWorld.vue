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
    color: #c8e0f4;
    font-size: 1rem;
    font-family: 'Montserrat';
    border-right: 0.15em solid #9dd1f1; /* The typwriter cursor */
    white-space: nowrap; /* Keeps the content on a single line */
    margin: 0 auto; /* Gives that scrolling effect as the typing happens */
    letter-spacing: 0.1em; /* Adjust as needed */
    animation: typing 3.5s steps(40, end), blink-caret 0.75s step-end infinite;
  }
}
@keyframes typing {
  from {
    width: 0;
  }
  to {
    width: 100%;
  }
}
@keyframes blink-caret {
  from,
  to {
    border-color: transparent;
  }
  50% {
    border-color: #9dd1f1;
  }
}
</style>
