<template>
    <div> 
    <h1>Dynamic component </h1>
    <button @click="activeTab='Dynamicjava' " >Java</button>
    <button @click="activeTab='Dynamicnode' " >Node</button>
    <button @click="activeTab='Dynamicjavascript' " >Javascript</button>

    <Dynamicjava v-if="activeTab === 'Dynamicjava' "/>   
    <Dynamicnode v-if="activeTab === 'Dynamicnode' " />
    <Dynamicjavascript v-if="activeTab === 'Dynamicjavascript' "  /> 
    </div>
</template>

<script>

import Dynamicjava from './Dynamicjava.vue'
import Dynamicjavascript from './Dynamicjavascript.vue'
import Dynamicnode from './Dynamicnode.vue'
export default {
    name:'Dynamic',
    components:{
    Dynamicjava,
    Dynamicnode,
    Dynamicjavascript
    },
    data(){
        return {
            activeTab:'Dynamicjava'
        }
    }
}
</script>