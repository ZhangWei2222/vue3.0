<template>
  <div class="mord-model">
    {{ firstName }}-{{ lastName }}
    <MoreModelChild
      v-model:first-name="firstName"
      v-model:last-name="lastName"
    ></MoreModelChild>
  </div>
</template>

<script>
import MoreModelChild from "./MoreModelChild.vue";
export default {
  data() {
    return {
      firstName: "我是第一个名字",
      lastName: "我是最后一个名字",
    };
  },
  components: {
    MoreModelChild,
  },
};
</script>
