<template>
  <div id="todo-item">
    <li>
      {{ title }}
      <button @click="$emit('remove')">Remove</button>
    </li>
  </div>
</template>

<script>
export default {
  props: ["title"],
  emits: ["remove"],
};
</script>
