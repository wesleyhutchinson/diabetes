<template>
  <v-row>
    <left class="layout" col="4"></left>
    <vertical-nav class="layout" col="2"></vertical-nav>
    <right class="layout" col="4"></right>
  </v-row>
</template>

<script>
import Left from "@/views/BaseLayouts/LeftView.vue";
import Right from "@/views/BaseLayouts/RightView.vue";
import VerticalNav from "@/components/VerticalNav.vue";
export default {
  components: [Left, Right, VerticalNav],
};
</script>

<style scoped>
.layout {
  height: 100vh;
}
</style>
