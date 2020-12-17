<template>
  <!-- <img alt="Vue logo" src="./assets/logo.png" /> -->
  <!-- <HelloWorld msg="Hello Vue 3.0 + Vite" /> -->
  <!-- <TodoList/> -->
  <!-- <BlogPosts/> -->
  <Custom />
</template>

<script>
import HelloWorld from "./components/HelloWorld.vue";
import TodoList from "./components/TodoList.vue";
import BlogPosts from "./components/BlogPosts.vue";
import Custom from "./components/Custom.vue";

export default {
  name: "App",
  components: {
    HelloWorld,
    TodoList,
    BlogPosts,
    Custom,
  },
};
</script>
