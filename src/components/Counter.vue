<template>
  <div>{{ count }}</div>
</template>

<script>
export default {
  name: "Counter",
  props: {
    count: Number,
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
