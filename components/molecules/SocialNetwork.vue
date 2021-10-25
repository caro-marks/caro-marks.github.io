<template>
  <div class="social-networks">
    <SocialLink
      name="Github"
      icon="github.svg"
      to="https://www.github.com/caro-marks"
    />
    <SocialLink
      name="Linkedin"
      icon="linkedin.svg"
      to="https://www.linkedin.com/in/caro-marks"
    />
    <SocialLink
      name="Twitter"
      icon="twitter.svg"
      to="https://www.twitter.com/carom4rks"
    />
  </div>
</template>

<style lang="scss" scoped>
.social-networks {
  display: grid;
  grid-template-columns: 1fr 1fr 1fr;
  column-gap: 0.5rem;
  // justify-items: center;
}
</style>
