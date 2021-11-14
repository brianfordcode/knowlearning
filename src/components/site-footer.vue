<template>

    <footer>
        
        <div class="links">
            <router-link to="/login">Log In</router-link>
            <p>Icons made by <a href="https://www.freepik.com" title="Freepik">Freepik</a> from <a href="https://www.flaticon.com/" title="Flaticon">www.flaticon.com</a></p>
        </div>
        <p>2021 KnowLearning</p>
    </footer>
  
</template>

<script>

export default {}
</script>

<style scoped>

footer {
    background: rgb(254, 139, 38);
    padding: 15px 30px 15px 30px;
    bottom: 0;
    display: flex;
    justify-content: space-between;
    align-items: center;
}
.links {
    display: flex;
    flex-direction: column;
}

.links p {
    font-size: 6px;
}

</style>