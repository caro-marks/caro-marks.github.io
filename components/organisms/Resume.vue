<template>
  <div class="my-4">
    <h3>Hi, there! Please to meet me (;</h3>
    <h4> I've been a programmer since 2019, initially as a data analyst and lately as a FullStack web developer.</h4>
    <br />
    <SkillView />
    <br />
    <h4>I have professional experience using Python frameworks (<strong>Django</strong> and <strong>Sanic</strong>) for Backend development, and Javascript frameworks (<strong>React.js</strong> and <strong>Vue.js</strong>) for Frontend development.</h4>

    <div class="accordion" role="tablist">
      
      <h5>Below are some skills and trivia facts.</h5>
      <SkillSet />
    
      <Quests />
    </div>
  </div>
</template>
<style lang="scss" scoped>
h3 {
  color: color('light');
  text-align: center;
}
h4, h5 {
  text-align: justify;
  color: rgb(225, 200, 225);

}
</style>
