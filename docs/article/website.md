# docsify 集成

### 脚手架方式

脚手架安装

```js
npm i docsify-cli -g
```

如果想在项目的 ./docs 目录里写文档，直接通过 init 初始化项目

```js
docsify init ./docs
```

初始化成功后，可以看到 ./docs 目录下创建的几个文件

1. index.html 入口文件
2. README.md 会做为主页内容渲染
3. .nojekyll 用于阻止 GitHub Pages 忽略掉下划线开头的文件

### 手动创建

如果不喜欢 npm 或者觉得安装工具太麻烦，我们可以直接手动创建一个 index.html 文件

```html
<!DOCTYPE html>
<html>
  <head>
    <meta http-equiv="X-UA-Compatible" content="IE=edge,chrome=1" />
    <meta name="viewport" content="width=device-width,initial-scale=1" />
    <meta charset="UTF-8" />
    <link
      rel="stylesheet"
      href="//cdn.jsdelivr.net/npm/docsify/themes/vue.css"
    />
  </head>
  <body>
    <div id="app"></div>
    <script>
      window.$docsify = {
        //...
      };
    </script>
    <script src="//cdn.jsdelivr.net/npm/docsify/lib/docsify.min.js"></script>
  </body>
</html>
```

- [详细参考官网](https://docsify.js.org/#/zh-cn/quickstart)

- [具体配置项](https://docsify.js.org/#/zh-cn/configuration)
