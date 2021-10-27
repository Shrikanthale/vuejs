<template>
  <div>
    <h1>Form validation</h1>
    <!-- <p v-if="error.length">
        <b>please enter the follwing errors </b>
        <ul>
            <li v-for="e in error" v-bind:key="e.id">
                {{e}}
            </li>
        </ul> 
    </p> -->
    <form @submit="login">
      <input type="text" placeholder="Enter user name" v-model="name" /><br><br>
      <input
        type="password"
        placeholder="Enter user password"
        v-model="password"
      /><br><br>
      <button type="submit">Login</button>
    </form>
  </div>
</template>

<script>
export default {
  name: "Login",
  data()
  {
    return{
        errors:[],
        name:null,
        password:null
    }
  },
  methods: {
    login(e)
    {
        if(this.name && this.password){
            console.log("Loginfunction Called")
        }
        this.errors=[];
        if(!this.name){
            this.error.push("name is required")
        }
        if(!this.password){
            this.error.push("password is required")
        }
        // console.warn("ERRORS",this.error)
        e.preventDefault();
    } 
  }
};
</script>