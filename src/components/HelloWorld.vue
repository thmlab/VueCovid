<template>
  <div class="hello">
    <h1>{{ msg }}</h1>
    <p>
      <br><br>
      实时数据页面是国内疫情和国外疫情的实时数据
    </p>
    <br><br>
    <p>
      数据爬虫于
      <a href="http://sa.sogou.com/new-weball/page/sgs/epidemic" target="_blank" rel="noopener">搜狗疫情实时动态</a>.
    </p>
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  props: {
    msg: String
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>
