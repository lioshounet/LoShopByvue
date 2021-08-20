<template>
  <div>
    <div class="goods" v-if="xi == 'missjane' || xi == ''">
      <div class="til">
        <p>货架</p>
      </div>
      <missjane></missjane>
    </div>
    <div class="goods" v-if="xi == 'autumnforest'">
      <div class="til">
        <p>货架</p>
      </div>
      <autumnforest></autumnforest>
    </div>
    <div class="goods" v-if="xi == 'honeyhoney'">
      <div class="til">
        <p>货架</p>
      </div>
      <honeyhoney></honeyhoney>
    </div>
    <div class="goods" v-if="xi == 'arconasdream'">
      <div class="til">
        <p>货架</p>
      </div>
      <arconasdream></arconasdream>
    </div>
    <div class="goods" v-if="xi == 'badoni'">
      <div class="til">
        <p>货架</p>
      </div>
      <badoni></badoni>
    </div>
    <div class="goods" v-if="xi == 'brokendoll'">
      <div class="til">
        <p>货架</p>
      </div>
      <brokendoll></brokendoll>
    </div>
    <div class="goods" v-if="xi == 'pandabamboo'">
      <div class="til">
        <p>货架</p>
      </div>
      <pandabamboo></pandabamboo>
    </div>
    <div class="goods" v-if="xi == 'anthonycake'">
      <div class="til">
        <p>货架</p>
      </div>
      <anthonycake></anthonycake>
    </div>
    <div class="goods" v-if="xi == 'aprilamwell'">
      <div class="til">
        <p>货架</p>
      </div>
      <aprilamwell></aprilamwell>
    </div>
    <div class="goods" v-if="xi == 'lancelot'">
      <div class="til">
        <p>货架</p>
      </div>
      <lancelot></lancelot>
    </div>
  </div>
</template>
<style>
@import "../../public/css/goods.css";
</style>
<script>
import missjane from "./sheets/missjane_sheets.vue";
import autumnforest from "./sheets/autumnforest_sheets.vue";
import honeyhoney from "./sheets/honeyhoney_sheets.vue";
import arconasdream from "./sheets/arconasdream_sheets.vue";
import badoni from "./sheets/badoni_sheets.vue";
import brokendoll from "./sheets/brokendoll_sheets.vue";
import pandabamboo from "./sheets/pandabamboo_sheets.vue";
import anthonycake from "./sheets/anthonycake_sheets.vue";
import aprilamwell from "./sheets/aprilamwell_sheets.vue";
import lancelot from "./sheets/lancelot_sheets.vue";
import Msg from "./msg.js";
export default {
  // name: "DollMissJane",
  components: {
    missjane,
    autumnforest,
    honeyhoney,
    arconasdream,
    badoni,
    brokendoll,
    pandabamboo,
    anthonycake,
    aprilamwell,
    lancelot,
  },

  // directives: { DirectiveName },

  data() {
    return {
      xi: "",
    };
  },

  mounted() {
    var _this = this;
    Msg.$on("showwhat", function (m) {
      _this.xi = m;
    });
  },

  methods: {},
};
</script>