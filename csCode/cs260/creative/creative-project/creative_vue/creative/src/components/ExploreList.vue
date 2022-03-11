<template>
    <div class="wrapper">
        <div class="products">
            <div class="people" v-for="person in people" :key="person.id" >
                <div class="card">
                    <div class="image">
                        <img class="card-img-top" src="../assets/images/screenshots/runner.jpg" alt="Card image cap">
                                <!-- <img src="'person.image'" />  -->
                                <!-- <img :src="'../assets/images/screenshots/'+person.image">  need to fix this eventually-->
                    </div>
                    <div class="card-body">
                        <h5 class="card-title"><b>{{person.title}}</b></h5>
                        <p class="card-text">{{person.description}}</p>
                        <a href="#" class="btn btn-primary">See Info</a>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
  name: 'ExploreList',
  props: {
    people: Array
  }
}
</script>

<style scoped>
.wrapper {
  display: flex;
  align-items: center;
  justify-content: center;
}

.products {
  margin-top: 20px;
  display: flex;
  flex-wrap: wrap;
}

.people {
  margin: 10px;
  margin-top: 20px;
  width: 450px;
}


.card{
    width: 450px;
}

.card-title{
    justify-content: center;
    text-align: center;
}

.card-body {
    width: 450px;
    height: 250px;
}

.people img {
  border: 2px solid #333;
  height: 300px;
  width: 425px;
  object-fit: cover;
}

.people .image {
  display: flex;
  justify-content: center;
  margin-bottom: 5px;
}
</style>