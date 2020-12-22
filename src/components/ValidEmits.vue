<template>
  <div class="valid-emits">
    <ValidEmitsChild @submitChild="submit"></ValidEmitsChild>
  </div>
</template>

<script>
import ValidEmitsChild from "./ValidEmitsChild.vue";

export default {
  methods: {
    submit(event) {
      console.log("提交"); // 将记录所选选项的值
    },
  },
  components: {
    ValidEmitsChild,
  },
};
</script>
