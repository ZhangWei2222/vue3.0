<template>
  <div class="slot">
    <SlotChild
      ><template v-slot:default="slotProps">
        <i class="fas fa-check"></i>
        <span class="green">{{ slotProps }} {{ slotProps.item }}</span>
      </template></SlotChild
    >
  </div>
</template>

<script>
import SlotChild from "./SlotChild.vue";

export default {
  components: {
    SlotChild,
  },
};
</script>
