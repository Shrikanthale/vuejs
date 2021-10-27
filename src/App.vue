<template>
  <div id="app">
  <!-- <nav>
    <ul>
      <li>
        <router-link to="/">Home</router-link>
      </li>
      <li>
        <router-link to="/Dashboard">Dashboard</router-link>
      </li>
      <li>
        <router-link to="/Login">Login</router-link>
      </li>
      <li>
        <router-link to="/Signup">Signup</router-link>
      </li>
      <li>
        <router-link to="*"> </router-link>
      </li>
      
    </ul>
  </nav> -->
    <!-- <router-view></router-view> -->
    <!-- <h1> {{title}} </h1> -->
    <!-- <img alt="Vue logo" src="./assets/logo.png"> -->
    <!-- <HelloWorld msg="Welcome to Your Vue.js App"/> -->
    <!-- <Home data=" Shrikant is here " msg="u both work together" /> -->
    <!-- <Compo pass="pass msg from app.vue" pass1="u can paSS multiple msg "/>
    <IfElse msg="check if else condition here:"/>
    <Forloop msg="For Loop"/> -->
    <!-- <dashboard/> -->
    <!-- <Template/> -->
    <!-- <databinding/> -->
    <!-- <child v-on:changeTitle="updateTitleText($event)" /> -->
    <!-- <child1 name='Sam curran'/> -->
    <!-- <child1 v-bind:users=users /> -->
    <!-- <Login /> -->
    <!-- <signup /> -->
    <!-- <validation /> -->
    <!-- <div v-if="display">
      <lifecycle/>
    </div>
    <button v-on:click="toggle">Toggle</button> -->
    <!-- <Api /> -->
    <!-- <Bootstrap /> -->
    <!-- <Postdata/> -->
    <Dynamic />
  </div> 
</template>

<script>
// import Dynamic from './components/DynamicComponent/Dynamic.vue'
// import Postdata from './components/Postdata.vue'
// import Child from './components/Child.vue'
// import Child1 from './components/Child1.vue'
// import Databinding from './components/Databinding.vue'
// import Template from './components/Template.vue'
// import HelloWorld from './components/HelloWorld.vue'
// import Home from './components/Home.vue'
// import Dashboard from './components/Dashboard.vue'
// import Compo from './components/Compo.vue'
// import IfElse from './components/IfElse.vue'
// import Forloop from './components/Forloop.vue'
// import Login from './components/Login.vue'
// import Signup from './components/Signup.vue'
// import Validation from './components/Validation.vue'
// import Lifecycle from './components/Lifecycle.vue'
// import Api from './components/Api.vue'
// import Bootstrap from './components/Bootstrap.vue'
import Dynamic from './components/Dynamic.vue'

export default {
  name: 'App',
  components: {
    Dynamic
    // Postdata
    // Child1
    // Child
    // Template,
    // Databinding
    // HelloWorld,
    // Dashboard,
    // Home,
    // Compo,
    // IfElse,
    // Forloop,
    // Login,
    // Signup,
    // Validation,
    // Lifecycle,
    // Api
    // Bootstrap
    
  }
  // ,data(){
  //   return{
  //     display: true,
  //   }
  // },
  // methods: {
  //   toggle()
  //   {
  //     this.display=!this.display;
  //   }
  // }
  // ,
  // data () {
  //   return{
  //     // name:"Alex hales"
  //     users:[
  //       {name:"Sam" ,age:24},
  //       {name:"Alex" ,age:34},
  //       {name:"Hannah" ,age:24},
  //     ]
  //   }
  // }
  // ,data()
  // {
  //   return {
  //     title:"pass data from Child component to parent component"
  //   }
  // },
  // methods: {
  //   updateTitleText(title)
  //   {
  //     this.title = title
  //   }
  // }
}
</script>

<style lang="scss">
@import "~@/assets/scss/vendors/bootstrap-vue/index";
@import "~@/assets/scss/vendors/bootstrap-vue/index";
@import "~@/assets/scss/vendors/bootstrap-vue/index";
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
