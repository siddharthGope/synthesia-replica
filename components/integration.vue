<template>
  <div>
    <div class="avatar-demo-container">
      <div class="avatar-demo-grid">
        <div class="caption">INTEGRATIONS</div>
        <div class="features--heading">
          Embed your videos into your favorite tools
        </div>
      </div>
      <div class="features-videos">
        <div class="paragraph-2">
          Streamline your video creation process by embedding your videos into
          your authoring tool, LMS, LXP, and more.
        </div>
        <div class="button-div">
          <button class="caption">Explore all integrations</button>
        </div>
      </div>
    </div>
    <carousel />
    <div class="avatar-demo-container2">
      <div class="features-videos">
        <div class="avatar-wrapper">
          <img src="/images/integration-image1.png" class="features-avtar2" />
        </div>
      </div>
      <div class="avatar-demo-grid">
        <div class="">
          <img src="/images/Heineken_logo.svg" class="Heineken_logo" />
        </div>
        <div class="Heineken_logo--heading">
          “If you’re considering to try Synthesia,
          <span> don’t get ready. Get started.”</span>
        </div>
        <div class="divider"></div>
        <div class="paragraph-3">Frank C. Van der Grijspaarde</div>
        <div class="paragraph-4">
          Global TPM Manager, CS&L and Planning, Heineken
        </div>
      </div>
    </div>
    <!-- ________________________________________________________________________ -->
    <div class="grid-card-medium">
      <div class="avatar-demo-grid">
        <div class="caption">AI SAFETY</div>
        <div class="features--heading">
          Built on the foundations of ethics and security
        </div>
        <div class="paragraph-2">
          People first, always. We prioritize secure, safe and ethical use of
          Artificial Intelligence in our product development processes.
        </div>
        <div class="button-div">
          <button class="caption">Learn more</button>
        </div>
      </div>
      <div class="features-videos">
        <div class="card-medium-container">
          <v-row>
            <v-col v-for="n in 4" :key="n" cols="6">
              <div class="card-medium-container-heading">
                SOC 2 & GDPR compliant
              </div>
              <div class="card-medium-container-text">
                Our data handling practices, systems, and processes have been
                independently audited and certified.
              </div>
            </v-col>
          </v-row>
        </div>
      </div>
    </div>
    <div class="logos-wrap">
      <img v-for="n in 6" :key="n" src="/images/BBC.svg" class="bbc-logo" />
    </div>
  </div>
</template>
<script>
export default {};
</script>
<style scoped lang="css">
.avatar-demo-container {
  grid-column-gap: 4.5rem;
  grid-row-gap: 1rem;
  margin-bottom: 4.5rem;
  display: flex;
}
.button-div {
  margin-top: 1.7rem;
}
.paragraph-2 {
  font-family: "Poppins", sans-serif;
  font-size: 1.125rem;
  font-weight: 400;
  line-height: 1.625rem;
  margin: 2rem 0;
}
.avatar-demo-container2 {
  display: grid;
  grid-template-columns: repeat(2, 1fr);
  grid-template-rows: 1fr;
  grid-column-gap: 74px;
  grid-row-gap: 0px;
  align-items: center;
  justify-items: center;
  background-color: #fff;
  border-radius: 1rem;
  padding: 2rem 2.5rem;
  margin: 5rem 0 10rem;
}
.features-avtar2 {
  height: 300px;
  border-radius: 11.3315px;
}
.avatar-wrapper {
  border-radius: 0.625rem;
  padding: 0.47rem;
  box-shadow: 0px 0.586811px 2.34724px rgba(15, 20, 30, 0.06);
}
.Heineken_logo {
  height: 40px;
}
.Heineken_logo--heading {
  font-family: "Poppins", sans-serif;
  font-size: 1.125rem;
  font-weight: 400;
  line-height: 1.625rem;
}
.paragraph-3 {
  font-family: "Poppins", sans-serif;
  font-size: 1.125rem;
  font-weight: 500;
  line-height: 1.625rem;
}
.Heineken_logo--heading {
  letter-spacing: -0.02rem;
  font-size: 2rem;
  line-height: 2.625rem;
  font-family: "Poppins", sans-serif;
  font-weight: 500;
  margin: 2rem 0;
}
.Heineken_logo--heading span {
  background-image: linear-gradient(91deg, #002577, #084df2 1%, #002577 67%);
  background-clip: text;
}

.paragraph-4 {
  font-family: "Poppins", sans-serif;
  font-size: 1rem;
  font-weight: 400;
  line-height: 1.5rem;
  color: #6e778c;
}
.divider {
  width: 100%;
  height: 1px;
  border-bottom: 1px solid #e9ecf6;
  background-color: #e9ecf6;
  color: #e9ecf6;
  align-self: stretch;
  margin: 1rem 0;
}
.card-medium-container {
  border: 1px solid #e9ecf6;
  background-color: #f5f7fe;
  border-radius: 0.5rem;
  align-items: start;
  padding: 2.5rem;
}
.card-medium-container-heading {
  font-family: "Poppins", sans-serif;
  font-size: 1rem;
  font-weight: 500;
  line-height: 1.5rem;
}
.card-medium-container-text {
  font-family: "Poppins", sans-serif;
  font-size: 0.875rem;
  font-weight: 400;
  line-height: 1.375rem;
}
.grid-card-medium {
  grid-column-gap: 5rem;
  grid-row-gap: 2rem;
  grid-template-rows: auto;
  grid-template-columns: 1fr 1.75fr;
  grid-auto-columns: 1fr;
  display: grid;
  margin-top: 6rem;
}
.card-medium-container-heading,
.card-medium-container-text {
  width: 300px;
}
.logos-wrap {
  display: flex;
  justify-content: space-between;
  margin-top: 6rem;
}
.bbc-logo {
  height: 40px;
}
</style>
