<template>
  <div class="more-model-child">
    {{ firstName }}-{{ lastName }}
    <button @click="changeName"></button>
  </div>
</template>

<script>
export default {
  props: {
    firstName: String,
    lastName: String,
  },
  emits: ["update:firstName", "update:lastName"],
  methods: {
    changeName() {
      this.$emit("update:firstName", "我是树11");
      this.$emit("update:lastName", "我是树22");
    },
  },
};
</script>
