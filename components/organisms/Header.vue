<template>
  <header class="header">
    <nav>
      <div class="items">
        <div class="item">
          <NuxtLink to="/">
            <HelloWorld />
          </NuxtLink>
        </div>
        <div class="item">
          <NuxtLink to="/skills">SKILLS</NuxtLink>
        </div>
        <div class="item">
          <NuxtLink to="/projects">PROJECTS</NuxtLink>
        </div>
        <div class="item">
          <NuxtLink to="/sobre">ABOUT</NuxtLink>
        </div>
      </div>
    </nav>
  </header>
</template>

<style lang="scss" scoped>
.header {
  display: grid;
  justify-content: center;
  nav {
    box-shadow: -1px 8px 26px 5px rgba(color('dark', 'darkest'), 0.55);
    background: color('dark', 'base');
    width: 450px;
    height: 50px;
    padding: 0 10px;
    border-radius: 35px;
    align-items: center;
    .items {
      display: grid;
      grid-template-columns: 40% auto auto auto;
      align-items: center;
      justify-content: space-between;
      height: 100%;
    }
    .item a {
      color: color('light');
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
        background: color('light', 'darkest');
        left: 0;
        bottom: -16px;
      }
    }
  }
}
</style>
