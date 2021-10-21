<template>
  <div class="presentation">
    <div class="hey">
      <img class="selfie" src="@/assets/images/selfie.jpeg" alt="Me smiling!" />
    </div>
    <div class="ho">
      <div class="my-name">
        <span>My name is </span>
        <div class="logo">MARCOS.</div>
        <p>Jr Full Stack Developer</p>
      </div>
      <SocialNetwork />
    </div>
  </div>
</template>

<script lang="ts">
import { defineComponent } from 'vue'
import { SocialNetwork } from '@/components/molecules'

export default defineComponent({
  data() {
    return {
      presentation: {
        physics: ''
      }
    }
  },
  components: {
    SocialNetwork
  }
})
</script>

<style lang="scss" scoped>
@import url('https://fonts.googleapis.com/css2?family=Montserrat');
.presentation {
  display: grid;
  grid-template-columns: 2fr 3fr;
  grid-template-rows: 1fr;
  align-items: center;
  margin: 1rem 4em;
  widows: 80%;
  .hey {
    justify-self: center;
  }
  .selfie {
    max-width: 18rem;
    border-radius: 150px;
  }
  .ho {
    display: grid;
    grid-template-rows: 1fr 40%;
    text-align: center;
    align-items: center;
    max-width: 90%;
    .my-name {
      display: grid;
      grid-template-rows: 20% 1fr 1fr;
      row-gap: 1rem;
      color: #c8e0f4;
      font-family: Montserrat;
      span {
        font-size: 2.5rem;
      }
      .logo {
        font-size: 4rem;
      }
      p {
        font-size: 1.5rem;
      }
    }
  }
}
@media only screen and (max-width: 915px) {
  .presentation {
    grid-template-rows: 1fr 1fr;
    grid-template-columns: 1fr;
    max-width: 100vw;
    justify-items: center;
    .ho {
      .my-name {
        background: #031927;
        border-radius: 100px;
        padding: 2rem;
      }
    }
  }
}
</style>
