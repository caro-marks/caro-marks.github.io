<template>
  <div class="presentation">
    <div class="hi">
      <span>I'm</span>
      <Logo />
    </div>
    <img class="selfie" src="@/assets/images/selfie.jpeg" alt="Me smiling!" />
    <SocialNetwork />
  </div>
</template>

<script lang="ts">
import { defineComponent } from 'vue'
import { Logo } from '@/components/atoms'
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
    Logo,
    SocialNetwork
  }
})
</script>

<style lang="scss" scoped>
.presentation {
  padding: 0 0.5rem;
  max-width: 50%;
  min-width: 450px;
  display: grid;
  justify-content: center;
  row-gap: 1.5rem;
  .hi {
    display: grid;
    grid-template-columns: 1fr auto;
    text-align: center;
    align-items: center;
    padding: 0.2rem 0;
    span {
      font-size: 2.5rem;
      font-family: serif;
      font-style: oblique;
    }
  }
  .selfie {
    max-width: 18rem;
    justify-self: center;
    border-radius: 150px;
  }
}
// @media only screen and (min-width: 700px) {
//   .presentation {
//     width: 50%;
//   }
// }
</style>
