<template>
    <div>
        <h1>SignUp Form </h1>
        <input type="text" placeholder="Enter User name" v-model="signupForm.username" /> <br> <br>
        <input type="password" placeholder="Password" v-model="signupForm.password" /> <br> <br>

        <p>Hobbies</p>
        <input type="checkbox" value="travel" id="travel" v-model="signupForm.hobbies" />
        <label for="travel">Travel</label> <br>

        <input type="checkbox" value="sport" id="travel" v-model="signupForm.hobbies" />
        <label for="Sport">Sport</label> <br>

        <p>Gender</p>

        <input type="checkbox" value="male" id="male" />
        <label for="male">Male</label> <br>
        <input type="checkbox" value="female" id="female" />
        <label for="female">Female</label> <br>

        <button v-on:click="signupUser">Submit</button>
    </div>
</template>

<script>
export default {
    name:'SignUp',
    data(){
        return {
            signupForm:{
                username:null,
                password:null,
                hobbies:[],
                gender:"",
            }
        }
    },
    methods:{
        signupUser()
        {
            console.log("hi!" , this.signupForm)
        }
    }
}
</script>