<template>
  <div class="capitalize">
    <CapitalizeChild v-model:myText.capitalize="myText"></CapitalizeChild>
  </div>
</template>

<script>
import CapitalizeChild from "./CapitalizeChild.vue";
export default {
  data() {
    return {
      myText: "我是第一个名字",
    };
  },
  components: {
    CapitalizeChild,
  },
};
</script>
