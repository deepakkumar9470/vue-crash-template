<template>
  <h1>About Page</h1>
   <div class="container">
      <h4>Welcome to About</h4>
      <p>Lorem ipsum, dolor sit amet consectetur adipisicing elit. Autem quibusdam dolores qui omnis expedita atque fugit nihil ipsa repellat, rerum exercitationem officia ullam debitis possimus excepturi rem, libero non hic!</p>
   </div>
</template>

<script>
export default {
 name : 'About'
}
</script>

<style scoped>

.containedr{
   display: flex;
   width: 80%;
   height: 40vh;
   padding: 20px;
   margin: 0 auto;
   flex-direction: column;
   background: #FEFBF3;
   box-shadow: 1px 2px 2px 3px rgba(219, 217, 217, 0.67);
}
.container p{
   padding: 10px 0px;
   width: 90%;

}
</style>
