<template>

  <div class="background">
    <navBar/>

    <router-view/>

    <siteFooter class="footer"/>


  </div>


</template>

<script>
import navBar from './components/navbar.vue'
import siteFooter from './components/site-footer.vue'

export default {
  components: { navBar, siteFooter }
}
</script>


<style>

* {
  margin: 0;
  padding: 0;
}

#app {
  font-family: 'Gill Sans', 'Gill Sans MT', Calibri, 'Trebuchet MS', sans-serif;
  min-height: 100vh;
  padding-bottom: 100px;
  height: 100vh;
}

.background::after { 
    content: "";
    width: 100%;
    height: 1000px;
    position: absolute;
    top: -500px;
    right: 0;
    /* left: 0; */
    background: rgb(254, 139, 38);
    transform: skewY(6deg);
    z-index: -10;
}

@media screen and (max-width: 768px) {
  .background::after {
    height: 900px;
  }
}

</style>
