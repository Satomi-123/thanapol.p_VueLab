<template>
  <div class="container">
    <manufacturer v-slot="data">
      <devices v-bind:manufacturerId="data.factId"></devices>
    </manufacturer>
    <!-- <Manufacturer /> -->
  </div>
</template>

<script>
import Manufacturer from "@/components/Manufacturer.vue"; //@ = SRC
import Devices from "@/components/Devices.vue";
export default {
  //name: "App", เพ่ือให้ดึงชื่อ main มาใช้
  components: {
    Manufacturer: Manufacturer,
    Devices: Devices,
  },
};
</script>
