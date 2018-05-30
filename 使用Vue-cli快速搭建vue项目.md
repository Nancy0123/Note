1.安装vue-cli ：npm install -g vue-cli
2.创建项目：vue init webpack XX  （请确保安装了webpack）
3.开发模式的文件在src目录下，进入文件后，打开package.json ,查看配置信息
4.安装项目需要的依赖包:cnpm install (or npm install) 
5.安装好后，运行npm run dev (以开发环境 | 热加载运行)：热加载可以让我们在修改完代码后不用手动刷新浏览器就能实时看到修改后的效果。


这里简单介绍下 npm run dev 命令，其中的“run”对应的是package.json文件中，scripts字段中的dev，也就是 node build/dev-server.js命令的一个快捷方式。

项目运行成功后，浏览器会自动打开localhost:8080（如果浏览器没有自动打开，可以手动输入）。运行成功后，会看到如下所示的界面

以后如果自己写的项目，也可以通过这种方式进行开发！至于进行单元测试，以及打包（npm run build）可自行百度深入了解
