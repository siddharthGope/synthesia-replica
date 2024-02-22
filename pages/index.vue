<template>
  <div>
    <AppBar />
    <header class="page-padding">
      <div class="heading-caption">#1 AI VIDEO CREATION PLATFORM</div>
      <h1 class="heading">Create professional videos in 15 minutes</h1>
      <div class="header-desc">
        Create studio-quality videos with AI avatars and voiceovers in 130+
        languages. It’s as easy as making a slide deck.
      </div>
      <div class="d-flex header-buttons">
        <button class="blue-button">Create account</button>
        <button class="white-button">Book a demo</button>
      </div>
      <div class="header-image-wrap">
        <img src="@/assets/img/homepage-image1.gif" class="homepage-image1" />
      </div>
    </header>
  </div>
</template>

<style scoped lang="css">
.page-padding {
  padding-left: 2.5rem;
  padding-right: 2.5rem;
}
.heading {
  letter-spacing: -0.025rem;
  font-family: "Poppins", sans-serif;
  font-size: 2.5rem;
  font-weight: 500;
  line-height: 3rem;
}
.heading-caption {
  letter-spacing: 0.0525rem;
  text-transform: uppercase;
  font-family: "Poppins", sans-serif;
  font-size: 0.875rem;
  font-weight: 500;
  line-height: 1.25rem;
  color: #084df2;
}
.header-desc {
  margin-bottom: 1rem;
  font-family: "Poppins", sans-serif;
  font-size: 1.125rem;
  font-weight: 400;
  line-height: 1.625rem;
}
.homepage-image1 {
  width: 100%;
}
</style>
