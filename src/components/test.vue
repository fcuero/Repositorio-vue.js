<template>
<div class="test">

   {{ msg }}

</div>



</template>

<script>
 export default{

    data(){
        return{
        title: 'hola vuejs',

        user: {
            firstNeme: 'fabio',
            lastName: 'mcmillan'
        },
        myhtml: '<h3>holo vuejs</h3>',
        showName: true,
        tasks:[
            {title:'eat'},
            {title:'cos'},
            {title:'uj'},
            {title:'fr'},
       ]
     }
       
    },
    props: {
        msg:{
            type: String
        }
    }

   
        
 }

</script>

<style median="screen">
.test{
    background-color: #eee;
}


</style>