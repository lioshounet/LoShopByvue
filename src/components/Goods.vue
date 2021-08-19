<template>
  <div>
    <div class="goods" v-if="xi == 'missjane' || xi == ''">
      <div class="til">
        <p>货架</p>
      </div>
      <missjane></missjane>
    </div>
    <div class="goods" v-if="xi == 'autumnforest'">
      <div>
        <div class="til"><p>货架</p></div>
        <div class="sheet">
          <div class="good">
            <img
              src="../../public/img/goods/【原创】秋冬森林小红帽lolita新年红洛丽塔可爱斗篷绑带少女OP连衣裙.png"
              alt=""
              width="225px"
            />
            <p>【原创】秋冬森林小红帽lolita新年红洛丽塔OP连衣裙</p>
            <p>$666</p>
          </div>
          <div class="good">
            <img
              src="../../public/img/goods/【原创】秋冬森林小红帽lolita新年红洛丽塔可爱斗篷绑带少女OP连衣裙.png"
              alt=""
              width="225px"
            />
            <p>【原创】秋冬森林小红帽lolita新年红洛丽塔OP连衣裙</p>
            <p>$666</p>
          </div>
          <div class="good">
            <img
              src="../../public/img/goods/【原创】秋冬森林小红帽lolita新年红洛丽塔可爱斗篷绑带少女OP连衣裙.png"
              alt=""
              width="225px"
            />
            <p>【原创】秋冬森林小红帽lolita新年红洛丽塔OP连衣裙</p>
            <p>$666</p>
          </div>
          <div class="good">
            <img
              src="../../public/img/goods/【原创】秋冬森林小红帽lolita新年红洛丽塔可爱斗篷绑带少女OP连衣裙.png"
              alt=""
              width="225px"
            />
            <p>【原创】秋冬森林小红帽lolita新年红洛丽塔OP连衣裙</p>
            <p>$666</p>
          </div>
        </div>
        <div class="sheet">
          <div class="good">
            <img
              src="../../public/img/goods/【原创】秋冬森林小红帽lolita新年红洛丽塔可爱斗篷绑带少女OP连衣裙.png"
              alt=""
              width="225px"
            />
            <p>【原创】秋冬森林小红帽lolita新年红洛丽塔OP连衣裙</p>
            <p>$666</p>
          </div>
          <div class="good">
            <img
              src="../../public/img/goods/【原创】秋冬森林小红帽lolita新年红洛丽塔可爱斗篷绑带少女OP连衣裙.png"
              alt=""
              width="225px"
            />
            <p>【原创】秋冬森林小红帽lolita新年红洛丽塔OP连衣裙</p>
            <p>$666</p>
          </div>
          <div class="good">
            <img
              src="../../public/img/goods/【原创】秋冬森林小红帽lolita新年红洛丽塔可爱斗篷绑带少女OP连衣裙.png"
              alt=""
              width="225px"
            />
            <p>【原创】秋冬森林小红帽lolita新年红洛丽塔OP连衣裙</p>
            <p>$666</p>
          </div>
          <div class="good">
            <img
              src="../../public/img/goods/【原创】秋冬森林小红帽lolita新年红洛丽塔可爱斗篷绑带少女OP连衣裙.png"
              alt=""
              width="225px"
            />
            <p>【原创】秋冬森林小红帽lolita新年红洛丽塔OP连衣裙</p>
            <p>$666</p>
          </div>
        </div>
        <div class="sheet">
          <div class="good">
            <img
              src="../../public/img/goods/【原创】秋冬森林小红帽lolita新年红洛丽塔可爱斗篷绑带少女OP连衣裙.png"
              alt=""
              width="225px"
            />
            <p>【原创】秋冬森林小红帽lolita新年红洛丽塔OP连衣裙</p>
            <p>$666</p>
          </div>
          <div class="good">
            <img
              src="../../public/img/goods/【原创】秋冬森林小红帽lolita新年红洛丽塔可爱斗篷绑带少女OP连衣裙.png"
              alt=""
              width="225px"
            />
            <p>【原创】秋冬森林小红帽lolita新年红洛丽塔OP连衣裙</p>
            <p>$666</p>
          </div>
          <div class="good">
            <img
              src="../../public/img/goods/【原创】秋冬森林小红帽lolita新年红洛丽塔可爱斗篷绑带少女OP连衣裙.png"
              alt=""
              width="225px"
            />
            <p>【原创】秋冬森林小红帽lolita新年红洛丽塔OP连衣裙</p>
            <p>$666</p>
          </div>
          <div class="good">
            <img
              src="../../public/img/goods/【原创】秋冬森林小红帽lolita新年红洛丽塔可爱斗篷绑带少女OP连衣裙.png"
              alt=""
              width="225px"
            />
            <p>【原创】秋冬森林小红帽lolita新年红洛丽塔OP连衣裙</p>
            <p>$666</p>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>
<style>
@import "../../public/css/goods.css";
</style>
<script>
import missjane from "./sheets/missjane_sheets.vue";
import Msg from "./msg.js";
export default {
  // name: "DollMissJane",
  components: { missjane },

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