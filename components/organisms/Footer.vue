<template>
  <div>
    <footer class="footer">
      <Container>
        <Logo />
        <SocialNetwork />
      </Container>
    </footer>
  </div>
</template>

<style lang="scss" scoped>
.footer {
  width: 100%;
  height: 110px;
  background: color(dark, darkest);
  .container {
    display: grid;
    height: 100%;
    grid-auto-flow: column;
    justify-content: space-around;
    align-items: center;
    p {
      color: color('light', 'darkest');
    }
  }
}
</style>
