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
.nav-item {
  color: #055612;
  text-decoration: none;
  font-size: 1rem;
  padding: 0.2rem;
  &:hover {
    transform: scale(1.1);
    border-radius: 10px;
    background-color: #29c936;
  }
}
</style>
