<template>
  <div class="setup">
    11{{location}}
    <button @click="changeTitle()">点我</button>
    <SetupChild></SetupChild>
  </div>
</template>

<script>
import SetupChild from "./SetupChild.vue";
import { provide, reactive, ref, readonly } from "vue";

export default {
  data() {
    return {
      title: "一本书",
    };
  },
  setup() {
    const location = ref("North Pole");
    const geolocation = reactive({
      longitude: 90,
      latitude: 135,
    });

    const updateLocation = () => {
      location.value = "South Pole";
    };

    provide("location", readonly(location));
    provide("geolocation", readonly(geolocation));
    provide("updateLocation", updateLocation);
    return {
      location
    }
  },
  components: {
    SetupChild,
  },
  methods: {
    changeTitle() {
      console.log("11");
      this.location = "South Pole";
    },
  },
};
</script>
