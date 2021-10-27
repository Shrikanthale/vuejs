// two things define one html part and second js
// template define html code and in script define js code

<template>
<div>
<h1>hello shri from home component</h1>
<h1> {{data}} </h1>
<h1> {{msg}} </h1>
<button v-on:mouseover="hello('u can pass data here')" >call me</button>
<h1 v-if="show">condition</h1>
<!-- <h1 v-else> else parts </h1> -->
<button v-on:click="display">Toogle</button>
</div>
</template>

<script>
export default {
    name:'home',
    props:{
        data:String,
        msg:String
    },// ,methods:{
    //     hello(item)
    //     {
    //         alert(item);
    //     }
    // }
    data()
    {
      return {
          show:false
      }
    },
    methods:{
        display()
        {
            this.show = ! this.show
        }
    }
}
</script>