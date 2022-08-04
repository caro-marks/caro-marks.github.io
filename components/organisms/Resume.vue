<template>
  <div class="resume my-4">
    <h3>Hi, there! Please to meet me (;</h3>

    <SkillView />
    
    <br />
    <div class="d-flex justify-content-center">
      <b-button v-b-toggle.collapse-data class="more w-50 text-center p-1">
        Ideas and Ideals
      </b-button>
    </div>
    <b-collapse id="collapse-data" class="mt-4">
      <div role="tablist">
        <div class="d-flex justify-content-center p-1" role="tab"><b-button v-b-toggle.whoami class="more w-75"><h5>Who and where am I?</h5></b-button></div>
        <b-collapse id="whoami">
          <p class="text-center">I'm Marcos Nolasco, 28-y brazilian, born at Porto Velho - RO, and living
          nowadays at Florianópolis - SC.</p>
        </b-collapse>

        <div class="d-flex justify-content-center p-1" role="tab"><b-button v-b-toggle.hobbies class="more w-75"><h5>What hobbies do I have?</h5></b-button></div>
        <b-collapse id="hobbies">
          <p class="text-center">I've been a compulsive reader since childhood, and I enjoy to watch movies
          a lot.</p>
        </b-collapse>

        <div class="d-flex justify-content-center p-1" role="tab"><b-button v-b-toggle.wanties class="more w-75"><h5>What do I want most?</h5></b-button></div>
        <b-collapse id="wanties">
          <p class="text-center">I hope a better world for those who will come, so I wanna help with
          educational status improvement. I also wanna travel all Earth around.</p>
        </b-collapse>

        <div class="d-flex justify-content-center p-1" role="tab"><b-button v-b-toggle.donies class="more w-75"><h5>What have I done?</h5></b-button></div>
        <b-collapse id="donies">
          <p class="text-center">I graduated at Physics college some months ago. I used to do research
          about complex biophysics systems using Python, and teach classes for Enem
          exams as volunteer.</p>
        </b-collapse>
        
        <div class="d-flex justify-content-center p-1" role="tab"><b-button v-b-toggle.doinges class="more w-75"><h5>What have I been doing?</h5></b-button></div>
        <b-collapse id="doinges">
          <p class="text-center">Since half of 2020 I've been working to become a full-stack developer. I
          did some jobs as backend using Django, and also some personal projects as
          frontend using Vue.</p>
        </b-collapse>
        
        <div class="d-flex justify-content-center p-1" role="tab"><b-button v-b-toggle.goinges class="more w-75"><h5>Where am I up to?</h5></b-button></div>
        <b-collapse id="goinges">
          <p class="text-center">I'm thrilling to be healthier, happier, and to achieve financial freedom.
          Have I said that I wanna travel the world?</p>
        </b-collapse>
      </div>
    </b-collapse>
  </div>
</template>
<style lang="scss" scoped>
p {
  color: rgba(color('light'), 0.9);
}
h3 {
  color: color('light')
}
h4 {
  color: rgba(rgb(225, 200, 225), 0.75);
  text-shadow: 0px 0px 1px rgba(color('light'), .5),
    0px 0px 2px rgba(color('light','lightest'), 0.25)
}
.more {
  background-color: rgba(color('light', 'darkest'), 0.8);
  border-radius: 3rem;
  color: rgb(225, 200, 225);
  font-weight: bold;
}
</style>
