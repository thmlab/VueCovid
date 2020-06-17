<template>
  <div class="container">
    <div class="about">
    <h1 class="abouth1">国内新型冠状病毒实时数据</h1>
    <div class="BOX">
      <div class="box-1s">
         <img class="aboutimg" src="../assets/imgs/backg3.jpeg"/>
      </div>
    </div>

    <div class="Tab">
      <div id="Tabs" class="Tab-header">
        <div class="TabOn" @click="cur=0" :class="{active:cur==1}">
          <h3>国内疫情</h3>
        </div>

        <div class="TabOff" @click="cur=1" :class="{active:cur==0}">
          <h3>国外疫情</h3>
        </div>
      </div>

      <div class="Text-box">
        <div class="Text active" v-show="cur==0">
          <table>
            <tbody class="tableone" v-if="info.data">
              <tr v-for="(data,index) in info.data[0]" :key="index" >
                  <td v-for="i in data" :key="i">
                    {{i}}
                </td>
              </tr>
            </tbody>
          </table>
          <div class="time" v-if="info.data">
              {{info.data[2]}}
          </div>
        </div>

        <div class="Text active" v-show="cur==1">
          <table class="globaltable">
            <tbody class="tabletwo" v-if="info.data">
              <tr v-for="(data,index) in info.data[1]" :key="index">
                  <td v-for="i in data" :key="i">
                    {{i}}
                </td>
              </tr>
            </tbody>
          </table>
          <div class="time" v-if="info.data">
              {{info.data[2]}}
          </div>
        </div>
        
      </div>
    </div>
  </div>
  </div>
</template>



<script>

export default {
  name: "About",
  data() {
    return {
      info: "",
      cur: 0
    };
  },
  mounted() {
    this.$axios
      .get("http://120.77.243.252:8888/")
      .then(response => (this.info = response))
      .catch(function(error) {
        // 请求失败处理
        console.log(error);
      });
  }
};
</script>

<style>
@import "../assets/css/about.css";
</style>

