运行前需要安装的包：<br>
1. Vue-Cli4
2. node.js

检查是否安装：<br>
1. node: **$ node -v** <br>
2. Vue-cli: **$ vue --version** <br>

如未安装需要去命令行输入：<br>
node.js:  **$ yum install -y nodejs** (CentOs) https://nodejs.org/zh-cn/download/ (Windows & MacOs) <br>
Vue-Cli: **$ npm install -g @vue/cli** 或者 **$ yarn global add @vue/cli** <br>

Vue CLI 的包名称由 vue-cli 改成了 @vue/cli。 如果你已经全局安装了旧版本的 vue-cli (1.x 或 2.x)，你需要先通过 **$ npm uninstall vue-cli -g** 或 **$ yarn global remove vue-cli** 卸载它。<br>


安装完毕后：<br>
1. 进入目录
   **$ cd VueCovid**  <br>
1. 安装项目模组<br>
   **$ npm install**  或者  **$ yarn install**<br>

2. 启动服务器 <br>
   **$ npm run serve**  或者  **$ yarn serve**<br>

3. 打开浏览器输入 http://localhost:8080/<br>
