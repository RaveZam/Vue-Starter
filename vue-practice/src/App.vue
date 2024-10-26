<template>
  <Header />
  <div>
    <h1>Hello</h1>
    <h1>{{ counter }}</h1>
    <button @click="decrementValue">Click</button> <br />
    <button @click="logHelloMessage">Click</button>
  </div>
</template>

<script lang="ts">
import { defineComponent } from "vue";
import Header from "./components/Header.vue";

export default defineComponent({
  components: {
    Header,
  },

  data() {
    return {
      counter: 0,
    };
  },

  methods: {
    decrementValue(): void {
      if (this.counter > 0) {
        this.counter--;
      } else {
        null;
      }
    },

    logHelloMessage(): void {
      this.counter++;
    },
  },
});
</script>
