<template>
  <div class="header">
    <div class="header-left">
      <div class="iconfont back-icon">&#xe666;</div>
    </div>
    <div class="header-input">
      <span class="iconfont">&#xe67d;</span>
      输入城市
    </div>
    <router-link to="/city">
      <div class="header-right">
        {{ this.city }}
        <span class="iconfont arrow-icon">&#xe688;</span>
      </div>
    </router-link>
  </div>
</template>

<script>
export default {
  name: "homeHeader",
  props: {
    city: String,
  },
};
</script>

<style lang="less" scoped>
@import "../../../assets/styles/varibles.less";
// @bdColor: #00bcd4;
.header {
  display: flex;
  line-height: @headerHeight;
  background: @bdColor;
  color: #fff;
  .header-left {
    width: 0.64rem;
    float: left;
    .back-icon {
      text-align: center;
      font-size: 0.4rem;
    }
  }
  .header-input {
    flex: 1;
    height: 0.64rem;
    line-height: 0.64rem;
    margin-top: 0.12rem;
    margin-left: 0.2rem;
    padding-left: 0.2rem;
    background: #fff;
    border-radius: 0.1rem;
    color: #ccc;
  }
  .header-right {
    width: 1.24rem;
    float: right;
    text-align: center;
    .arrow-icon {
      margin-left: -0.04rem;
      font-size: 0.24rem;
    }
  }
}
</style>