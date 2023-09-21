<template>
  <div>FullName: {{ fullName }}</div>
</template>

<script>
import { ref, computed } from "vue";

export default {
  setup() {
    const firstName = ref("Leonardo");
    const lastName = ref("Valdez");

    const fullName = computed(() => {
      return `${firstName.value} ${lastName.value}`;
    });

    return {
      fullName,
    };
  },
};
</script>
