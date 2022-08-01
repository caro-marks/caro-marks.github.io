<template>
  <div class="error vh-100 d-flex flex-column align-items-center justify-content-center">
    <div v-if="error.statusCode === 404">
      <div class="text-center">
        <h1 class="display-1 fw-bold">OOPS! Nothing was found here.</h1>
      </div>
    </div>
    <div v-else>
      <h1 class="display-1 fw-bold text-white">An error occurred</h1>
    </div>
    <div class="d-flex justify-content-center">
      <b-img src="https://einoo.files.wordpress.com/2012/03/wqt3y.gif" fluid/>
    </div>
    <NuxtLink to="/">
      <h2>
        Let's go back to somewhere safe
      </h2>
    </NuxtLink>
  </div>
</template>

<script>
  export default {
    props: { error: { type: Object, default: () => {}}},
  }
</script>
<style lang="scss" scoped>
  .error {
    background-color: color('dark','darkest');
    h1 {
      color: color('dark','darkest');
      animation: flicker 1.5s infinite alternate;
    }
  }
  @keyframes flicker {
  0%, 18%, 22%, 25%, 53%, 57%, 100% {
    text-shadow:
      0 0 1px color('light', 'darkest'),
      0 0 2px color('light', 'darkest'),
      0 0 4px color('light', 'darkest'),
      0 0 8px color('light'),
      0 0 16px color('light'),
      0 0 32px color('light'),
      0 0 64px color('light', 'lightest'),
      0 0 150px color('light', 'lightest');
  }
  20%, 24%, 55% {       
    text-shadow: none;
  }
}
</style>