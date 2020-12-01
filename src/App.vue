<template>
  <Counter :count="count" />
  <button @click="increment">add more</button>
  <button @click="decrement">decrease more</button>
</template>

<script>
import Counter from "./components/Counter.vue";

export default {
  name: "App",
  components: {
    Counter: Counter,
  },
  data() {
    return { count: 0 };
  },
  created() {
    this.count = this.count + 5;
  },

  methods: {
    increment() {
      this.count = this.count + this.factor;
    },
    decrement() {
      this.count--;
    },
  },
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
