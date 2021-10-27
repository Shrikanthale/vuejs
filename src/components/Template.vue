
<template>
    <div>
        <!-- javascript property used in html without any class, getelementbyId etc -->
        <!-- <h1>Template in vue </h1> -->
        <!-- <h2 v-once>{{name}}</h2> -->
        <p v-html="header"></p>
        <h2>{{name}}</h2>
        <!-- <button v-on:click="change">click me</button> -->
        <button v-bind:disabled="btnDisabled" v-on:click="change">click me</button>
        <!-- <p>{{15+30}}</p>
        <p>{{15*30}}</p> -->
        <h3>{{ok?"yes":"no"}}</h3>
    </div>
</template>

<script>
export default {
    name:'template',
    data(){
        return{
            name:'sam',
            ok:true,
            header:"<h1>Template in vue(use html header) </h1>",
            btnDisabled:true,
        }
    },methods:
    {
        change()
        {
            // alert("Hello click")
            // this.name = 'shrikant';

            // this.ok =false
            this.ok=!this.ok
        }
    }
}
</script>