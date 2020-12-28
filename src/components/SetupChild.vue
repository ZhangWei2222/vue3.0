<template>
  <div class="setup-child">
    <button @click="changeTitle()">点我1111</button>
    {{ userLocation }}
    {{ userGeolocation }}
  </div>
</template>

<script>
import { toRefs, onMounted, onUpdated, computed, watch } from "vue";
import { inject } from "vue";

export default {
  inject: ["location", "geolocation"],
  setup() {
     const userLocation = inject('location', 'The Universe')
    const userGeolocation = inject('geolocation')
    const updateUserLocation = inject('updateLocation')

    return {
      userLocation,
      userGeolocation,
      updateUserLocation
    }
  },
  methods: {
    changeTitle() {
      // this.updateUserLocation();
      this.userLocation= '111'
    },
  },
};
</script>
