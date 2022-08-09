<template>  
  <b-row class="new-footer py-2 px-1 d-flex justify-content-around">
    <div v-for="item in footList" :key="item.id">
      {{ item }}
    </div>
    
  </b-row>
</template>
<script lang="ts">
import Vue from 'vue'
export default Vue.extend({
  data: () => {
    return {
      footList: ['Contact me!', 'E-mail: marcosabn08@gmail.com', 'WhatsApp: +55 48 93618 0541']
    }
  }
})
</script>
<style lang="scss">
  .new-footer {
    background-color: color('dark', 'darkest');
    color: color('light', 'lightest');
    box-shadow: -1px 4px 13px 10px rgba(color('light', 'darkest'), 0.65);
  }
</style>