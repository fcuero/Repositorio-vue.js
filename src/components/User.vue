<template lang="html">
    <div class="Users">
        <h1>Bienvenidos</h1>
        <ul>
            <li v-for="user in users">
            {{ user. name }} : {{ user. email }} 
            <button v-on:click="deleteUser(user)">x</button>
            </li>
        </ul>
        <form v-on:submit.prevent="addUser">
            <input type="text" v-model="newUser.name" placeholder="Name">
            <input type="email" v-model="newUser.email" placeholder="Email">
           
            <button type="submit">
                Add
            </button>
        
        </form>
    </div>


    

</template>
<script>
 export default{
  data() {
    return {
        users: [
         {
            name: 'yeison',
            email: 'yeison@amil.com',
            contacted: false
         },
         {
            name: 'avatar',
            email: 'avatar@amil.com',
            contacted: false
         },
         {
            name: 'jose',
            email: 'jose@amil.com',
            contacted: 3242435353
         },
         {
            name: 'carlos',
            email: 'carlos@amil.com',
            contacted: true
         }
        ],
        newUser:{}  

    }
  },

  methods: {
       addUser(){
       this.users.push(this.newUser);
       this.newUser = {};
    },
    deleteUser(user){
        alert('Advertencia estas seguro de eliminar este elemento')
        this.users.splice(this.users.indexOf(user), 1);
        
    }
    
  }
  

 }

</script>
<style lang="css">
 .template{
      padding: 2px;
  }
 .Users{
    background: #00fff7;
    color: #fff;
    padding: 15px;
 }

</style>