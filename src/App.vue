<template>
  <!-- <img alt="Vue logo" src="./assets/logo.png" /> -->
  <HelloWorld />
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
  <!-- <Setup /> -->
  <!-- <TeleportDEMO /> -->
</template>

<script>
import HelloWorld from "./components/HelloWorld.vue";
import TodoList from "./components/TodoList.vue";
import BlogPosts from "./components/BlogPosts.vue";
import Custom from "./components/Custom.vue";
import NoProp from "./components/NoProp.vue";
import ValidEmits from "./components/ValidEmits.vue";
import SingleModel from "./components/SingleModel.vue";
import MoreModel from "./components/MoreModel.vue";
import Capitalize from "./components/Capitalize.vue";
import Slot from "./components/Slot.vue";
import Provide from "./components/Provide.vue";
import Setup from "./components/Setup.vue";
import TeleportDEMO from "./components/Teleport.vue";

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
    Setup,
    TeleportDEMO,
  },
};
</script>
