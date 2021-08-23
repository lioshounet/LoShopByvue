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
    var url = "";
    // url = "json/good_anthonycake.json";
    url = "json/good_" + _this.goodId + ".json";
    this.$http.get(url).then(function (res) {
      _this.list = res.data;
    });
    // console.log(list);
    return {
      list: [],
    };
  },
  props: {
    goodId: String,
  },

  watch: {
    goodId() {
      var _this = this;
      var url = "";
      url = "json/good_" + _this.goodId + ".json";
      this.$http.get(url).then(function (res) {
        _this.list = res.data;
      });

      return {
        list: [],
      };
    },
  },

  mounted() {},

  methods: {},
};
// console.log(list);
</script>