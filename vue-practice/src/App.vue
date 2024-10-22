<template>
  <div>
    <h1>Hello</h1>
    <button @click="logMessage">Click</button> <br />
    <button @click="logHelloMessage">Click</button>
  </div>
</template>

<script lang="ts">
import { defineComponent } from "vue";

export default defineComponent({
  methods: {
    logMessage(): void {
      console.log("Button was pressed!");
    },

    logHelloMessage(): void {
      console.log("Hello World");
    },
  },
});
</script>
