<template>
  <div class="skillsview">
    <div class="skillview">
      <div class="top">
        <img src="@/assets/images/icons/front.png" alt="front icon" />
        <h3>Front-End</h3>
      </div>
      <p>
        I'm able to build designed interfaces, with responsivity and a bit of
        UX.
      </p>
    </div>
    <div class="skillview">
      <div class="top">
        <img src="@/assets/images/icons/back.png" alt="back icon" />
        <h3>Back-End</h3>
      </div>
      <p>
        I'm experienced with API build and integration, database modelling,
        refactoring, and other cool stuffs.
      </p>
    </div>
  </div>
</template>

<style lang="scss" scoped>
.skillsview {
  display: grid;
  grid-template-columns: 25em;
  row-gap: 1rem;
  .skillview {
    display: grid;
    justify-items: center;
    text-align: center;
    border: 1px solid color('dark');
    border-radius: 3rem;
    .top {
      display: grid;
      grid-auto-flow: column;
      align-items: center;
      justify-content: space-between;
      column-gap: 2rem;
      img {
        max-width: 4rem;
      }
    }
  }
}
</style>
