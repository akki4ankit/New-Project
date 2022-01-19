<template>
    <div><table border="1px">
        <input type="text" placeholder="Name" v-model="user.name"/><br><br>
        <input type="password" placeholder="Password" v-model="user.password"/><br><br>
        <p>Select Hobbies</p>
        <input type="checkbox" id="cricket"  value="cricket" v-model="user.hobbies">
        <label for="cricket">Cricket</label>
        <input type="checkbox" id="Football" value="Football" v-model="user.hobbies">
        <label for="Football">Football</label><br><br>
        <p>select gender</p>
        <input type="radio" id="male" value="male" v-model="user.gender">
        <label for="male">Male</label><br><br>
        <input type="radio" id="female" value="female" v-model="user.gender">
        <label for="female">Female</label><br><br>
        <button v-on:click="sign()">sign Up</button>
        </table>
    </div>
</template>

<script>
export default {
    name:'Form1',
    data(){
        return{
            user:{
                name:null,
                password:null,
                hobbies:[],
                gender:null
            }
        }
    },
    methods:{
        sign(){
           console.warn(this.user)
        }
    }
    
}
</script>