<template>
  <div class="caption">USE CASES</div>
  <div class="features--heading">
    For teams who create training videos at scale
  </div>
  <v-tabs
    v-model="tab"
    color="#084df2"
    slider-color="#084df2"
    align-tabs="center"
    class="tabs-wrap"
  >
    <v-tab
      class="each-tab"
      prepend-icon="mdi-message-text"
      hide-slider
      :value="1"
      >Learning & Development</v-tab
    >
    <v-tab
      class="each-tab tab-margin"
      prepend-icon="mdi-message-text"
      hide-slider
      :value="2"
    >
      Sales Enablement</v-tab
    >
    <v-tab
      class="each-tab"
      prepend-icon="mdi-message-text"
      hide-slider
      :value="3"
      >Customer Service</v-tab
    >
  </v-tabs>
  <v-window v-model="tab">
    <v-window-item v-for="n in 3" :key="n" :value="n">
      <v-container fluid>
        <v-row class="all-tabs-content-wrap">
          <v-col cols="6" class="tabs-content-left-wrap">
            <div class="tab-desc-heading">
              Create high-quality sales enablement videos your team won't skip
            </div>
            <div class="tab-desc-text">
              "Sales people require engaging training content. With Synthesia's
              AI avatars and voiceovers, we can now facilitate quicker knowledge
              transfer."
            </div>
            <div class="caption-2">JASON E.</div>
            <div class="label-regular">
              Global L&D Sales Training Strategy Manager at Xerox
            </div>
            <button class="white-button">Learn more</button>
          </v-col>
          <v-col cols="6" class="tabs-images-wrap">
            <img src="/images/tabs-images.png" class="tabs-images" />
          </v-col>
        </v-row>
      </v-container>
    </v-window-item>
  </v-window>
</template>
<script>
export default {
  data: () => ({
    tab: null,
  }),
};
</script>
<!-- background-color: #e8f0ff; -->
<style scoped lang="css">
.each-tab {
  border-radius: 0.5rem !important;
  text-transform: capitalize;
  font-family: "Poppins", sans-serif;
  font-weight: 500;
  font-size: 16.33px;
}
.tab-desc-heading {
  font-family: "Poppins", sans-serif;
  font-weight: 500;
  letter-spacing: -0.015rem;
  font-size: 1.5rem;
  line-height: 2rem;
}
.tab-desc-text {
  font-family: "Poppins", sans-serif;
  font-size: 1.125rem;
  font-weight: 400;
  line-height: 1.625rem;
  margin: 2rem 0;
}
.caption-2 {
  letter-spacing: 0.045rem;
  text-transform: uppercase;
  font-family: "Poppins", sans-serif;
  font-size: 0.75rem;
  font-weight: 500;
  line-height: 1.125rem;
}
.label-regular {
  font-family: "Poppins", sans-serif;
  font-size: 0.75rem;
  font-weight: 400;
  line-height: 1.125rem;
}
.tabs-wrap {
  padding: 0.25rem;
  border-radius: 0.75rem;
  border: 1px solid #e9ecf6;
  height: 59px;
  width: 70%;
  margin: 0 auto;
}
.tab-margin {
  margin: 0 2rem;
}
.all-tabs-content-wrap {
  margin-top: 2rem;
}
.v-slide-group-item--active {
  background: #e8f0ff;
}
.tabs-images-wrap {
  box-shadow: 0 -6px 20px rgba(11, 18, 32, 0.12);
  border: 1px solid rgba(245, 247, 254, 0.2);
  padding: 0.5rem;
  border-radius: 1rem;
  backdrop-filter: blur(0.25rem);
  background-color: rgba(255, 255, 255, 0.3);
}
.tabs-images {
  border: 1px solid #f5f7fe;
  border-radius: 0.5rem;
}
.white-button {
  margin-top: 2rem;
}
.tab-desc-heading,
.tab-desc-text {
  margin-right: 2rem;
}
.features--heading,
.caption {
  text-align: center;
}
.features--heading {
  margin-bottom: 3rem;
}
</style>
