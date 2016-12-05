# 第一章：AngularJS 简介

<img src="../img/angelababy.jpg" width="200" alt="angelababy">
<img src="../img/AngularJS-large.png" alt="AngularJS">

**AngularJS，程序员的 angelababy**

以下简称：`ng`

## 知识储备

- HTML
- CSS
- JavaScript

为了更好的学习效果，最好擅长一些 JavaScript 库，如果有后台开发经验效果最佳。

## 哪些人在用

- 前端开发人员
- 后端开发人员目前更多

## What is AngularJS

<img src="../img/baike-ng.png" width="500" alt="">

## 什么是 AngularJS

- 一款非常优秀的前端高级 **JavaScript 框架**
- 2009 年起先由 Miško Hevery 和Adam Abron 开发
- 后被 Google 收购，用于其多款产品
- 有一个全职的开发团队继续开发和维护这个库
- 可以轻松构建 **SPA 应用程序**
- 通过 **指令** 扩展了 HTML，通过 **表达式** 绑定数据到 HTML
- **最大程度上解放了 DOM 操作**
- 构建更加动感的 HTML 应用程序

AngularJS是为了克服HTML在构建应用上的不足而设计的。
AngularJS有着诸多特性，最为核心的是：

- MVC
- 模块化
- 自动化双向数据绑定
- 语义化标签、依赖注入等等

---

## 为什么使用 Angular(演示 Demo 中的 compare)

以前我们是这样的：

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>传统页面操作数据操作方式</title>
</head>
<body>
  <input id="txt_value" type="number">
  <input id="btn_add" type="button" value="增加">
  <script>
    (function(window, document) {
      var txt = document.querySelector('#txt_value');
      var btn = document.querySelector('#btn_add');
      btn.addEventListener('click', function(e) {
        var now = txt.value - 0;
        now = now + 1;
        txt.value = now;
      });
    })(window, document);
  </script>
</body>
</html>
```

以后将会是这样的：

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>使用AngularJS实现自增功能</title>
</head>
<body ng-app>
  <input type="number" ng-model="value">
  <input type="button" ng-click="value=value+1" value="增加">
  <script src="../bower_components/angular/angular.js"></script>
</body>
</html>
```

- 更少的代码，实现更强劲的功能，当然不仅仅是这些，这些只是皮毛
- 背后带来的价值才是巨大的
- 带领前端进入了 MV* 的时代
- 又是一场革命，Angular 引领了前端工业革命
  + 从 Angular 2009 年之后，前端市场越来越火爆了

---

## 项目案例演示

- TODOList
- 豆瓣电影列表

---

## AngularJS 优缺点

优点：

1. AngularJS模板功能强大丰富，自带了极其丰富的angular指令。
2. AngularJS是完全可扩展的，与其他库的兼容效果很好，每一个功能可以修改或更换，以满足开发者独特的开发流程和功能的需求。
3. AngularJS是一个比较完善的前端MVC框架，包含服务，模板，数据双向绑定，模块化，路由，过滤器，依赖注入等所有功能；
4. AngularJS是互联网巨人谷歌开发，这也意味着他有一个坚实的基础和社区支持。

缺点：

1. AngularJS强约束导致学习成本较高，对前端不友好。但遵守 AngularJS 的约定时，生产力会很高，对 后台服务器开发程序员友好。
2. AngularJS不利于SEO，因为所有内容都是动态获取并渲染生成的，搜索引擎没法爬取。
3. AngularJS作为 MVVM 框架，因为实现了数据的双向绑定，对于大数组、复杂对象会存在性能问题。

---

## AngularJS 使用场景

- 单页面应用程序
- 复杂的后台管理系统
  + CRUD（增加 Create、查询 Retrieve、更新 Update、删除 Delete）
  + 繁杂的 DOM 操作处理的页面

Angular 是一个类 MVC 类结构的 JavaScript 框架，建议构建 CRUD 类型应用的时候使用它，
而对于那些图形编辑、游戏开发等应用，使用 Angular 就不如调用其它 JavaScript 类库方便，
如 jQuery。

---

## 学习资源推荐

- 菜鸟教程：http://www.runoob.com/angularjs/angularjs-tutorial.html
- AngularJS 中文社区：http://angularjs.cn/
- 官方文档：https://docs.angularjs.org/api
- AngularJS 权威教程
- AngularJS 深度剖析与最佳实践
- [AngularJS入门教程](http://www.ituring.com.cn/minibook/303)
- [七步从Angular.JS菜鸟到专家](http://blog.jobbole.com/46779/)
