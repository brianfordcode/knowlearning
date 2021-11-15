<template>

    <footer>
        <div class="wrapper">
            <div class="links">
                <router-link to="/login">Log In</router-link>
                <p>Icons made by <a href="https://www.freepik.com" title="Freepik">Freepik</a> from <a href="https://www.flaticon.com/" title="Flaticon">www.flaticon.com</a></p>
            </div>
            <div class="kl-wrapper">
                <img draggable="false" src="../assets/logo.png" alt="">
                <p>2021 KnowLearning</p>
            </div>
        
        </div>
        
    </footer>
  
</template>

<script>

export default {}
</script>

<style scoped>

footer {
    background: rgb(254, 139, 38);
    padding: 10px 30px 10px 30px;
}

.wrapper {
    max-width: 1200px;
    display: flex;
    justify-content: space-between;
    align-items: center;
    margin: 0 auto;
}

.links {
    display: flex;
    flex-direction: column;
}

.links p {
    font-size: 6px;
}

.kl-wrapper {
    display: flex;
    align-items: center;
}
img {
    height: 40px;
    margin-right: 10px;
}

</style>