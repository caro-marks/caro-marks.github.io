<template>
  <b-row class="m-auto py-3">    
    <a class="py-2 vw-100 text-center social-link" :href="to">
      {{ name }}
    </a>
  </b-row>
</template>

<script lang="ts">
import Vue from 'vue'

export default Vue.extend({
  props: {
    name: { type: String, required: true },
    to: { type: String, required: true },
  }
})
</script>

<style lang="scss" scoped>
.social-link {
  border-radius: 3em;
  background-color: rgba(color('light', 'darkest'), 0.30);
  color: color('light');
  box-shadow: 1px 1px 10px 1px rgba(color('light', 'lightest'), 0.65);
  &:hover {
    text-decoration: none;
    // transform: scale(1.02);
    box-shadow: 1px 1px 15px 2px rgba(color('light', 'lightest'), 0.65);
  }
}
</style>
