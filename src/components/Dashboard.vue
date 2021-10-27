<template>
    <div class="dash">
        <h1>HOME PAGE</h1>
        <About/>
        <Contact/>
    </div>
</template>

<script>
import About from './About.vue'
import Contact from './Contact.vue'
export default {
    name:"dashboard",
    components:{
        About,
        Contact
    }
}
</script>

<style scoped>
.dash{
    background:rgb(255, 10,180);
    /* text-align:center; */
    height:500%;
    width:100%;
    padding: auto;
    margin: 15px;
}
</style>