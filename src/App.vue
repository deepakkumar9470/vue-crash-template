<template>
 
  
       <!-- <h2>Vue JS Crash Course App!</h2> -->
       <Navbar/>
  

       <router-view></router-view>

</template>




<script>
import Navbar from './components/Navbar.vue';

export default {
  name: 'App',
  components: { Navbar }
}
</script>


<style>
@import './style.css';
#app {
  
}
</style>
