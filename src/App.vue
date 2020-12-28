<template>
  <!-- <img alt="Vue logo" src="./assets/logo.png" /> -->
  <!-- <HelloWorld msg="Hello Vue 3.0 + Vite" /> -->
  <!-- <TodoList/> -->
  <!-- <BlogPosts/> -->
  <!-- <Custom /> -->
  <!-- <NoProp /> -->
  <!-- <ValidEmits /> -->
  <!-- <SingleModel /> -->
  <!-- <MoreModel /> -->
  <!-- <Capitalize /> -->
  <!-- <Slot /> -->
  <!-- <Provide /> -->
  <Setup/>
</template>

<script>
import HelloWorld from "./components/HelloWorld.vue";
import TodoList from "./components/TodoList.vue";
import BlogPosts from "./components/BlogPosts.vue";
import Custom from "./components/Custom.vue";
import NoProp from "./components/NoProp.vue";
import ValidEmits from './components/ValidEmits.vue';
import SingleModel from './components/SingleModel.vue';
import MoreModel from './components/MoreModel.vue';
import Capitalize from './components/Capitalize.vue';
import Slot from './components/Slot.vue';
import Provide from './components/Provide.vue';
import Setup from './components/Setup.vue';

export default {
  name: "App",
  components: {
    HelloWorld,
    TodoList,
    BlogPosts,
    Custom,
    NoProp,
    ValidEmits,
    SingleModel,
    MoreModel,
    Capitalize,
    Slot,
    Provide,
    Setup
  },
};
</script>
