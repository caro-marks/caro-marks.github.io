<template>
  <a class="social-link" :href="to">
    <img :src="iconPath" :alt="name" />
  </a>
</template>

<script lang="ts">
import { defineComponent } from 'vue'

export default defineComponent({
  props: {
    name: { type: String, required: true },
    icon: { type: String, required: true },
    to: { type: String, required: true }
  },
  computed: {
    iconPath(): string {
      return require(`@/assets/images/icons/${this.icon}`)
    }
  }
})
</script>

<style lang="scss" scoped>
.social-link {
  background-color: #031927;
  width: 50px;
  height: 50px;
  border-radius: 5rem;
  display: grid;
  justify-items: center;
  align-items: center;
  transition: transform 0.2s linear;
  &:hover {
    transform: scale(1.1);
  }
  img {
    width: 25px;
    height: 25px;
  }
}
</style>
