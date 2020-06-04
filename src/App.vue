<template>
  <div class="app">
    <div class="mains">
      <router-view></router-view>
    </div>
    <div> HHHHHH </div>

    <div class="rou">
      
      <router-link to="/shouye"><van-icon name="wap-home" size="0.48rem"/>首页</router-link>
      <router-link to="/gouwuche"><van-icon name="cart-o" size="0.48rem"/>购物车</router-link>
      <router-link to="/weitao"><van-icon name="coupon-o" size="0.48rem"/>微淘</router-link>
      <router-link to="/wodetaobao"><van-icon name="friends-o" size="0.48rem"/>我的淘宝</router-link>
      <router-link to="/xiaoxi"><van-icon name="volume" size="0.48rem"/>消息</router-link>
      <router-link to="/abc">22</router-link>
    </div>
  </div>
</template>

<script>
import Vue from 'vue';
import { Button } from 'vant';
Vue.use(Button);

export default {
  components: {}
};
</script>

<style lang="scss">
* {
  padding: 0;
  margin: 0;
}
html,
body {
  width: 100%;
  height: 100%;
}
.app {
  width: 100%;
  height: 100%;
  position: relative;
  .mains {
    width: 100%;
  }
  .rou {
    position: fixed;
    left: 0;
    bottom: 0;
    width: 100%;
    font-size: .28rem;
    font-weight:900;
    display: flex;
    justify-content: space-around;
    align-items: center;
    height:1.2rem;
    background: #cccccc;;
    a {
      text-decoration: none;
      display: inline-block;
      color: #5d656b;
      font-size:0.3rem;
      font-weight: 900;
      display: flex;
      flex-direction: column;
      justify-content: center;
      align-items: center;
      box-sizing: border-box;
    }
  }
}
</style>
