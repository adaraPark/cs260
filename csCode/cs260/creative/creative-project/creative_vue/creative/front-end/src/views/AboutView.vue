<template>
  <div class="about">
       <div class="container">
      <div class="image">
        <img src="../assets/images/screenshots/pexels-photo-9944009.jpg" style="float: left;">
      </div>
      <div class="text"> 
        <h2>About AthleteUp</h2> 
        <div class="aboutMeDef"  style="float: right;"><p>
          We are an organization determined to help athletes reach their dreams, by providing a way to <br> access collegiate athletes, 
          professional athletes, and coaches from around the world. <br><br>
          Aspiring athletes can come and learn from the best in their field in 1-on-1 training sessions <br> online. No matter the distance between, 
          you can recieve training and advice from the best!
        </p></div>
      </div>
    </div>
    <hr>
  </div>
</template>

<style scoped>
      .container {
    display: flex;
    align-items: center;
    justify-content: center;
    padding-top: 20px;
    padding-bottom: 40px;
  }
  img {
    max-width: 100%;
  }
  .image {
    flex-basis: 50%;
  }
  .text {
    padding-left: 20px;
    padding-right: 20px;
  }

.aboutMeDef {
  padding-left: 20px;
  font-size: 30px;
}

.steps {
  padding-right: 20px;
  font-size: 30px;
}
</style>
