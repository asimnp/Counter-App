<template>
  <h1>Counter App</h1>
  <h3>Counter: {{ counter }}</h3>
  <button @click="increment">Increment</button>
  <button @click="decrement">Decrement</button>
  <button @click="reset">Reset</button>
</template>

<script>
export default {
  data() {
    return {
      counter: 0,
    };
  },
  methods: {
    increment() {
      this.counter += 1;
    },
    decrement() {
      this.counter -= 1;
    },
    reset() {
      this.counter = 0;
    },
  },
};
</script>
