<template>
  <div class="single-model-child">
    {{ title }}
    <button @click="changeTitle"></button>
  </div>
</template>

<script>
export default {
  props: ["title"],
  emits: ["update:title"],
  methods: {
    changeTitle() {
      this.$emit("update:title", "我是树11");
    },
  },
};
</script>
