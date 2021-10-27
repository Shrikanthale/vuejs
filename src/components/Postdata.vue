<template>
  <div>
    <h1>Post data</h1>
    <form @submit="Postdata" method="post">
      <input type="text" name="title" placeholder="enter title" v-model="posts.title" /><br /><br />
      <input type="text" name="author" placeholder="enter author" v-model="posts.author" /><br /><br />
      <button type="submit">Post</button>
    </form>
  </div>
</template>

<script>
// import  Vue from 'Vue' 
// import axios from 'axios'
// import VueAxios from 'vue-axios'
// Vue.use(VueAxios, axios)
export default {
  name: "Postdata",
  data() {
    return {
      posts: {
        title: null,
        author: null,
      },
    };
  },
  methods: {
    Postdata(e) 
    {
      // console.log(this.posts)
      this.axios.post("http://localhost:3000/posts",this.posts)
      .then((res)=>{
        console.log(res)
      })
      e.preventDefault();
    },
  },
};
</script>