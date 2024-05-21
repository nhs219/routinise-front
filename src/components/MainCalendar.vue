<template>
  <Calendar
      class="pt-3"
      :attributes="attrs"
      expanded borderless/>
</template>

<script>

import { Calendar } from 'v-calendar';
import 'v-calendar/style.css';
import {ref} from 'vue';

export default {
  components: {
    Calendar,
  },
  setup() {
    const attrs = ref([
      {
        key: 'today',
        highlight: {
          color: 'red',
          fillMode: 'outline',
        },
        dates: new Date(),
      },
    ]);
    return {
      attrs,
    };
  },
}
</script>

<style scoped>

</style>