<template>
  <div class="container">
    <manufacturer v-slot="data">
      <devices v-bind:manufacturerID="data.factID"></devices>
    </manufacturer>
  </div>
</template>

<script>
import Manufacturer from "@/components/Manufacturer.vue";
import Devices from "@/components/Devices.vue";
export default {
  components: {
    Manufacturer: Manufacturer,
    Devices: Devices,
  },
};
</script>

