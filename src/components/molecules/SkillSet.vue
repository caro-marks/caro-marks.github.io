<template>
  <div class="skill-set">
    <Skill name="Physics" rate="92%" className="phys" />
    <Skill name="English" rate="90%" className="eng" />
    <Skill name="Python" rate="86%" className="py" />
    <Skill name="Django" rate="80%" className="dj" />
    <Skill name="Javascript" rate="77%" className="js" />
    <Skill name="Html" rate="75%" className="html" />
    <Skill name="Css" rate="73%" className="css" />
    <Skill name="Vue" rate="72%" className="vue" />
    <Skill name="Git" rate="69%" className="git" />
    <Skill name="Typescript" rate="58%" className="ts" />
    <Skill name="Docker" rate="46%" className="dk" />
    <Skill name="AWS" rate="42%" className="aws" />
    <Skill name="Design" rate="27%" className="des" />
  </div>
</template>

<script lang="ts">
import { defineComponent } from 'vue'
import { Skill } from '@/components/atoms'

export default defineComponent({
  components: { Skill }
})
</script>

<style lang="scss" scoped>
.skill-set {
  width: 100%;
}
</style>
