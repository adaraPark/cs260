<template>
    <div class='explore'>
        <div class="jumbotron jumbotron-fluid navbar-dark bg-dark" style="margin: 40px; color: white; text-align: center; height: 350px;">
          <div class="container">
            <h1 class="display-4">Coaches Explore Page</h1>
            <p class="lead">Find the Perfect coach for you!</p>

            <div class="lead search form-inline justify-content-center align-self-center">
              <form class="pure-form">
                  <i class="fas fa-search"></i><input class="form-control mr-sm-2"  type="search" placeholder="Search by Sport" aria-label="Search" v-model="searchText" />
                   <button class="btn btn-outline-success my-2 my-sm-0" type="submit">Search</button>
               </form>
            </div>
          </div>
        </div>
       <ExploreList :people="people" />
      <hr>

    </div>
</template>

<script>
import ExploreList from "../components/ExploreList.vue"
export default {
  name: 'ExploreView',
  components: {
    ExploreList
  },
  data() {
    return {
      searchText: '',
    }
  },
  computed: {
    people() {
      return this.$root.$data.people.filter(people => people.title.toLowerCase().search(this.searchText.toLowerCase()) >= 0);
      //return this.$root.$data.people;
    }
  },
}
</script>


<style scoped>

    .card {
        margin: 25px;
    }

    h1 h2 {
        margin: 20px;
        text-align: center;
    }
</style>