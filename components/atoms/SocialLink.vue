<template>
  <a class="social-link" :href="to">
    <img :src="iconPath" :alt="name" />
  </a>
</template>

<script lang="ts">
import Vue from 'vue'

export default Vue.extend({
  props: {
    name: { type: String, required: true },
    icon: { type: String, required: true },
    to: { type: String, required: true },
  },
  computed: {
    iconPath(): string {
      return require(`@/assets/images/icons/${this.icon}`)
    },
  },
})
</script>

<style lang="scss" scoped>
.social-link {
  background-color: color('dark');
  width: 35px;
  height: 35px;
  border-radius: 3em;
  display: grid;
  justify-items: center;
  align-items: center;
  transition: transform 0.2s linear;
  &:hover {
    transform: scale(1.1);
  }
  img {
    width: 18px;
    height: 18px;
  }
}
</style>
