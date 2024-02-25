<
<template>
  <div>
    <div class="caption">THE ROI FOR YOUR BUSINESS</div>
    <div class="heading">
      You don't have to choose between cost, time, and quality
    </div>

    <v-row class="all-cards-wrap">
      <v-col v-for="i in 3" :key="i" cols="4">
        <div class="cards">
          <img src="/images/xerox.svg" class="cardImage" />
          <div class="line-break-small"></div>
          <div class="line1">Cost savings</div>
          <div class="line2">+50%</div>
          <div class="line3">
            Xerox's global training team
            <strong>reduced video and voiceover costs by over 50%</strong>,
            compared to hiring voiceover artists in multiple languages.
          </div>
          <div class="line4">Read case study</div>
        </div>
      </v-col>
    </v-row>
  </div>
</template>
<script>
export default {};
</script>
<style scoped lang="css">
.caption {
  letter-spacing: 0.0525rem;
  text-transform: uppercase;
  font-family: "Poppins", sans-serif;
  font-size: 0.875rem;
  font-weight: 500;
  line-height: 1.25rem;
  color: #084df2;
  text-align: center;
}
.heading {
  font-family: "Poppins", sans-serif;
  font-weight: 500;
  letter-spacing: -0.02rem;
  font-size: 2rem;
  line-height: 2.625rem;
  text-align: center;
  margin-bottom: 3rem;
}
.cards {
  width: 100%;
  border: 1px solid #d0d7e7;
  background-color: #f5f7fe;
  border-radius: 1rem;
  flex-direction: column;
  justify-content: space-between;
  align-self: stretch;
  padding: 2.5rem 2.5rem 2rem;
  transition: box-shadow 0.2s;
  display: flex;
  align-items: flex-start;
  position: relative;
  font-family: "Poppins", sans-serif;
}
.cards:hover {
  box-shadow: 4px 0 20px rgba(0, 0, 0, 0.08);
}
.cardImage {
  height: 30px;
  margin-bottom: 1.5rem;
}
.line-break-small {
  width: 100%;
  height: 1px;
  background-color: #e4e6ed;
  margin-bottom: 1.5rem;
}
.line1 {
  font-family: "Poppins", sans-serif;
  font-size: 1rem;
  font-weight: 400;
  line-height: 1.5rem;
  font-weight: 500;
}
.line2 {
  letter-spacing: -0.03rem;
  font-family: "Poppins", sans-serif;
  font-size: 3rem;
  font-weight: 500;
  line-height: 3.5rem;
  color: #002577;
  margin-bottom: 1.5rem;
}
.line4 {
  grid-column-gap: 0.5rem;
  grid-row-gap: 0.5rem;
  color: #084df2;
  text-align: center;
  flex-wrap: nowrap;
  align-items: center;
  margin-left: -0.25rem;
  margin-right: -0.25rem;
  padding-left: 0.25rem;
  padding-right: 0.25rem;
  padding-top: 3.5rem;
  font-family: "Poppins", sans-serif;
  font-size: 1rem;
  font-weight: 500;
  line-height: 1.5rem;
  transition: all 0.2s;
  display: flex;
}
</style>
