<template>
    <div>
        <h2 v-for="user in users" :key="user.name">{{user.name}}</h2>
        <h2 v-for="user in users" :key="user.name">{{user.age}}</h2>
    </div>
</template>

<script>
export default {
    name:'child1',
    props:['users']
}
</script>