<template>
  <div class="box-skill px-4">
    <h2 class="title">{{ name }}</h2>
    <div class="skill">
      <div :class="['quality', className]">{{ rate }}</div>
    </div>
  </div>
</template>

<script lang="ts">
import Vue from 'vue'
export default Vue.extend({
  props: {
    name: { type: String, required: true },
    rate: { type: String, required: true },
    className: { type: String, required: true },
  },
})
</script>

<style lang="scss" scoped>
.box-skill {
  margin: 0.5rem 0;
  text-align: center;
  .title {    
    color: rgb(225, 200, 225);
    font-size: 1em;
  }
  .skill {  
    widows: 100%;
    background-color: color('light', 'darkest');
    border-radius: 25px;
    margin-top: 3px;
    .quality {
      text-align: right;
      padding: 5px;
      font-size: 0.8rem;      
      color: rgb(225, 200, 225);
      background-color: color('dark', 'darkest');
      border-radius: 25px 10px 10px 25px;
    }
    .lgc {
      width: 92%;
    }
    .eng {
      width: 90%;
    }
    .py {
      width: 88%;
    }
    .html {
      width: 86%;
    }
    .js {
      width: 84%;
    }
    .dj {
      width: 82%;
    }
    .rct {
      width: 80%;
    }
    .css {
      width: 78%;
    }
    .vue {
      width: 76%;
    }
    .git {
      width: 68%;
    }
    .ts {
      width: 58%;
    }
    .aws {
      width: 42%;
    }
    .dk {
      width: 46%;
    }
    .des {
      width: 32%;
    }
  }
}
</style>