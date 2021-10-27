<template>
    <div>
        <h1>Form in vue js</h1>
        <input type="text" placeholder="Enter user Name" v-model="loginForm.username" /> <br> <br>
        <input type="password" placeholder="Enter user password" v-model="loginForm.password"/> <br> <br>
        <button v-on:click="getLogin" >Login</button>
    </div>
</template>

<script>
export default {
    name:'Login',
    data(){
        return{
            loginForm: {
                username:null,
                password:null
            }
        }
    },
    methods: {
        getLogin()
        {
            console.log("getLogin called",this.loginForm.username,this.loginForm.password)
        }
    }
}
</script>