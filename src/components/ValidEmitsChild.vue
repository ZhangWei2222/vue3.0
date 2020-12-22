<template>
  <div class="valid-emits-child">
    <button @click="submitForm"></button>
  </div>
</template>

<script>
export default {
  emits: {
    // 没有验证
    click: null,
    // 验证submit 事件
    submitChild: ({ email, password }) => {
      if (email && password) {
        return true;
      } else {
        console.error("Invalid submit event payload!");
        return false;
      }
    },
  },
  methods: {
    submitForm() {
      const email = "";
      const password = "";
      this.$emit("submitChild", { email, password });
    },
  },
};
</script>
