<template>
  <b-container class="pb-5">
    <b-row class="d-flex justify-content-center">
      <img class="selfie" src="@/assets/images/selfie.jpeg" alt="Me smiling!" />
    </b-row>
    <b-row class="d-flex flex-column align-items-center">
      <h4 class="mt-2">Marcos Nolasco</h4>
      <h5>
        Software Enginner and Physicist Educator
      </h5>
    </b-row>
  </b-container>
</template>
<style lang="scss" scoped>
  .selfie {
    max-width: 10rem;
    border: 5px solid color('light');
    border-radius: 40%;
  }
  h4, h5 {
    color: color('light');
  }
</style>