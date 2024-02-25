<template>
  <div>
    <div class="avatar-demo-container">
      <div class="avatar-demo-grid">
        <div class="caption">AI AVATARS</div>
        <div class="features--heading">
          Create videos as diverse as your audience
        </div>
        <ul>
          <li>Engage your viewers with over 160 AI avatars</li>
          <li>Make your videos more inclusive and diverse</li>
          <li>Create your own AI avatar (your digital twin)</li>
        </ul>
        <div class="button-div">
          <button class="white-button">See all avatars</button>
        </div>
      </div>
      <div class="features-videos">
        <v-row>
          <v-col v-for="i in 6" :key="i" cols="4">
            <div class="avatar-wrapper">
              <img src="/images/features-avtars.png" class="features-avtars" />
            </div>
          </v-col>
        </v-row>
      </div>
    </div>

    <div class="feature-wrap2 card-margin">
      <div class="avatar-demo-container2">
        <div class="features-videos">
          <div class="avatar-wrapper">
            <img src="/images/features-image2.png" class="features-avtar2" />
          </div>
        </div>
        <div class="avatar-demo-grid">
          <div class="caption">AI VOICEOVERS</div>
          <div class="features--heading">
            Turn text into high-quality voiceovers with one click
          </div>
          <ul>
            <li>Get consistent voiceovers in over 130 languages</li>
            <li>Automatically generate closed captions</li>
            <li>Clone your own voice</li>
          </ul>
          <div class="button-div">
            <button class="white-button">Test all languages</button>
          </div>
        </div>
      </div>
    </div>
    <div class="avatar-demo-container2">
      <div class="avatar-demo-grid">
        <div class="caption">EASY UPDATES</div>
        <div class="features--heading">
          Keep your video library up to date without reshoots
        </div>
        <ul>
          <li>Prototype your video and share it with your team</li>
          <li>Get feedback and make edits in one place</li>
          <li>Update your videos with a click of a button</li>
        </ul>
        <div class="button-div">
          <button class="white-button">See all features</button>
        </div>
      </div>
      <div class="features-videos">
        <div class="avatar-wrapper">
          <img src="/images/features-image3.png" class="features-avtar2" />
        </div>
      </div>
    </div>
  </div>
</template>
<script>
export default {};
</script>
<style scoped lang="css">
.avatar-demo-container {
  background-color: #fff;
  border-radius: 1rem;
  padding: 2rem 2.5rem;
  display: grid;
  grid-template-columns: repeat(2, 1fr);
  grid-template-rows: 1fr;
  grid-column-gap: 0px;
  grid-row-gap: 0px;
  align-items: center;
}
li::marker {
  color: #084df2;
}
.avatar-demo-grid li {
  color: #2c374f;
  font-family: "Poppins", sans-serif;
  font-size: 1rem;
  font-weight: 400;
  line-height: 1.5rem;
  margin-bottom: 1.5rem !important;
  margin-left: 10px;
}
.features-avtars {
  height: 10rem;
  border-radius: 11.3315px;
}
.avatar-wrapper {
  border-radius: 0.625rem;
  padding: 0.47rem;
  box-shadow: 0px 0.586811px 2.34724px rgba(15, 20, 30, 0.06);
}

.features--heading {
  margin: 1rem 0 2rem;
}
.white-button {
  margin-top: 3rem;
}
.features-avtar2 {
  height: 200px;
  border-radius: 11.3315px;
}
.avatar-demo-container2 {
  display: grid;
  grid-template-columns: repeat(2, 1fr);
  grid-template-rows: 1fr;
  grid-column-gap: 0px;
  grid-row-gap: 0px;
  align-items: center;
  justify-items: center;
  background-color: #fff;
  border-radius: 1rem;
  padding: 2rem 2.5rem;
}
.card-margin {
  margin: 3rem 0;
}
</style>
