<template>


    <div class="container">
        <div class="cust-container module">
            <img draggable="false" src="../assets/customize.png" alt="customize-icon">
            <p>Our architecture allows for development and adaptation of open-source learning experiences that are customizable and remixable.</p>
        </div>
        <div class="cust-container module">
            <img draggable="false" src="../assets/module.png" alt="customize-icon">
            <p>Educators from any background can organize experiences into custom modules, or find and use modules contributed by others.</p>
        </div>
        <div class="cust-container module">
            <img draggable="false" src="../assets/track.png" alt="customize-icon">
            <p>Educators can assign and track progress on customized content modules for their learners.</p>
        </div>
        <div class="cust-container module">
            <img draggable="false" src="../assets/pipeline.png" alt="customize-icon">
            <p>KnowLearning provides a simple but flexible data pipeline for reporting and analysis.</p>
        </div>
    </div>
  
</template>

<script>
export default {

}
</script>

<style scoped>

.container {
    display: flex;
    align-items: flex-start;
    justify-content: space-around;
    padding: 100px 30px 100px 30px;
}

.module {
    width: 250px;
    display: flex;
    flex-direction: column;
    align-items: center;
    text-align: center;
    margin: 0 20px 0 20px;
}

img {
    margin-bottom: 15px;
    width: 100px;
}

@media screen and (max-width: 850px) {
    .container {
        flex-wrap: wrap;
        padding-top: 50px;
        align-items: center;
    }

    .module {
        margin: 40px 0 0 0;
    };
}

</style>