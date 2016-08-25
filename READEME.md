#流行框架第1天 构建自动化工作流环境

## 学习目标


- 了解什么是Node，什么是NPM；（Node.js）
- 掌握Npm的使用;
- 掌握Bower的使用；
- 使用Less/Sass；
- 搭建一个自己的自动化工作流环境；
  + 自动编译
  + 自动合并
  + 自动刷新
  + 自动部署
- GIT 与 GITHUB（就是一个网站）
  + master 托管源文件
  + 在github搭建自己的blog

- php 是一种语言，也是一个运行环境(php).

### 为什么要有自动化工作流程

### 前端存在了一些问题

## 1.Node

### 1.1.什么是Node
  - [官网](https://www.nodojs.org)
  - Node 本质就是一个js引擎.
  - chrome V8。
  - 最初 0.10.X 
  - node管理者是个追求完美的人.
  - IO.js,2015.
  - 4.x.x  发生了重大的变化
  - 4.x.1  
  - IO.js 5.0.0；
  - node == 4.x.x
  - IO.js == 5.x.x
    + 6.0.0


### 1.2.安装Node(windows)

#### REPL环境（控制台环境)

### 1.3.Node 入门
- cd -> change director
  + 切换到指定的目录
- 可以直接将js代码写在js文件中，然后通过
  + node 文件名  执行当前文件，需要把命令行路径切换到当前文件所在目录

- Ctrl+C *注意在命令行中这个快捷键不是复制,是终止当前命令的执行*
- cls 清除当前命令行中所有输出.
- 创建一个http服务
  1. 得到http对象
  2. 创建http服务
  3. 启动http服务

- get
- post

## 2.NPM

### 2.1.什么是NPM
 - node package manager
 - 方便的帮助我们管理node或前端的一些包文件
 - bootstrap,jquery
 - package.json.

### 2.1.为什么使用NPM

### 2.2.NPM 使用
  - 链接：
      + [官网](http://npmjs.com/)
  - 可以通过 npm -v 命令查看npm版本
  - 初始化package.json文件
    + 命令: `npm init`
      * 这个命令仅仅是创建了一个package.json文件，与我们手动新建一个package.json文件的效果是一样
  
  - 下载一个包文件
    + 命令: `npm install jquery`
    + 命令: `npm install bootstrap`
      * 会在当前目录生成一个node_modules的文件夹.
      * 本质就是帮助我们自动的把jquery或bootstrap 下载到本地
    + 一般在安装包文件时会加个`--save`
      * `npm install jquery --save`
    + 执行成功之后，命令行会看到类似树状结构的界面.
  - 卸载一个已经安装的包文件
    + 命令: `npm remove jquery`
    + 命令: `npm remove jquery --save`
  - 不仅仅能够安装前端的依赖包,还可以安装一些前端的工具.
    + 命令： 只需要把原来的包名改成工具的名字
          * `npm install gulp`
          * `npm install gulp --save-dev`
          * --save-dev 表示会把 当前安装的工具信息添加到开发依赖中：也就是会自动添加 devDependencies属性到package.json文件，并写入相关信息
  - 如果拿到的项目是通过npm来管理项目中的包文件，只需要得到一个package.json
  这个配置文件就可以了
    + 通过命令: `npm install` ,就会把package.json文件中配置的一些包文件或者工具自动的下载下来

  - 默认所有的包文件都会下载到package.json所在目录的node_modules目录的.
  - 
  
*****


## 3.Bower

### 3.1.什么是Bower
- 链接
    + [官网](http://bower.io/)

- npm install jquery --save
- bower install jquery --save

### 3.2.为什么使用Bower


### 3.3.Bower 安装
  - ` npm install  -g bower`
  - g   ==  global
*****

## 4.browser-sync

### 4.1.browser-sync 安装与使用
  - `npm  install -g  browser-sync --save-dev`
  - `browser-sync  --server    --files "./index.html,style.css" `
  - `browser-sync  --server    --files "./index.html,*.css" `

### browser-sync 可以与gulp 同用

*****

## 5.Gulp 
-  `npm install -g gulp-cli --save-dev`
-  

### 5.1.Gulp简介
- 链接：
    + [官网](http://gulpjs.com/)
    + [中文网](http://www.gulpjs.com.cn/)


### 5.2.Gulp准备工作
每一件事就是一个任务

### 5.3. Gulp的使用

### 常用Gulp插件

- [编译 Less：gulp-less](https://www.npmjs.com/package/gulp-less)
- [创建本地服务器：gulp-connect](https://www.npmjs.com/package/gulp-connect)
- [合并文件：gulp-concat](https://www.npmjs.com/package/gulp-concat)
- [最小化 js 文件：gulp-uglify](https://www.npmjs.com/package/gulp-uglify)
- [重命名文件：gulp-rename](https://www.npmjs.com/package/gulp-rename)
- [最小化 css 文件：gulp-minify-css](https://www.npmjs.com/package/gulp-minify-css)
- [压缩html文件 gulp-minify-html](https://www.npmjs.com/package/gulp-minify-html)
- [压缩html文件 gulp-htmlmin](https://www.npmjs.com/package/gulp-htmlmin)
- [最小化图像：gulp-imagemin](https://www.npmjs.com/package/gulp-imagemin)


### Markdown

### xx
[less中文网](http://lesscss.cn/)
