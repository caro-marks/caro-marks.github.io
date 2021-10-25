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
    </div>
  </div>
</template>

<style lang="scss" scoped>
.presentation {
  display: grid;
  grid-template-columns: repeat(2, 1fr);
  align-items: center;
  margin: 0.5rem auto;
  .hey {
    justify-self: center;
  }
  .selfie {
    max-width: 13rem;
    border-radius: 150px;
  }
  .ho {
    display: grid;
    grid-template-rows: 1fr 40%;
    text-align: center;
    align-items: center;
    .my-name {
      display: grid;
      grid-template-rows: 25% 55% auto;
      row-gap: 1rem;
      color: color('dark', 'darkest');
      span {
        font-size: 2rem;
      }
      .logo {
        font-size: 3rem;
      }
      p {
        font-size: 1rem;
      }
    }
  }
}
@include screen('small', 'medium') {
  .presentation {
    grid-template-rows: 1fr 1fr;
    grid-template-columns: 1fr;
    justify-items: center;
  }
}
</style>
