<template>
    <div>
        <table border="1px">
            <tr>
                <th>Id</th>
                <th>Name</th>
                <th>Salary</th>
            </tr>
            <tr v-for="user in users" v-bind:key="user.id">
                <th>{{user.id}}</th>
                <th>{{user.employee_name}}</th>
                <th>{{user.employee_salary}}</th>
            </tr>
        </table>
    </div>
</template>

<script>
import Vue from 'vue';
import VueAxios from 'vue-axios';
import axios from 'axios';
Vue.use(VueAxios,axios)
export default {
    name:"EmployeeList",
    data(){
        return {users:undefined}
    },
    mounted(){

    Vue.axios.get('https://dummy.restapiexample.com/api/v1/employees')
    .then(res=>{
        console.warn("Api Output",res.data.data)
        this.users=res.data.data
    })
}
}

</script>