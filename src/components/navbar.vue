<template>
  <div class="main-container">
    <div id="nav">
        <router-link to="/"><img src="../assets/logo.png" alt="kl-logo"></router-link>
        
        <div class="page-btns">
        <router-link class="link" to="/about">Our History</router-link>
        <router-link class="link" to="/contact">Contact Us</router-link>
        </div>
        
    </div>
  </div>
</template>

<script>
export default {

}
</script>

<style scoped>

.main-container {
    background-color: rgba(255, 255, 255, 0.65);
    width: 100%;
    position: fixed;
}

#nav {
    display: flex;
    justify-content: space-between;
    align-items: center;
    max-width: 1200px;
    margin: 0 auto;
    padding: 7px 50px;
}

img {
    height: 50px;
}

.page-btns > * {
    margin: 0 10px;
    text-decoration: none;
    color: black;
}

.link.router-link-active {
    color: rgb(254, 139, 38);
}

</style>