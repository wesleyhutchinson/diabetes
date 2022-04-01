<template>
  <div class="navbar">
    <v-btn @click="setSide('both')">Both</v-btn>
    <v-btn @click="setSide('right')">Right</v-btn>
    <v-btn @click="setSide('left')">Left</v-btn>
  </div>
</template>

<script>
export default {
  methods: {
    setSide(side) {
      if (side == "right") {
        this.$emit("emitLayout", { left: false, right: true });
      } else if (side == "left") {
        this.$emit("emitLayout", { left: true, right: false });
      } else {
        this.$emit("emitLayout", { left: true, right: true });
      }
    },
  },
};
</script>

<style scoped>
.navbar {
  max-width: 80px;
  background: black;
  min-height: 100vh;
}
</style>
