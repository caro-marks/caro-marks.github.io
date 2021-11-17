<template>
  <div class="samples">
    <b-card
      img-src="@/assets/images/ibo1.png"
      class="overflow-hidden text-center"
      footer="Ibook"
      footer-tag="h3"
    >
    </b-card>
    <b-card
      img-src="@/assets/images/des1.png"
      class="overflow-hidden center text-center"
      footer="Desafio Física"
      footer-tag="h3"
    >
    </b-card>
    <b-card
      img-src="@/assets/images/vel1.png"
      class="overflow-hidden text-center"
      footer="Velasquez Winery"
      footer-tag="h3"
    >
    </b-card>
    <b-card
      img-src="@/assets/images/faq1.png"
      class="overflow-hidden text-center"
      footer="FAQ Cataline"
      footer-tag="h3"
    >
    </b-card>
  </div>
</template>

<style lang="scss" scoped>
.samples {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(400px, 1fr));
  grid-auto-rows: auto;
  gap: 3em;
}
</style>
