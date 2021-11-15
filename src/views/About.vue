<template>
<div class="container">
    <div class="history wrapper">
        <p class="title">Our History</p>
        <p>Lorem, ipsum dolor sit amet consectetur adipisicing elit. Veritatis, odit nobis suscipit quibusdam nam explicabo ut, perferendis saepe dolor facere consequatur magni doloremque? Ullam nam odio molestiae in nisi quidem magnam aspernatur. Aut laborum atque dolores soluta illum similique officia tempora minus totam voluptatem nostrum voluptas rerum quibusdam vel, excepturi, repellat magni alias impedit magnam itaque deleniti distinctio culpa. Facere explicabo repellendus autem eveniet enim corporis assumenda quia accusantium totam numquam eum labore fugiat qui nobis nesciunt porro in nulla nostrum, sunt natus expedita beatae! Aspernatur assumenda mollitia suscipit omnis inventore eligendi non, sapiente corporis a consequuntur accusantium architecto! Illum?</p>
    </div>
    <div class="founders wrapper">
        <p class="title">About the Founders</p>
        <div class="founder-info first">
          <img src="https://picsum.photos/150/150" alt="founder-pic">
          <div class="founder-text">
              <p class="founder-name">Jason Ford</p>
              <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Voluptatem, necessitatibus et commodi, voluptatum, cumque consequuntur reiciendis ipsa nihil praesentium consectetur corrupti reprehenderit maiores possimus iure. Amet quod, laborum tempore esse dicta accusantium similique at illum non, quos incidunt temporibus molestiae modi, veritatis porro excepturi perspiciatis repellat est laudantium velit placeat!</p>
          </div>
        </div>
        <div class="founder-info second">
          <img src="https://picsum.photos/150/150" alt="founder-pic">
          <div class="founder-text">
              <p class="founder-name">Matt McClain</p>
              <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Voluptatem, necessitatibus et commodi, voluptatum, cumque consequuntur reiciendis ipsa nihil praesentium consectetur corrupti reprehenderit maiores possimus iure. Amet quod, laborum tempore esse dicta accusantium similique at illum non, quos incidunt temporibus molestiae modi, veritatis porro excepturi perspiciatis repellat est laudantium velit placeat!</p>
          </div>
        </div>
    </div>
</div>
  
</template>

<script>
export default {

}
</script>

<style scoped>

.container {
  margin: 0 auto;
  max-width: 800px;
  text-align: center;
  padding: 75px 50px 0 50px;
}

.history {
  margin-bottom: 200px;
}

.founders {
  margin-bottom: 50px;
}

.title {
  font-size: 36px;
  padding-bottom: 20px;
}

.first {
  display: flex;
  text-align: left;
  max-width: 700px;
  margin: 0 auto 30px auto;
}

.founder-name {
  font-size: 22px;
  padding-bottom: 10px;
}

.first p {
  margin-left: 20px;
}

.second {
  display: flex;
  flex-direction: row-reverse;
  text-align: right;
  max-width: 700px;
  margin: 0 auto;
}

.second p {
  margin-right: 20px;
}

img {
  border-radius: 5%;
}

@media screen and (max-width: 768px) {
  .history {
    margin-bottom: 50px;
  }

  .founder-info {
    display: flex;
    flex-direction: column;
    align-items: center;
    text-align: center;
  }

.first p {
  margin-left: 0px;
}

.second p {
  margin-right: 0px;
}

  img {
    height: 150px;
    width: 150px;
    margin-bottom: 20px;
  }
}

</style>