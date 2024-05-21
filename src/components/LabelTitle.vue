<template>
  <label>
    {{ label }}
    <input v-model="value" type="text"/>
  </label>
</template>

<script>

import {computed} from "@vue/reactivity";

export default {
  name: "LabelInput",
  props: ['title', 'label'],
  emits: ['update:title'],
  setup(props, {emit}) {
    const value = computed({
      get() {
        return props.title;
      },
      set(value) {
        emit('update:title', value);
      },
    });
    return { value };
  }
}
</script>

<style scoped>

</style>