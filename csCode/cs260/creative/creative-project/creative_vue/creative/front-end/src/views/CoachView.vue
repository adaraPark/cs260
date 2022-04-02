<template>
    <div class="coach">
    <div class="container">
        <div class="image">
          <img src="../assets/images/screenshots/pexels-photo-4577209.jpg" style="float: left;">
        </div>
        <div class="text"> 
          <h2>Becoming A Coach</h2> 
          <div class="aboutMeDef"  style="float: right;"><p>
          Becoming A coach is simple, all you do is create an account, fill you profile with your accomplishments, and post your
           availability. Younger aspiring athletes then have the chance to be coached by you online.
          </p></div>
        </div>
      </div>
      <hr>

      <div class="container">
        <div class="image"><img src="../assets/images/screenshots/baseball-coach.jpeg" style="float: right;"></div>
        <div class="text">
          <h2>Steps to Finishing Your Account</h2>
          <div class="steps"  style="float: left;">
            <ul>
              <li>Create an Introduction Video for athletes to get to know you</li>
              <li>List your qualifications and athletic accomplishments</li>
              <li>Fill out your Bio with Video film of either you coaching or competiting</li>
              <li>Post you availability and pricing</li>
            </ul>
          </div>
        </div>
      </div>
      <hr>

      <div class="jumbotron" style="margin: 80px;text-align: center;">
        <h1 class="display-4">Teach athletes what you know and make money doing it!</h1>
        <!-- <p class="lead">Be able to connect with your collegiate idols and hear their story! <br> let them teach you all that they know</p> -->
        <hr class="my-4">
        <p>Click to create your own class</p>
        <router-link class="btn btn-primary btn-lg" to="/createclass"> Create </router-link>
    </div>
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
