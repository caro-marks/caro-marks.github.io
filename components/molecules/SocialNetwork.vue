<template>
  <b-container class="m-auto">
    <b-row class="py-3 m-auto">
      <NuxtLink class="py-2 vw-100 text-center cv" to="/cv">Curriculum Vitae</NuxtLink>
    </b-row>
    <SocialLink
      name="Linkedin"
      to="https://www.linkedin.com/in/caro-marks"
    />
    <SocialLink
      name="Dev.To"
      to="https://dev.to/caromarks"
    />
    <SocialLink
      name="SlackShare"
      to="https://stackshare.io/caro-marks"
    />
    <SocialLink
      name="Github"
      to="https://www.github.com/caro-marks"
    />
    <SocialLink
      name="Twitter"
      to="https://twitter.com/MarquetipS"
    />
  </b-container>
</template>
<style lang="scss" scoped>

  .cv {
    border-radius: 3em;
    background-color: rgba(color('light', 'darkest'), 0.75);
    color: color('light');
    box-shadow: 1px 1px 10px 1px rgba(color('light', 'lightest'), 0.65);
    &:hover {
      text-decoration: none;
      // transform: scale(1.02);
      box-shadow: 1px 1px 15px 2px rgba(color('light', 'lightest'), 0.65);
    }
  }
</style>
