<template>
 
  <h1>Contact Page</h1>
  <div class="form">
       <div class="input">
            <label class="input_label" for="name">Name</label>
            <input type="text" name="name" placeholder="Enter name...">
       </div>
       <div class="input">
            <label class="input_label" for="name">Email</label>
            <input type="text" name="email" placeholder="Enter email...">
       </div>
       <div class="input">
            <label class="input_label" for="name">Message</label>
            <input type="text" name="message" placeholder="Enter message...">
       </div>
       <div class="input">
            <button>Send</button>
       </div>
  </div>
</template>

<script>
export default {
name : 'Contact'
}
</script>

<style>

.form{
  width: 60%;
  height: 50vh;
  display: flex;
  margin: 0 auto;
  color: #fff;
  padding: 20px;
  align-items: center;
  background-image: url('https://images.pexels.com/photos/3293148/pexels-photo-3293148.jpeg?auto=compress&cs=tinysrgb&w=1260&h=750&dpr=1');
  justify-content: center;
  object-fit: cover;
  background-size: 100%;
  flex-direction: column;
}
.input{
  width: 400px;
}
.input .input_label{
  font-size: 20px;
  margin-bottom: 10px;
  padding: 10px 0px;
  color: #fff;
}
.input input{
  width: 100%;
  padding: 10px 5px;
  outline: none;
  color: #333;
  border-radius: 4px;
  border: 1px solid gray;
  margin-bottom: 10px;
}
.button{
  width: 100px;
}
 .input button{
   width: 100%;
   font-size: 18px;
   background: #3E00FF;
   color: #fff;
   border-radius: 4px;
   padding: 10px 20px;
   border: none;
   outline: none;
   cursor: pointer;
 }
</style>