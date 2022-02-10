<template>

<li>
  <h2>{{ friend.name }}</h2>
  <button @click="toggledet">Show Details</button>

<ul v-if="detailvisible">
  <li><strong>Phone:</strong> {{ friend.phone }} </li>
  <li><strong>Email:</strong> {{ friend.email }} </li>
</ul>
</li>
  </template>

  <script>

  export default {
  
   data() {
     return{
       detailvisible:false,
       friend: {
           
               id: 'ishita', 
               name: 'Ishita Shah',
               phone: '0897 567 991', 
               email: 'ishita@gmail.com' 
               },
       
          };
      },
     methods: {
       toggledet() {
         this.detailvisible = !this.detailvisible;
       }
     } 
  };
  </script>
  
    
  
