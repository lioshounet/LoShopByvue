<template>
  <div id="app" class="main">
    <div class="left_box">
      <List></List>
    </div>
    <div class="right_box">
      <div class="top">
        <img
          src="../public/img/main/best_sell/小熊你好.png"
          alt=""
          width="980px"
        />
      </div>
    </div>
  </div>
</template>

<style>
@import "../public/css/base.css";
@import "../public/css/app.css";

#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

#nav {
  padding: 30px;
}

#nav a {
  font-weight: bold;
  color: #2c3e50;
}

#nav a.router-link-exact-active {
  color: #42b983;
}
</style>

<script>
import List from "./components/List";
export default {
  components: { List },
};
</script>
