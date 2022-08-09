<template>
  <div class="d-flex flex-column mt-3 py-2">
    <div class="d-flex justify-content-center" role="tab">
      <b-button v-b-toggle.collapse-skills class="more text-center p-1 w-50">
      Skills
    </b-button>
    </div>
    <b-collapse id="collapse-skills" accordion="r-accordion" class="mt-2 skillset">
      <Skill name="Logic" rate="92%" class-name="lgc" />
      <Skill name="English" rate="90%" class-name="eng" />
      <Skill name="Python" rate="88%" class-name="py" />
      <Skill name="Html" rate="86%" class-name="html" />
      <Skill name="Javascript" rate="84%" class-name="js" />
      
      <Skill name="Django" rate="82%" class-name="dj" />
      <Skill name="React.js" rate="80%" class-name="rct" />
      <Skill name="CSS" rate="78%" class-name="css" />
      <Skill name="Vue.js" rate="76%" class-name="vue" />
      <Skill name="Git" rate="68%" class-name="git" />
      <Skill name="Typescript" rate="58%" class-name="ts" />
      <Skill name="Docker" rate="46%" class-name="dk" />
      <Skill name="AWS" rate="42%" class-name="aws" />
      <Skill name="Design" rate="32%" class-name="des" />
    </b-collapse>
  </div>
</template>

<style lang="scss" scoped>
.skillset {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(333px, 1fr));
  grid-auto-rows: auto;
  column-gap: 1em;
  background-color: rgba(color('light', 'darkest'), 0.5);
  border-radius: 3rem;
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
</style>
