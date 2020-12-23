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
  <Slot />
</template>

<script>
import HelloWorld from "./components/HelloWorld.vue";
import TodoList from "./components/TodoList.vue";
import BlogPosts from "./components/BlogPosts.vue";
import Custom from "./components/Custom.vue";
import NoProp from "./components/NoProp.vue";
import ForceUpdate from "./components/ForceUpdate.vue";
import ValidEmits from './components/ValidEmits.vue';
import SingleModel from './components/SingleModel.vue';
import MoreModel from './components/MoreModel.vue';
import Capitalize from './components/Capitalize.vue';
import Slot from './components/Slot.vue';

export default {
  name: "App",
  components: {
    HelloWorld,
    TodoList,
    BlogPosts,
    Custom,
    NoProp,
    ForceUpdate,
    ValidEmits,
    SingleModel,
    MoreModel,
    Capitalize,
    Slot
  },
};
</script>
