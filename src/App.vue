<template>
  <div id="app" class="add">
    <button v-on:click="incrementNumber">⬆︎</button>
    <input v-model="number" />
    <Calculate :data="Array.from({ length: number }, (v, i) => 10 + i)" />
  </div>
</template>

<script>
import Calculate from "./components/Calculate.vue";

export default {
  name: "App",
  components: {
    Calculate,
  },
  data() {
    return {
      number: 5,
    };
  },
  methods: {
    incrementNumber() {
      this.number++;
    },
  },
};
</script>

<style>
div {
  box-sizing: border-box;
  color: rgb(36, 41, 46);
  display: block;
  font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Helvetica, Arial,
    sans-serif, "Apple Color Emoji", "Segoe UI Emoji", "Segoe UI Symbol";
  font-size: 16px;
  height: 600px;
  line-height: 24px;
  margin-bottom: 32px;
  margin-left: 340px;
  margin-right: 340px;
  margin-top: 32px;
  max-width: 1012px;
  padding-left: 16px;
  padding-right: 16px;
  width: 1012px;
}
button {
  background-color: rgb(192, 192, 192);
  font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Helvetica, Arial,
    sans-serif, "Apple Color Emoji", "Segoe UI Emoji", "Segoe UI Symbol";
  height: 35px;
  width: 35px;
  margin-left: 350px;
  margin-right: 10px;
}
input {
  background-color: rgb(255, 255, 255);
  border-width: 2px 2px;
  color: rgb(0, 0, 0);
  font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Helvetica, Arial,
    sans-serif, "Apple Color Emoji", "Segoe UI Emoji", "Segoe UI Symbol";
  font-size: 16px;
  height: 29px;
  width: 200px;
}
</style>

