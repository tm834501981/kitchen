<template>
  <div id="app">
    <div class="navborder">
      <div class="nav">
        <div class="logo">
          <img src="http://www.tminlife.cn/kitchenimages/logo.png" alt="">
        </div>
        <div class="serachBtn">
          <input type="text" placeholder="搜索菜谱、食材">
          <button>搜菜谱</button>
        </div>
        <div class="navList">
          <router-link to="/index">首页</router-link>
          <router-link to="/index">菜谱分类</router-link>
          <router-link to="/index">菜单</router-link>
          <router-link to="/index">作品状态</router-link>
        </div>
        <div class="avatar">
          <img src="http://www.tminlife.cn/kitchenimages/avatar.jpg" alt="">
        </div>
        <font-awesome-icon icon="coffee" />
      </div>
    </div>
    <router-view/>
  </div>
</template>

<script>
export default {
  name: 'App'
}
</script>

<style>
* {
  margin: 0;
  padding: 0;
}
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}
.nav {
  display: flex;
  justify-content: space-between;
  width:900px;
  margin:20px auto;
}
.navborder {
  border-bottom: 1px solid #f3f3f3;
}
.logo img{
  width:120px;
}
.navList {
  display: flex;
  justify-content: space-between;
}
.serachBtn {
  position: relative;
}
.serachBtn input {
  width:300px;
  height:44px;
  border: 1px solid #f3f3f3;
  font-size:16px;
  text-indent:10px;
}
.serachBtn input:focus {
  outline: none;
}
.serachBtn button {
  height:44px;
  text-align: center;
  font-size: 15px;
  color: #fff;
  background-color: #dd3915;
  border: none;
  width:80px;
  position:absolute;
  right:-75px;
  top:0;
}
.navList {
  margin-left: 50px;;
}
.navList a{
  font-size:16px;
  color:#dd3915;
  text-decoration: none;
  margin: 12px 10px;
}
.avatar {
  height: 44px;
}
.avatar img{
  width:30px;
  border-radius: 50%;
  margin-top: 7px;
}
.navList a:hover {
  background: #dd3915;
  color:#fff;
}
</style>
