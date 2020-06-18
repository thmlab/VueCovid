<template>
  <div id="app">
    <div id="nav">
      <router-link to="./">首页</router-link> |
      <router-link to="./personal">个人信息</router-link> |
      <router-link to="./about">实时数据</router-link>
      <hr/>
    </div>
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
  padding: 30px;
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
</style>
