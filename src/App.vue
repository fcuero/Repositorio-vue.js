<template>
  <div id="app">
    <div>
  <h3>REPOSITORIO VUE.JS</h3>
</div>
   <h1>STAR WARS</h1><hr>
   <h5>ingrese la siguiente informacion</h5><hr>
   
   <!--<test msg="hola!!!!"/>-->
  
   <User name/>
   
   <!--<nav>
    <ul>
      <li>
        <a href="#">test</a>
      </li>
      <li>
        <a href="#">User</a>
      </li>
    </ul>
   </nav>
   <router-view></router-view>-->
   
  </div>
</template>

<script>
 
import test from './components/test.vue';

import User from './components/User.vue';

export default {
  name: 'App',
  components: {
    test,
    User
  }
}
</script>

<style>
 #template{
      padding: 2px;
  }
#app {
  background: #6f00ff;
  padding: 5px;
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 40px;
}
</style>
