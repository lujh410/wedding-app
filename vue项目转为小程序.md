vue项目转为小程序
一.mpvue介绍

mpvue:是由美团点评团队出品的小程序开发的一款基于vue的框架，从整个Vue的核心代码上经过二次开发而形成的一个框架，相当于是给Vue本身赋能，增加了开发微信小程序的能力。

二.mpvue开发流程

1、小程序账号配置

1）前往https://mp.weixin.qq.com/wxopen/waregister?action=step1根据指引填写信息和提交相应的资料，申请小程序帐号。在菜单 “设置”-“开发设置”获取小程序的 AppID 。

2）在菜单 “设置”-“开发设置”中配置服务器域名，必须是https开头的域名

 

2、安装开发工具

前往 开发者工具下载页面 ，根据自己的操作系统下载对应的安装包进行安装，有关开发者工具更详细的介绍可以查看 《开发者工具介绍》 。

 

打开小程序开发者工具，用微信扫码登录开发者工具，准备开发小程序。

3、mpvue生成项目

# 全局安装 vue-cli

$ npm install --global vue-cli

 

# 创建一个基于 mpvue-quickstart 模板的新项目

$ vue init mpvue/mpvue-quickstart my-project

 

# 安装依赖

$ cd my-project

$ npm install

# 启动构建

$ npm run dev

 

Npm run dev运行成功后，本地目录下会生成一个dist文件，这个文件就是生成的小程序相关代码。

在小程序中新建项目，填写上一步获取的appid，便于后面可以在手机上预览，真机测试，小程序的文件目录就是本地项目目录的dist文件。
