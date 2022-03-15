<template>
  <button @click="handle">{{ name }}</button>
</template>

<script>
export default {
  props: {
    name: {
      type: String,
      required: true,
    },
    handle: {
      type: Function,
      required: true,
    },
  },
};
</script>
