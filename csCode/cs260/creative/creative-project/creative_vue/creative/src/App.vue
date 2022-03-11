<template>
  <div id="app">
      <nav class="navbar navbar-expand navbar-dark bg-dark">
         <router-link class="navbar-brand" to="/"> AthleteUp </router-link>
      <div class="collapse navbar-collapse" id="navbarNav" style="color: white;">
            <router-link to="/"> Home </router-link>
             <router-link to="/about"> About </router-link>
            <router-link to="/coach"> Become A Coach </router-link>
            <router-link to="/explore"> Explore </router-link>
      </div>
    </nav>
    <router-view/>

    <nav class="footer navbar sticky-bottom navbar-dark bg-dark" style="color: white;">
    <div >Visit The following Pages to learn more about us:</div>
        <router-link to="/about"> About </router-link>
        <router-link to="/termsofservice"> Terms Of Service </router-link>
        <a class="nav-link" style="color: white;" href="https://github.com/adaraPark/creative">Github Link: https://github.com/adaraPark/creative</a>
        <router-link class="navbar-brand" to="/"> AthleteUp </router-link>
    </nav>
  </div>

  
</template>

<style scoped>
#app {
  font-size: 20px;
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: gray;
  margin-left: 7px;
  margin-right: 8px;
}

.footer{
  font-size: 17px;;
}

nav a {
  font-weight: bold;
  color:gray;
  margin-left: 7px;
  margin-right: 8px;
}

nav a.router-link-exact-active {
  color: grey;
  margin-left: 7px;
  margin-right: 8px;
}
</style>
