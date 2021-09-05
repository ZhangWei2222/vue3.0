<template>
  <div class="teloport" style="position: relative">
    <h3>Tooltips with Vue 3 Teleport</h3>
    <div>
      <TeleportChild></TeleportChild>
    </div>
  </div>
</template>

<script>
import TeleportChild from "./TeleportChild.vue";

export default {
  components: {
    TeleportChild,
  },
};
</script>


