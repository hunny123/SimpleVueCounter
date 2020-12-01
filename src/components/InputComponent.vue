<template>
  <input v-bind:value="value" v-on:change="onchangeMethod" />
</template>
<script>
export default {
  name: "InputComponent",
  props: {
    value: Number,
    onchangeMethod: Function,
  },
};
</script>