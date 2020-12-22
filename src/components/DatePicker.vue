<template>
  <!-- <div class="date-picker">
    <input type="datetime" v-bind="$attrs" />
    <select>
      <option value="1">Yesterday</option>
      <option value="2">Today</option>
      <option value="3">Tomorrow</option>
    </select>
  </div> -->
  <header></header>
  <main v-bind="$attrs">
    <input type="datetime" />
  </main>
  <footer></footer>
</template>

<script>
export default {
  created() {
    // console.log(this.$attrs); // { onChange: () => {}  }
    // console.log(this.$attrs["data-status"]); // activated
  },
};
</script>
