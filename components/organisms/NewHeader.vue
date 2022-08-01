<template>  
  <b-row class="new-header py-4 pl-5 text-align">
    <NuxtLink to='/'>
      <HelloWorld />
    </NuxtLink>
  </b-row>
</template>

<style lang='scss' scoped>
  .new-header {
    background-color: color('dark', 'darkest');
    box-shadow: -1px 8px 15px 5px rgba(color('dark', 'lightest'), 0.75);
    border-radius: 0 0 15px 10px;
    a {
      &:hover {
        text-decoration: none;
      }
    }
  }
</style>