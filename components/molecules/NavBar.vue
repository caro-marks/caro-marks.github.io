<template>
  <div class="nav-bar">
    <div class="nav-item">
      <NuxtLink to="/skills">SKILLS</NuxtLink>
    </div>
    <div class="nav-item">
      <NuxtLink to="/projects">PROJECTS</NuxtLink>
    </div>
    <div class="nav-item">
      <NuxtLink to="/sobre">ABOUT</NuxtLink>
    </div>
  </div>
</template>

<style lang="scss" scoped>
.nav-bar {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  align-items: center;
  justify-content: space-around;
}
.nav-item a {
  color: color('light', 'base');
  position: relative;
  font-weight: 500;
  &:hover {
    color: color('dark', 'darkest');
    text-decoration: none;
  }
  &.nuxt-link-active:after {
    content: '';
    position: absolute;
    width: 100%;
    height: 4px;
    background: color('light', 'base');
    left: 0;
    bottom: -16px;
  }
}
</style>
