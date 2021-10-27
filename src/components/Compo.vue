<template>
    <div>
        <h1>hello World</h1>
        <h1>{{pass}}</h1>
        <h1>{{pass1}}</h1>
        <button v-on:mouseover="Compo('u can show here your data')" >click me</button>
        <h1 v-if="show">if block </h1>
        <h1 v-else>else block </h1>
        <button v-on:click="display">Toogle</button>
        <!-- <table>
            <tr>
                <td>id</td><td>name</td>age<td></td>
            </tr>
            <tr v-for="user in users" :key="user.age">
              <td>{{user.id}}</td>
              <td>{{user.name}}</td>
              <td>{{user.age}}</td>
            </tr>
        </table> -->
    </div>
</template>

<script>
export default {
    name:'Compo',
    props:{
        pass:String,
        pass1:String
    },data(){
        return {
            show : false
        }
    },
    // methods:{
    //     display()
    //     {
    //         this.show = !this.show;
    //     }
    //     },
        // data(){
        //     return {
        //         users: [
        //           {id:1,name:"shri",age:22},
        //           {id:2,name:"jason",age:26},
        //           {id:3,name:"hannah",age:24},
        //         ]
        //     }
        // }
    // methods:{
    //     Compo(msg)
    //     {
    //         alert(msg)
    //     }
    // }
}
</script>