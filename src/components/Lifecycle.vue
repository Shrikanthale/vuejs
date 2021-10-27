<template>
    <div>
        <h1 id="demo">{{name}}</h1>
    </div>
</template>

<script>
export default {
    name:'Lifecycle',
    data(){
        return{
            name:'SAM'
        }
    },
    created() {
        // this.name="SHRI" it will be run after beforCreated run
        console.log("created",this.name)
    },
    beforeCreate() {
        //beforeCrerated first run then rest of methods
        this.name="SHRI"
        console.log("beforeCreated",this.name)
    },
    mounted() {
        // it will be mount after beforeMount 
        console.log("mounted",document.getElementById('demo'));
    },
    beforeMount() {
        // console.log("beforeMount",this.$el) first mount then after rest of mount
        console.log("beforeMount",document.getElementById('demo'));
    },
    destroyed() {
        console.log("Destoyed method called after the beforeDestoye method called")
    },
    beforeDestroy() {
        console.log("beforeDestroy");
    }
}
</script>