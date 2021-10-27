<template>
    <div>
      <h1>{{msg}}</h1> 
      <h1 v-if="show">if condition true </h1>
      <h1 v-else>else parts here </h1>
      <button v-on:click="display">Toggle</button>
    </div>
</template>

<script>
export default {
    name:'IfElse',
    props:{
        msg:String
    },data()
    {
        return {
            show:false
        }
    },methods:{
        display()
        {
            this.show = !this.show;
        }
    }
}
</script>