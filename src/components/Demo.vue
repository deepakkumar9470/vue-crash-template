<template>
  <div class="text">
      <h3>Hello {{name}}</h3>
      <span>Age : {{age}}</span>
      <span>Address : {{add}}</span>
      <span>{{count}}</span>
      <button @click="counter">Click</button>

      <ul v-for="(x ,i) in user" :key="x.id">
          <li> Id: {{i+1}}</li>
          <li> Name: {{x.name}}</li>
          <li> RollNo: {{x.rollno}}</li>
          <li @click="remove(x.id)">x</li>
      </ul>

     
  </div>

  
  
</template>

<script>
export default {
  name  : 'Demo',
  props: {
      name : String,
      age : Number,
      add : String
  },
  data (){
      return {
          count : 0,
          user : [
              {id:  1,name:'Dk', rollno:12},
              {id:  2,name:'Ak', rollno:1},
              {id:  3,name:'Dhk', rollno:13},
              {id:  4,name:'Anujk', rollno:2},
              {id:  5,name:'Suraj', rollno:10},
          ]
      }
  },
  methods: {
      counter (){
          this.count = this.count+1
      }
       ,
      remove(id){
            if(confirm('Are you sure')){
                this.user = this.user.filter((item)=> item.id !==id)
            }
      }
  },
 
}
</script>

<style>
 
.text{
    display: flex;
    align-items: center;
    justify-content: center;
    flex-direction: column;
}
h3{
     padding: 5px;
     background-color: rgb(43, 241, 241);
      padding: 5px 10px;
      margin-bottom: 5px;
      color: #333;
      border-radius: 3px;
      cursor: pointer;
      border-right: 5px solid rgb(13, 137, 209);
}
  span{
      background-color: cadetblue;
      padding: 5px 10px;
      margin-bottom: 5px;
      color: #fff;
      border-radius: 3px;
      cursor: pointer;
      border-right: 5px solid rgb(207, 205, 205);
  }
</style>