<template>
  <div id="displayvideo">
    <video width="320" height="240" controls>
      <source
        src="https://synthesia-results.s3.eu-west-1.amazonaws.com/website_demos/Features-short-demos/avatars.mp4"
        type="video/mp4"
      />
    </video>
  </div>
  <!-- <Tippy content="HI">
    <button>Tippy!</button>
  </Tippy> -->

  <!-- <Tippy
    content="{
      html: '#displayvideo',
    }"
  >
    Static HTML Template
  </Tippy> -->
</template>

<script setup>
// import { Tippy } from "vue-tippy";
// import vTippy from "vue-tippy";
</script>

<style lang="css">
#displayvideo {
  margin-bottom: 200px;
}
</style>
