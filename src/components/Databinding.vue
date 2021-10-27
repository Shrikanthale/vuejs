<template>
    <div>
        <h1>{{message}}</h1>
        <input type="text" v-model="message" />
    </div>
</template>

<script>
export default {
    name:'databinding',
    data(){
        return{
           message:" "
        }
    }
}
</script>