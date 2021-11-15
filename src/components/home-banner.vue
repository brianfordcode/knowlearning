<template>

    <div class="container">
        <div class="text-btn-wrapper">
            <p>A <span>Non-Profit</span> project dedicated
            <br> 
            to a new generation of <span>Digital
            <br> 
            Learning Experiences</span>.
            </p>
          
            <router-link to="/contact">
                <button>Get in touch<br>for a demo!</button>
            </router-link>
        </div>

        <div class="circle">
          <img src="../assets/pic.jpg" alt="main-pic">
        </div>

    </div>
  
</template>

<script>

export default {
  name: 'Home',
  components: {
  }
}
</script>

<style scoped>

  .container {
    display: flex;
    justify-content: space-around;
    align-items: center;
    padding-top: 50px;
    /* border: 1px solid black; */
  }

  .text-btn-wrapper {
    display: flex;
    flex-direction: column;
    justify-content: space-between;
    align-items: center;
    width: max-content;
    height: 225px;
    color: rgb(39, 39, 39);
    /* border: 1px solid black; */
  }

  p {
    font-size: 28px
  }

  p span {
    font-size: 36px;
  }

  button {
    padding: 12px 35px;
    border: none;
    background-color: rgb(231, 231, 231);
    color: black;
    cursor: pointer;
    border-radius: 10px;
    transition: .25s ease-in-out;
  }

  button:hover {
    transform: scale(1.05);
  }

  .circle {
    border-radius: 50%;
    overflow: hidden;
    display: inline-block;
    height: 300px;
    width: 300px;
  }

  img {
    height: 350px;
  }

  @media screen and (max-width: 768px) {

    .text-btn-wrapper {
        height: 200px;
    }

    p {
        text-align: center;
        font-size: 20px;
    }

    p span {
        font-size: 30px;
    }

    .circle {
        height: 250px;
        width: 250px;
    }
    img {
      height: 300px;
    }
  }
  @media screen and (max-width: 600px) {
      .circle {
          display: none;
      }
      .img {
          display: none;
      }
  }

</style>
