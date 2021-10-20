<template>
  <img class="logo" src="@/assets/images/logo.svg" alt="Marcos" />
</template>

<style lang="scss" scoped>
.logo {
  width: 100%;
  padding: 0.3rem;
  transition: all 0.5s;
  &:hover {
    transform: scale(1.1);
    border-radius: 10px;
    background-color: #29c936;
    cursor: pointer;
  }
}
</style>
