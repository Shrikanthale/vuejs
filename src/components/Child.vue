<template>
    <div>
        <button v-on:click="upadateTitile">Update Title</button>
    </div>
</template>

<script>
export default {
    name:'child',
    methods: {
        upadateTitile(){
            // console.log("updateTitle")
            this.$emit('changeTitle','props will be passed')
        }
    },
}
</script>