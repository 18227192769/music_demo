# 基于gulp实现的音乐播放器

### 项目简介
- 这个demo是用zepto，配合基于工作流的前端工程化工具gulp实现的，整个demo用到了模块化和面向对象的思想。

- 由于使用的原生js，并且没有使用es6语法，因此模块化是使用IIFE实现的(jQuery的封装思想)。

### src/js
- index.js：功能逻辑的主入口文件。

- audioControl.js：对播放器实例的封装，对外提供了创建播放器实例的构造器(AudioPlayer)，实例原型上封装了三个功能函数(音乐的播放，暂停和加载)。

- indexControl.js：封装音乐切换的控制器，该模块对外暴露了控制器实例(Control)，并提供了四个方法(切换上一首，下一首，跳转到指定索引，获取播放进度)。

- gaussBlur.js：第三方封装好的高斯模糊算法函数。

- render.js：渲染函数，主要的功能是渲染歌曲图片，信息，以及是否被收藏的状态。