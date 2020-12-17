<template>
  <div class="custom">
    {{ searchText }}
    <CustomInput v-model="searchText"></CustomInput>
  </div>
</template>

<script>
import CustomInput from "./CustomInput.vue";

export default {
  data() {
    return {
      searchText: "",
    };
  },
  components: {
    CustomInput,
  },
};
</script>
