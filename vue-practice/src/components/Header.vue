<template>
  <div class="bg-gray-500 w-screen h-[10vh]">
    <h1 class="font-lg">This is the header</h1>
  </div>
</template>

<script lang="ts">
import { defineComponent } from "vue";
export default defineComponent({
  name: "Header",
  data() {
    return {
      firstNumber: 0,
      secondNumber: 0,
    };
  },
});
</script>
