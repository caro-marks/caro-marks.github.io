<template>
  <div class="presentation">
    <Logo />
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
  width: 100%;
  display: grid;
  justify-content: center;
  row-gap: 1.5rem;
  .selfie {
    max-width: 18rem;
    justify-self: center;
    border-radius: 150px;
  }
  .social-networks {
    justify-self: center;
  }
}
@media only screen and (min-width: 700px) {
  .presentation {
    width: 50%;
  }
}
</style>
