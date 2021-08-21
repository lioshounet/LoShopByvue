<template>
  <div class="list">
    <!-- 修改标志 -->
    <div class="til">种类</div>
    <ul>
      <li @click="missjane()">珍妮小姐</li>
      <li @click="autumnforest()">秋日森林</li>
      <li @click="honeyhoney()">Honeyhoney</li>
      <li @click="arconasdream()">阿尔可纳之梦</li>
      <li @click="badoni()">巴朵妮</li>
      <li @click="brokendoll()">崩坏人偶</li>
      <li @click="pandabamboo()">熊猫梦竹</li>
      <li @click="anthonycake()">安东尼蛋糕</li>
      <li @click="aprilamwell()">四月安</li>
      <li @click="lancelot()">兰斯洛特</li>
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
    honeyhoney: function () {
      Msg.$emit("showwhat", "honeyhoney");
    },
    arconasdream: function () {
      Msg.$emit("showwhat", "arconasdream");
    },
    badoni: function () {
      Msg.$emit("showwhat", "badoni");
    },
    brokendoll: function () {
      Msg.$emit("showwhat", "brokendoll");
    },
    pandabamboo: function () {
      Msg.$emit("showwhat", "pandabamboo");
    },
    anthonycake: function () {
      Msg.$emit("showwhat", "anthonycake");
    },
    aprilamwell: function () {
      Msg.$emit("showwhat", "aprilamwell");
    },
    lancelot: function () {
      Msg.$emit("showwhat", "lancelot");
    },
  },
};
</script>