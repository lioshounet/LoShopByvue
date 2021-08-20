<template>
  <div class="sheet" name="sheet">
    <div class="good" v-for="good in list">
      <img v-bind:src="good.img" alt="" />
      <p>{{ good.goodName }}</p>
    </div>
  </div>
</template>
<style>
@import "../../../public/css/sheets.css";
</style>
<script>
// import Msg from "./msg.js";
export default {
  name: "sheet",
  data() {
    var _this = this;
    this.$http.get("json/good_anthonycake.json").then(function (res) {
      _this.list = res.data;
    });
    // console.log(list);
    return {
      list: [],
    };
  },

  mounted() {},

  methods: {},
};
// console.log(list);
</script>