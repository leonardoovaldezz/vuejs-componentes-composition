<template>
  <div>{{ counter }}</div>
</template>

<script>
import { ref } from "vue";

export default {
  setup() {
    const counter = ref(0);
    setInterval(() => counter.value++, 500)
    return { counter };
  },
};
</script>