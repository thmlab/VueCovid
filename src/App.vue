<template>
  <div class="container" id="app">
    <h2 class="website">戴伟健的个人网站</h2>
    <hr/>
    <div id="nav">
      <router-link to="./">首页</router-link> |
      <router-link to="./personal">个人信息</router-link> |
      <router-link to="./about">疫情实时数据</router-link> |
      <router-link to="./baoxiao">报销系统</router-link>
    </div>
    <hr/>
    <router-view/>
     <footer class="site-info">
      <span>粤ICP备20051750号-1</span>
  </footer>
  </div>
</template>

<style>

#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #2c3e50;
}

#nav {
  padding: 0px 0px 0 30px;
  text-align: left;;
}

#nav a {
  font-weight: bold;
  color: #2c3e50;
}

#nav a.router-link-exact-active {
  color: #42b983;
}
.site-info{
  margin-top: 0;
  text-align: center;
  padding-top: 10%;
}
.website{
  padding: 30px 0 0 0;
  border-bottom: none;
}
hr{
  padding: 0;
}
</style>
