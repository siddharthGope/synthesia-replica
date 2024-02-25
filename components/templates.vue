<template>
  <div>
    <div class="template-header">
      <div>
        <div class="caption-1">TEMPLATES</div>
        <h2 class="heading-style-h1">
          Get started in minutes with 200+ free video templates
        </h2>
      </div>
      <div class="button-wrap">
        <button class="white-button">See all templates</button>
      </div>
    </div>
    <v-row class="all-templates">
      <v-col v-for="i in 6" :key="i" cols="4">
        <img src="/images/template-image.png" class="template-image" />
      </v-col>
    </v-row>
  </div>
</template>
<script>
export default {};
</script>
<style scoped lang="css">
.template-header {
  display: flex;
  grid-column-gap: 1.5rem;
  grid-row-gap: 1.5rem;
  justify-content: space-between;
  align-items: center;
  color: #fff;
  margin-bottom: 3rem ;
}
.template-image {
  height: 200px;
}
.heading-style-h1 {
  letter-spacing: -0.02rem;
  font-size: 2rem;
  line-height: 2.625rem;
  font-family: "Poppins", sans-serif;
  font-weight: 500;
}
.caption-1 {
  letter-spacing: 0.0525rem;
  text-transform: uppercase;
  font-family: "Poppins", sans-serif;
  font-size: 0.875rem;
  font-weight: 500;
  line-height: 1.25rem;
}
.all-templates {
    align-items: center;
    justify-content: center;
}
</style>
