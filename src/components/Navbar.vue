<template>
   <nav>
       <div class="logo">
           <router-link class="link" to="/"><h3>DEEPAK</h3></router-link>
       </div>


       <ul>
           <li><router-link to="/">Home</router-link></li>
           <li><router-link to="/about">About</router-link></li>
           <li><router-link to="/contact">Contact</router-link></li>
           <img src="https://images.pexels.com/photos/1043471/pexels-photo-1043471.jpeg?auto=compress&cs=tinysrgb&w=1260&h=750&dpr=1" alt="nopic">
       </ul>
       
   </nav>
</template>

<script>
export default {
   name: 'Navbar'

}
</script>

<style>
.link{
    text-decoration: none;
    color: #fff;
}
</style>