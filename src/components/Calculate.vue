<template>
  <div>
    <ul>
      <li v-for="item in data" :key="data[item]">
        <h1>
          <span>2</span><sup>{{ item }}</sup> = {{ 2 ** item }}
        </h1>
      </li>
    </ul>
  </div>
</template>

<script>
export default {
  name: "Calculate",
  props: {
    data: [Array],
  },
};
</script>


<style>
ul {
  box-sizing: border-box;
  color: rgb(36, 41, 46);
  display: block;
  font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Helvetica, Arial,
    sans-serif, "Apple Color Emoji", "Segoe UI Emoji", "Segoe UI Symbol";
  font-size: 16px;
  height: 420px;
  line-height: 24px;
  list-style-type: disc;
  margin-block-end: 16px;
  margin-bottom: 16px;
  margin-top: 0px;
  padding-inline-start: 32px;
  padding-left: 32px;
  width: 980px;
}
li {
  box-sizing: border-box;
  color: rgb(36, 41, 46);
  display: list-item;
  font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Helvetica, Arial,
    sans-serif, "Apple Color Emoji", "Segoe UI Emoji", "Segoe UI Symbol";
  font-size: 16px;
  height: 50px;
  line-height: 24px;
  list-style-type: disc;
  margin-top: 4px;
  text-align: left;
  width: 948px;
}
</style>