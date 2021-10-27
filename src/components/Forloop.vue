<template>
    <div>
        <h1>{{msg}}</h1>
        
        <table>
            <tr>
              <td>Id</td><td>name</td><td>Email</td> 
            </tr>
            
            <tr v-for="user in users" :key="user.id">
                <td>{{user.id}}</td>
                <td>{{user.name}}</td>
                <td>{{user.Email}}</td>
            </tr>
        </table>    
    </div>
</template>

<script>
export default {
    name:'forloop',
    props:{
        msg:String
    },data()
    {
        return {
            users:[
                {id:1,name:"sam",Email:"sam@.com"},
                {id:2,name:"tom",Email:"tom@.com"},
                {id:3,name:"alex",Email:"alex@.com"},
                {id:4,name:"hannh",Email:"hannah@.com"},
            ]}
    }
}
</script>