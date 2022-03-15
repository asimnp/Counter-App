<template>
  <h1>Counter App</h1>
  <h3>Counter: {{ counter }}</h3>
  <Button name="Increment" :handle="increment" />
  <Button name="Decrement" :handle="decrement" />
  <Button name="Reset" :handle="reset" />
</template>

<script>
import Button from "./components/Button.vue";

export default {
  data() {
    return {
      counter: 0,
    };
  },
  components: {
    Button,
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
