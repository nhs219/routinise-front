<template>
  <div class="container">
    <TheNav></TheNav>
    <TheView></TheView>
  </div>
</template>

<script>
import TheNav from "@/components/TheNav";
import TheView from "@/components/TheView";
export default {
  components: {
    TheNav,
    TheView,
  },
  setup() {
    return {};
  },
}
</script>

<style scoped>
@import "@/assets/css/style.css";

</style>