<template>
  <b-container class="d-flex flex-column flex-lg-row align-items-center justify-content-md-around">
    <b-row class="skillview col-lg-5">
      <b-col>
        <b-row class="d-flex align-items-center justify-content-center py-1">
          <img class="col-3 col-sm-2" src="@/assets/images/icons/front.png" alt="front icon" />
          <h4>Front-End</h4>
        </b-row>
        <b-row class="d-flex justify-content-center h-50 py-1">
          <p class="text-center font-weight-bold">
            Build designed interfaces, with responsivity and a bit of
            UX.
          </p>
        </b-row>
      </b-col>
    </b-row>
    <b-row class="skillview col-lg-5 mt-1">
      <b-col>
        <b-row class="d-flex align-items-center justify-content-center py-1">
          <img class="col-3 col-sm-2" src="@/assets/images/icons/back.png" alt="back icon" />
          <h4>Back-End</h4>
        </b-row>
        <b-row class="d-flex justify-content-center h-50 py-1">
          <p class="text-center font-weight-bold">
              API building, DB modelling,
            server refactoring, and integrations.
          </p>
        </b-row>
      </b-col>
    </b-row>
  </b-container>
</template>

<style lang="scss" scoped>
  .skillview {
    background-color: rgba(color('light', 'darkest'), 0.5);
    border: 2px double color('dark');
    border-radius: 3rem;
  }
  img {
    max-height:80%;
  }
  h4, p {
    color: rgb(225, 200, 225)
  }
</style>
