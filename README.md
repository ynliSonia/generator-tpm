# 突破前端脚手架（基础版）

这是一个比较基础的脚手架，可以生成开发所需要的目录结构，使用方法如下。

## 背景

可以快速生成开发所需的目录结构

## 介绍


目录结构

```
├── build
├── demo
│   └── index.html
├── src
│   ├── c
│   │	 └── lib
│   └── p
│   	 └── index
│  			  ├── index.js
│   		  └── index.less
├── package.json
├── README.md
└── gulpfile.js
```
## 使用方法

1. install npm

```
// install npm 
npm install -g yo
npm install -g generator-tpm

```

2. init

```
yo tpm
```

## 目录文件介绍

* build

  build 文件用来存放打包压缩后的文件，也是最后的线上版本。

* src

  开发文件，未打包未压缩的代码，用于本地开发与调试
  
* demo

  页面的静态模板，用于本地开发与调试
  
* gulpfile.js

  代码的打包压缩
  
* package.json

  包管理文件
  
* dev

  打包未压缩文件，默认不会提交
  
  
## 生成目录结构后如何开发

在生成目录结构后要投入开发需要怎么做？

- 执行相应的命令打包编译文件。最新版已经支持代码修改后页面的自动刷新，修改 less 时页面无刷新修改。去除了之前的dev 命令，watch 即可以实现自动起服务器的功能。

```
// 手动打包
  gulp

// 实现自动打包(推荐)
  gulp watch
```
 - js 开发

 类似于 node 的开发方式
 
 - less

 可以自动编译，无需手动操作

