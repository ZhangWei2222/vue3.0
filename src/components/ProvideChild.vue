<template>
  <div class="provide-child"></div>
</template>

<script>
export default {
  inject: ["user", "todoLength"],
  created() {
    console.log(`Injected property: ${this.user}`); // > 注入 property: John Doe
    console.log(`Injected property: ${this.todoLength.value}`); // 2
  },
  watch: {
    "todoLength.value"(cur, old) {
      console.log(cur, old);
    },
  },
};
</script>
