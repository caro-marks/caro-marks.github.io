<template>
  <header class="header">
    <nav>
      <b-nav class="items">
        <b-nav-item class="item">
          <NuxtLink to="/">
            <HelloWorld />
          </NuxtLink>
        </b-nav-item>
        <b-nav-item class="item">
          <NuxtLink to="/skills">SKILLS</NuxtLink>
        </b-nav-item>
        <b-nav-item class="item">
          <NuxtLink to="/projects">PROJECTS</NuxtLink>
        </b-nav-item>
        <b-nav-item class="item">
          <NuxtLink to="/about">ABOUT</NuxtLink>
        </b-nav-item>
      </b-nav>
    </nav>
  </header>
</template>

<style lang="scss" scoped>
.header {
  display: grid;
  justify-content: center;
  nav {
    box-shadow: -1px 8px 26px 5px rgba(color('dark'), 0.85);
    background: color('dark', 'darkest');
    width: max-content;
    height: 50px;
    padding: 0 2rem;
    border-radius: 35px;
    align-items: center;
    .items {
      display: grid;
      grid-template-columns: 40% auto auto auto;
      align-items: center;
      justify-content: space-between;
      height: 100%;
      .item a {
        color: color('light', 'darkest');
        position: relative;
        font-weight: 500;
        &:hover {
          color: color('dark');
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
}
</style>
