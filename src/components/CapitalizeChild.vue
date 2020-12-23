<template>
  <div class="capitalize-child">
    <input type="text" v-model="myText" @input="emitValue" />
  </div>
</template>

<script>
export default {
  props: {
    myText: String,
    myTextModifiers: {
      default: () => ({}),
    },
  },
  emits: ["update:myText"],
  created() {
    console.log(this.myTextModifiers); // { capitalize: true }
  },
  methods: {
    emitValue(e) {
      let value = e.target.value;
      if (this.myTextModifiers.capitalize) {
        value = value.charAt(0).toUpperCase() + value.slice(1);
      }
      this.$emit("update:myText", value);
    },
  },
};
</script>
