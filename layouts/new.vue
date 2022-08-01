<template>
  <b-container fluid class="new min-vh-100 d-flex flex-column justify-content-between">
    <NewHeader />
    <Container>
      <Nuxt />
    </Container>
    <NewFooter />
  </b-container>
</template>
<style lang='scss' scoped>
.new {
  background-color: color('dark', 'base');
}
</style>

