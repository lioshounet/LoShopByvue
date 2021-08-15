<template>
  <div class="list">
    <div class="til">种类</div>
    <ul>
      <li @click="missjane()">珍妮小姐</li>
      <li @click="autumnforest()">秋日森林</li>
      <li>789</li>
      <li>123</li>
      <li>456</li>
      <li>789</li>
      <li>456</li>
      <li>789</li>
      <li>123</li>
      <li>456</li>
      <li>789</li>
    </ul>
  </div>
</template>
<style>
@import "../../public/css/list.css";
</style>
<script type="text/javascript">
import Msg from "./msg";
export default {
  methods: {
    missjane: function () {
      Msg.$emit("showwhat", "missjane");
    },
    autumnforest: function () {
      Msg.$emit("showwhat", "autumnforest");
    },
  },
};
</script>