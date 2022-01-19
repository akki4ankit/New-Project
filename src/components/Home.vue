<template>
<div>
<!-- <h1>Hello Vue Im Ankit</h1>
<h2>{{data}}</h2> 
<button v-on:click="hello('Amit Crazy XYZ')" >click Me </button> 
<h1 v-if="show"> Hello And Welcome in Vue.js</h1>
<h1 v-else> Hello And Welcome  in else Vue.js</h1>
<button v-on:click="hello()">Toggle Button</button>
<h1>For loop Example</h1>
<table border="1px">
    <tr>
        <td>Id</td>
        <td>Name</td>
        <td>Email</td>
    </tr>
    <tr v-for="user in users" :key="user.id">
        <td>{{user.id}}</td>
        <td>{{user.name}}</td>
        <td>{{user.email}}</td>     
    </tr>
</table> -->
<h1>Home component</h1>
<homechild1/>
<homechild2/>
<homechild1/>
</div>
</template>
<script>
import homechild1 from './homechild1.vue'
import homechild2 from './homechild2.vue'
export default{
  components: { homechild1,homechild2 },
    name:"Home",
    /* props:{
        data:String
    },data(){
        return {show:true}
    },
    data(){
        return{
            users:[
                {id:1,name:"peter",email:"peter@gmail.com"},
                {id:2,name:"Sam",email:"sam@gmail.com"},
                {id:3,name:"Vector",email:"vector@gmail.com"},
                {id:4,name:"roman",email:"roman@gmail.com"}
            ]
        }
    },
    methods:{
        hello(){
            //console.log(data)
            this.show=!this.show
        }
    }, */
    
}
</script>
<style scoped>
div{
    background-color: aqua;
    height: 100px;
    width:300px;
    padding: 42px;

}
</style>