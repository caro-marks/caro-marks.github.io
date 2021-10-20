<template>
  <div class="typewriter">
    <h1>
      {{ text }}
    </h1>
  </div>
</template>

<script lang="ts">
import { defineComponent } from 'vue'

export default defineComponent({
  data() {
    return {
      text: 'Hello World'
    }
  }
})
</script>

<style lang="scss" scoped>
.typewriter {
  width: max-content;
  h1 {
    overflow: hidden; /* Ensures the content is not revealed until the animation */
    color: #055612;
    font-size: 3rem;
    border-right: 0.15em solid #91c321; /* The typwriter cursor */
    white-space: nowrap; /* Keeps the content on a single line */
    margin: 0 auto; /* Gives that scrolling effect as the typing happens */
    letter-spacing: 0.15em; /* Adjust as needed */
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
    border-color: #91c321;
  }
}
</style>
