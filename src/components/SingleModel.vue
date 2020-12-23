<template>
  <div class="single-model">
    {{ bookTitle }}
    <SingleModelChild v-model:title="bookTitle"></SingleModelChild>
  </div>
</template>

<script>
import SingleModelChild from "./SingleModelChild.vue";
export default {
  data() {
    return {
      bookTitle: "我是书本",
    };
  },
  components: {
    SingleModelChild,
  },
};
</script>
