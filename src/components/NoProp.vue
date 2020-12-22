<template>
  <div class="no-prop">
    <DatePicker
      class="no"
      data-status="activated"
      @change="showChange"
    ></DatePicker>
  </div>
</template>

<script>
import DatePicker from "./DatePicker.vue";

export default {
  methods: {
    showChange(event) {
      console.log(event.target.value); // 将记录所选选项的值
    },
  },
  components: {
    DatePicker,
  },
};
</script>
