<template>
  <div class="bg-red-200">
    <h1 class="text-red-200">Hello</h1>
    <h1>{{ counter }}</h1>
    <button @click="logMessage">Click</button> <br />
    <button @click="logHelloMessage">Click</button>
  </div>
</template>

<script lang="ts">
import { defineComponent } from "vue";

export default defineComponent({
  data() {
    return {
      counter: 0,
    };
  },

  methods: {
    logMessage(): void {
      console.log("Button was pressed!");
    },

    logHelloMessage(): void {
      this.counter++;
    },
  },
});
</script>
