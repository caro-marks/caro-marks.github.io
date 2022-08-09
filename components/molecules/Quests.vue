<template>
  <div class="mt-3">
    <div class="d-flex justify-content-center" role="tab">
      <b-button v-b-toggle.collapse-data class="more w-50 text-center p-1">
        Ideas and Ideals
      </b-button>
    </div>
    <b-collapse id="collapse-data" accordion="r-accordion" class="mt-2 quests py-2">
      <div class="accordion" role="tablist">
        <div class="d-flex justify-content-center p-1" role="tab"><b-button v-b-toggle.whoami class="more w-75"><h5>Who and where am I?</h5></b-button></div>
        <b-collapse id="whoami" visible accordion="q-accordion">
          <p class="text-center">I'm Marcos Nolasco, 29-y brazilian, born at Porto Velho - RO, and living
          nowadays at Florianópolis - SC.</p>
        </b-collapse>

        <div class="d-flex justify-content-center p-1" role="tab"><b-button v-b-toggle.hobbies class="more w-75"><h5>What hobbies do I have?</h5></b-button></div>
        <b-collapse id="hobbies" accordion="q-accordion">
          <p class="text-center">I've been a passionate reader since childhood, and I enjoy to watch movies and series
          a lot.</p>
        </b-collapse>

        <div class="d-flex justify-content-center p-1" role="tab"><b-button v-b-toggle.wanties class="more w-75"><h5>What do I want most?</h5></b-button></div>
        <b-collapse id="wanties" accordion="q-accordion">
          <p class="text-center">I hope a better world for those who will come, so I wanna help with
          educational status improvement.</p>
        </b-collapse>

        <div class="d-flex justify-content-center p-1" role="tab"><b-button v-b-toggle.donies class="more w-75"><h5>What have I done?</h5></b-button></div>
        <b-collapse id="donies" accordion="q-accordion">
          <p class="text-center">I graduated at Physics college in early 2021. I used to do research
          about complex biophysics systems using Python, and teach classes for Enem
          exams as volunteer. </p>
        </b-collapse>
        
        <div class="d-flex justify-content-center p-1" role="tab"><b-button v-b-toggle.doinges class="more w-75"><h5>What have I been doing?</h5></b-button></div>
        <b-collapse id="doinges" accordion="q-accordion">
          <p class="text-center"> I
          did some jobs as backend using Django and Sanic, and some jobs as frontend
          frontend using React and Vue.</p>
        </b-collapse>
        
        <div class="d-flex justify-content-center p-1" role="tab"><b-button v-b-toggle.goinges class="more w-75"><h5>Where am I up to?</h5></b-button></div>
        <b-collapse id="goinges" accordion="q-accordion">
          <p class="text-center">I'm thrilling to be healthier, happier, and to achieve financial freedom.
          Have I said that I wanna travel the world?</p>
        </b-collapse>
      </div>
    </b-collapse>
  </div>
</template>

<style lang="scss" scoped>
  p {
    color: rgb(225, 200, 225);
  }
  h4 {
    color: rgba(rgb(225, 200, 225), 0.75);
    text-shadow: 0px 0px 1px rgba(color('light'), .5),
      0px 0px 2px rgba(color('light','lightest'), 0.25)
  }
  .more {
    background-color: rgba(color('light', 'darkest'), 0.8);
    border: none;
    border-radius: 3rem;
    color: rgb(225, 200, 225);
    font-weight: bold;
    box-shadow: 1px 1px 10px 1px rgba(color('light', 'lightest'), 0.65);
    &:hover {
    box-shadow: 1px 1px 15px 2px rgba(color('light', 'lightest'), 0.65);
  }
  }
  .quests {
    background-color: rgba(color('light', 'darkest'), 0.5);
    border-radius: 3rem;
  }
</style>