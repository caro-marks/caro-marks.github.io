<template>
  <div class="presentation">
    <div class="left-top">
      <img class="selfie" src="@/assets/images/selfie.jpeg" alt="Me smiling!" />
      <div class="introducin">
        <h1 class="name">Hi, I'm Marcos.</h1>
        <ul class="roles">
          <li class="role">Developer</li>
          <li class="role">Physicist</li>
          <li class="role">Educator</li>
        </ul>
      </div>
    </div>
    <div class="right-bot">
      <SkillView />
    </div>
  </div>
</template>

<style lang="scss" scoped>
.presentation {
  display: grid;
  grid-template-columns: repeat(2, 1fr);
  margin: 0.95rem auto;
  gap: 5em;
  .left-top {
    display: grid;
    justify-items: center;
    gap: 1rem;
    .selfie {
      max-width: 13rem;
      border-radius: 100%;
    }
    .introducin {
      display: grid;
      row-gap: 1rem;
      justify-items: center;
      .roles {
        display: grid;
        row-gap: 0.5rem;
        font-size: 1.8rem;
      }
    }
  }
  .right-bot {
    display: grid;
    justify-content: center;
  }
}
// .presentation {
//   height: max-content;
//   .ho {
//     display: grid;
//     grid-template-rows: 1fr 40%;
//     text-align: center;
//     align-items: center;
//     .my-name {
//       display: grid;
//       grid-template-rows: 15% 35% auto;
//       row-gap: 1rem;
//       color: color('dark', 'darkest');
//       span {
//         font-size: 2rem;
//       }
//       .logo {
//         font-size: 3rem;
//         font-weight: bold;
//       }
//       ul {
//         display: grid;
//         grid-auto-rows: 2em;
//         row-gap: 0.75em;
//         li {
//           font-size: 1.5rem;
//         }
//       }
//     }
//   }
// }
// @include screen('small', 'medium') {
//   .presentation {
//     grid-template-rows: 1fr 1fr;
//     grid-template-columns: 1fr;
//     justify-items: center;
//     .ho {
//       .my-name {
//         ul {
//           grid-auto-flow: column;
//           column-gap: 0.75em;
//         }
//       }
//     }
//   }
// }
</style>
