<template>
  <div class="box-skill">
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
  margin: 1rem 0;
  text-align: center;
  .title {
    color: #031927;
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
      color: color('light');
      background-color: color('dark', 'darkest');
      border-radius: 25px 10px 10px 25px;
    }
    .js {
      width: 77%;
    }
    .ts {
      width: 58%;
    }
    .html {
      width: 75%;
    }
    .css {
      width: 73%;
    }
    .vue {
      width: 72%;
    }
    .dj {
      width: 80%;
    }
    .py {
      width: 86%;
    }
    .dk {
      width: 46%;
    }
    .git {
      width: 69%;
    }
    .aws {
      width: 42%;
    }
    .eng {
      width: 90%;
    }
    .des {
      width: 27%;
    }
    .phys {
      width: 92%;
    }
  }
}
</style>
