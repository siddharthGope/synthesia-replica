<template>
  
    <div class="d-flex flex-row">
      <v-tabs
        color="#084df2"
        slider-color="#084df2"
        v-model="tab"
        direction="vertical"
        class="tabs-wrap"
      >
        <v-tab class="each-tab" hide-slider value="option-1">
          <v-icon start> mdi-account </v-icon>
          <div class="tab-texts-wrap">
            <div class="tab-desc-heading">Create your script</div>
            <div class="tab-desc-desc">
              Work better, together by sharing your video with your team to get
              feedback.
            </div>
          </div>
        </v-tab>
        <v-tab class="each-tab" hide-slider value="option-2">
          <v-icon start> mdi-lock </v-icon>
          <div class="tab-texts-wrap">
            <div class="tab-desc-heading">Customize your video</div>
            <div class="tab-desc-desc">
              Work better, together by sharing your video with your team to get
              feedback.
            </div>
          </div>
        </v-tab>
        <v-tab class="each-tab" hide-slider value="option-3">
          <v-icon start> mdi-access-point </v-icon>
          <div class="tab-texts-wrap">
            <div class="tab-desc-heading">Collaborate</div>
            <div class="tab-desc-desc">
              Work better, together by sharing your video with your team to get
              feedback.
            </div>
          </div>
        </v-tab>
      </v-tabs>
      <v-window v-model="tab">
        <v-window-item value="option-1">
          <div class="vertical-tabs-img-wrap" flat>
            <img src="/images/vertical-tabs.png" class="vertical-tabs-img" />
          </div>
          >
        </v-window-item>
        <v-window-item value="option-2">
          <div class="vertical-tabs-img-wrap" flat>
            <img src="/images/vertical-tabs.png" class="vertical-tabs-img" />
          </div>
        </v-window-item>
        <v-window-item value="option-3">
            <div class="vertical-tabs-img-wrap" flat>
            <img src="/images/vertical-tabs.png" class="vertical-tabs-img" />
          </div>
        </v-window-item>
      </v-window>
    </div>
</template>
<script>
export default {
  data: () => ({
    tab: "option-1",
  }),
};
</script>
<style scoped>
.vertical-tabs-img {
  height: 400px;
}
.vertical-tabs-img-wrap {
  margin-left: 5rem;
  box-shadow: 0 -6px 20px rgba(11, 18, 32, 0.12);
  border-radius: 1rem;
  padding: 0.5rem;
  backdrop-filter: blur(0.25rem);
  background-color: rgba(255, 255, 255, 0.3);
  border: 1px solid rgba(245, 247, 254, 0.2);
}
.v-slide-group-item--active {
  background: #084df2;
}
.each-tab {
  border-radius: 0.5rem !important;
  text-transform: capitalize;
  border-radius: 0.75rem;
  height: 10rem !important;
  width: 24rem;
}
.tab-texts-wrap {
  display: flex;
  flex-direction: column;
  align-items: flex-start;
}
.tab-desc-heading {
  font-family: "Poppins", sans-serif;
  font-weight: 500;
  white-space: normal;
  font-size: 1.25rem;
  line-height: 2rem;
  color: #6e778c;
}
.tab-desc-desc {
  font-size: 0.875rem;
  font-family: "Poppins", sans-serif;
  font-weight: 400;
}
.v-slide-group-item--active .tab-desc-heading {
  color: #fff;
}
.v-slide-group-item--active .tab-desc-desc {
  color: #fff;
}
.v-slide-group-item--active i {
  color: #fff;
}
</style>
