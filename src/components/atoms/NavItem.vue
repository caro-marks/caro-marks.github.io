<template>
  <a class="nav-item" :href="to">
    {{ text }}
  </a>
</template>

<script lang="ts">
import { defineComponent } from 'vue'

export default defineComponent({
  props: {
    text: { type: String, required: true },
    to: { type: String, required: true }
  }
})
</script>

<style lang="scss" scoped>
@import url('https://fonts.googleapis.com/css2?family=Montserrat');
.nav-item {
  color: #9dd1f1;
  text-decoration: none;
  font-size: 1rem;
  font-family: Montserrat;
  padding: 0.2rem;
  &:hover {
    transform: scale(1.1);
    border-radius: 10px;
    color: #031927;
    background-color: #508aa8;
  }
}
</style>
