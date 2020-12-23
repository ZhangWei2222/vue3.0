<template>
  <div class="provide">
    {{ todos.length }}
    <button @click="todos.push('111')"></button>
    <ProvideChild></ProvideChild>
  </div>
</template>

<script>
import { computed } from "vue";
import ProvideChild from "./ProvideChild.vue";

export default {
  data() {
    return {
      todos: ["Feed a cat", "Buy tickets"],
    };
  },
  //   provide: {
  //     user: "John Doe",
  //     todoLength: this.todos.length // 将会导致错误 'Cannot read property 'length' of undefined`
  //   },
  provide() {
    return {
      user: "John Doe",
      todoLength: computed(() => this.todos.length),
    };
  },
  components: {
    ProvideChild,
  },
};
</script>
