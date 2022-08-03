<template>
  <div class="d-flex">
    <div class="mr-1">
      <NuxtLink to="/projects">portfolio</NuxtLink>
    </div>
    <div class="ml-1">
      <NuxtLink to="/about">about me</NuxtLink>
    </div>
  </div>
</template>

<style lang="scss" scoped>
  a {
  color: color('light', 'darkest');
  position: relative;
  font-weight: 500;
  &:hover {
    color: color('light');
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
