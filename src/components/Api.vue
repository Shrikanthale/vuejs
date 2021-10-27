<template>
    <div>
        <h1>Fetch data from API | Axios</h1> 
        <h1>Eployee List</h1>
        <table>
            <tr>
                <td>Name</td>
                <td>Salary</td>
                <td>Age</td>
            </tr>
            <tr v-for="item in list" v-bind:key="item.id">
                <td>{{item.employee_name}}</td>
                <td>{{item.employee_salary}}</td>
                <td>{{item.employee_age}}</td>
            </tr>
        </table>
    </div>
</template>

<script>
import Vue from 'vue';
import axios from 'axios';
import VueAxios from 'vue-axios'
Vue.use(VueAxios,axios)
export default {
    name:'Api',
    data(){
        return {list:undefined}
    },
    mounted() {
        Vue.axios.get('http://dummy.restapiexample.com/api/v1/employees')
        .then((res)=>{
            this.list=res.data.data;
            console.log(res.data.data)
        })
    }
}
</script>