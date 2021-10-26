<template>
  <div class="skillset">
    <Skill name="Physics" rate="92%" class-name="phys" />
    <Skill name="English" rate="90%" class-name="eng" />
    <Skill name="Python" rate="86%" class-name="py" />
    <Skill name="Django" rate="80%" class-name="dj" />
    <Skill name="Javascript" rate="77%" class-name="js" />
    <Skill name="Html" rate="75%" class-name="html" />
    <Skill name="Css" rate="73%" class-name="css" />
    <Skill name="Vue" rate="72%" class-name="vue" />
    <Skill name="Git" rate="69%" class-name="git" />
    <Skill name="Typescript" rate="58%" class-name="ts" />
    <Skill name="Docker" rate="46%" class-name="dk" />
    <Skill name="AWS" rate="42%" class-name="aws" />
    <Skill name="Design" rate="27%" class-name="des" />
  </div>
</template>

<style lang="scss" scoped>
.skillset {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(333px, 1fr));
  grid-auto-rows: auto;
  column-gap: 1em;
}
</style>
