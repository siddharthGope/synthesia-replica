<template>
  <div class="trusted">Trusted by over 50,000 companies of all sizes</div>
  <div class="carousel-wrap">
    <div class="carousel-images-wrap">
      <template v-for="images in carouselImages" :key="i">
        <img :src="images.imgSource" class="carousel-images" />
      </template>
    </div>
    <div class="carousel-images-wrap">
      <template v-for="images in carouselImages" :key="i">
        <img :src="images.imgSource" class="carousel-images" />
      </template>
    </div>
  </div>
  <div class="divider"></div>
</template>
<script>
export default {
  data: () => ({
    carouselImages: [
      {
        imgSource: "/images/CI-TIC.png",
      },
      {
        imgSource: "/images/Microsoft-Startups.png",
      },
      {
        imgSource: "/images/Startup-India.png",
      },
      {
        imgSource: "/images/Startup-TN.png",
      },
      {
        imgSource: "/images/CI-TIC.png",
      },
      {
        imgSource: "/images/Microsoft-Startups.png",
      },
      {
        imgSource: "/images/Startup-India.png",
      },
      {
        imgSource: "/images/Startup-TN.png",
      },
      {
        imgSource: "/images/CI-TIC.png",
      },
      {
        imgSource: "/images/Microsoft-Startups.png",
      },
    ],
  }),
};
</script>
<style lang="css">
.carousel-wrap {
  margin: 1rem 0 5rem;
  display: flex;
  width: 100%;
  mask-image: linear-gradient(
    90deg,
    transparent 5%,
    rgba(0, 0, 0, 1) 10%,
    rgba(0, 0, 0, 1) 90%,
    transparent 95%
  );
}
.carousel-images-wrap {
  display: flex;
  align-items: center;
  animation: logoloop 90s linear infinite;
}
.carousel-images {
  height: 50px;
  margin-left: 2rem;
  margin-right: 2rem;
}
.trusted {
  text-align: center;
  margin: 2rem 0;
  font-family: "Poppins", sans-serif;
  font-size: 1rem;
  font-weight: 400;
  line-height: 1.5rem;
}
.divider {
  width: 100%;
  height: 1px;
  border-bottom: 1px solid #e9ecf6;
  background-color: #e9ecf6;
  color: #e9ecf6;
  align-self: stretch;
  margin: 1rem 0 1rem;
}
@keyframes logoloop {
  0% {
    transform: translateX(0%);
  }
  100% {
    transform: translateX(-100%);
  }
}
</style>
