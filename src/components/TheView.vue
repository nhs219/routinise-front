<template>
  <main class="content">
    <MainCalendar></MainCalendar>
    <MainRoutine></MainRoutine>
    <button class="add-button" @click="onAddClick">+</button>
  </main>
</template>
<script>

import MainCalendar from "@/components/MainCalendar.vue";
import MainRoutine from "@/components/MainRoutine.vue";

export default {
  components: {
    MainRoutine,
    MainCalendar,
  },
}
</script>

<style scoped>
main.content {
  flex: 1 0 auto;
  overflow-y: auto;
  padding-bottom: 60px; /* to prevent content from being hidden under the footer */
}

.add-button {
  position: fixed;
  right: 10%;
  width: 60px;
  height: 60px;
  border-radius: 50%;
  background-color: #007bff;
  color: white;
  border: none;
  font-size: 30px;
  display: flex;
  align-items: center;
  justify-content: center;
  box-shadow: 0 2px 10px rgba(0, 0, 0, 0.1);
}

.add-button:hover {
  background-color: #0056b3;
}
</style>