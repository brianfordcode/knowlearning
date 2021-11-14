<template>

<div class="container">
  
  <homeBanner/>


  <div class="mission-container">
    <p class="title">Our Mission</p>
    <p class="text">Know Learning is committed to supporting an international group of partners and open-source contributors in building digital learning experiences that are more engaging, interactive, joyous, measurably effective, and freely available.</p>
  </div>

  <iconBanner/>

</div>
  

  





</template>

<script>
import homeBanner from "../components/home-banner.vue"
import iconBanner from "../components/icon-banner.vue"

export default {
  name: 'Home',
  components: { homeBanner, iconBanner }
}
</script>

<style scoped>

.container {
  margin: 0 auto;
  max-width: 1200px;
}

.mission-container {
  display: flex;
  flex-direction: column;
  align-items: center;
  margin-top: 130px;
}

.title {
  font-size: 36px;
  padding-bottom: 20px
}

.text {
  max-width: 700px;
  text-align: center;
  font-size: 20px;
  padding: 0 50px 0 50px;
}

</style>
