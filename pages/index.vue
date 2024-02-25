<template>
  <div>
    <AppBar />
    <header class="header-section page-padding">
      <div class="heading-caption">#1 AI VIDEO CREATION PLATFORM</div>
      <h1 class="heading">Turn text to video in minutes</h1>
      <div class="header-desc">
        Create studio-quality videos with AI avatars and voiceovers in 130+
        languages. It’s as easy as making a slide deck.
      </div>
      <div class="d-flex header-buttons">
        <button class="blue-button">Create a free AI video</button>
      </div>
      <div class="header-image-wrap">
        <img src="@/assets/img/homepage-image1.gif" class="homepage-image1" />
      </div>
    </header>
    <section class="carousel-section">
      <carousel />
    </section>
    <section class="tabs-section">
      <tabs />
    </section>
    <section class="virtical-section">
      <virticalTabs />
    </section>
    <section class="cards">
      <cards />
    </section>
    <section class="features">
      <features />
    </section>
    <section class="integration">
      <integration />
    </section>
    <section class="templates">
      <templates />
    </section>
  </div>
</template>

<style scoped lang="css">
.page-padding {
  padding-left: 2.5rem;
  padding-right: 2.5rem;
}
.header-section {
  display: flex;
  flex-direction: column;
  align-items: center;
}
.heading {
  letter-spacing: -0.025rem;
  font-family: "Poppins", sans-serif;
  font-size: 2.5rem;
  font-weight: 500;
  line-height: 3rem;
  text-align: center;
  margin-top: 0.7rem;
}
.heading-caption {
  letter-spacing: 0.0525rem;
  text-transform: uppercase;
  font-family: "Poppins", sans-serif;
  font-size: 0.875rem;
  font-weight: 500;
  line-height: 1.25rem;
  color: #084df2;
  text-align: center;
  margin-top: 3rem;
}
.header-desc {
  margin-bottom: 1rem;
  font-family: "Poppins", sans-serif;
  font-size: 1.125rem;
  font-weight: 400;
  line-height: 1.625rem;
  text-align: center;
  width: 600px;
  margin-top: 0.7rem;
}
.homepage-image1 {
  width: 100%;
  border-radius: 30px;
  filter: drop-shadow(0 0 0.75rem #01af89);
  margin: 1rem 0;
}
.blue-button {
  text-align: center;
  margin: 1.5rem 0 2rem;
}
section {
  padding: 6rem;
}
.features {
  background-color: #f5f7fe;
}
.templates {
  background-color: #2c374f;
}
.tabs-section {
  padding: 0 6rem 5rem;
}
</style>
