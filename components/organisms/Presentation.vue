<template>
  <div class="presentation">
    <div class="hey">
      <img class="selfie" src="@/assets/images/selfie.jpeg" alt="Me smiling!" />
    </div>
    <div class="ho">
      <div class="my-name">
        <span>My name is </span>
        <div class="logo">MARCOS.</div>
        <ul class="roles">
          <li class="role">Developer</li>
          <li class="role">Physicist</li>
          <li class="role">Educator</li>
        </ul>
      </div>
    </div>
  </div>
</template>

<style lang="scss" scoped>
.presentation {
  height: max-content;
  display: grid;
  grid-template-columns: repeat(2, 1fr);
  align-items: center;
  margin: 0.95rem auto -1em;
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
      grid-template-rows: 15% 35% auto;
      row-gap: 1rem;
      color: color('dark', 'darkest');
      span {
        font-size: 2rem;
      }
      .logo {
        font-size: 3rem;
        font-weight: bold;
      }
      ul {
        display: grid;
        grid-auto-rows: 2em;
        row-gap: 0.75em;
        li {
          font-size: 1.5rem;
        }
      }
    }
  }
}
@include screen('small', 'medium') {
  .presentation {
    grid-template-rows: 1fr 1fr;
    grid-template-columns: 1fr;
    justify-items: center;
    .ho {
      .my-name {
        ul {
          grid-auto-flow: column;
          column-gap: 0.75em;
        }
      }
    }
  }
}
</style>
