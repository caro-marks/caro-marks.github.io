<template>
  <div class="presentation">
    <div class="hi">
      <span>I am</span>
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
@import url('https://fonts.googleapis.com/css2?family=Montserrat');
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
      color: #c8e0f4;
      font-family: Montserrat;
      font-style: oblique;
    }
  }
  .selfie {
    max-width: 18rem;
    justify-self: center;
    border-radius: 150px;
  }
}

@media only screen and (max-width: 915px) {
  .presentation {
    display: flex;
    flex-direction: column;
    align-items: center;
    max-width: 100vw;
    .hi {
      column-gap: 1.5rem;
    }
  }
}
</style>
