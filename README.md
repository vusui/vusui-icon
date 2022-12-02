# Vusui-icon 图标库

一套集成了 500+ 个常用图标的字体图标库。

【[使用文档](https://www.vusui.com/icon)】|【[在线预览](https://www.vusui.com/icon/docs/guide/demo.html)】

## 使用包管理器

```sh
# 选择一个你喜欢的包管理器

# yarn
$ yarn add @vusui/icon

# npm
$ npm install @vusui/icon --save

# pnpm
$ pnpm install @vusui/icon
```

## 全局使用

```ts
// main.ts
import { createApp } from "vue";

// 引入图标库
import "@vusui/icon/font/index.css";

// 或者引入svg格式图标库
import "@vusui/icon/svg";
import "@vusui/icon/svg/style.css";

const app = createApp({});
app.mount("#app");
```

## 浏览器直接引入

直接通过浏览器的 HTML 标签导入 vusui-icon，然后就可以使用 Vusui-icon 图标库了。

根据不同的 CDN 提供商有不同的引入方式， 我们在这里以 [unpkg](https://unpkg.com/) 和 [jsDelivr](https://www.jsdelivr.com/) 举例。

### unpkg

```html
<head>
  <!-- 引入图标库 -->
  <link rel="stylesheet" href="//unpkg.com/@vusui/icon/font/index.css" />
  <!-- 或者使用svg格式的图标库 -->
  <link rel="stylesheet" href="//unpkg.com/@vusui/icon/svg/style.css" />
  <script src="//unpkg.com/@vusui/icon/svg"></script>
</head>
```

### jsDelivr

```html
<head>
  <!-- 引入图标库 -->
  <link
    rel="stylesheet"
    href="//cdn.jsdelivr.net/npm/@vusui/icon/font/index.css"
  />
  <!-- 或者使用svg格式的图标库 -->
  <link
    rel="stylesheet"
    href="//cdn.jsdelivr.net/npm/@vusui/icon/svg/style.css"
  />
  <script src="//cdn.jsdelivr.net/npm/@vusui/icon/svg"></script>
</head>
```

## Unicode

```vue
<!--Unicode 引用方法-->
<template>
  <i class="vusuiIcon">&#xedbd;</i>
</template>

<script>
import "@vusui/icon/font/index.css";
</script>
```

## Font Class

```vue
<!--class 样式引用方法-->
<template>
  <i class="vi-home"></i>
</template>

<script>
import "@vusui/icon/font/index.css";
</script>
```

## Symbol

💡 使用 svg 图标时，建议封装成公共组件来调用。

```vue
<!--svg 引用方法-->
<template>
  <svg class="vusuiSvg" aria-hidden="true">
    <use xlink:href="#vi-home"></use>
  </svg>
</template>

<script>
import "@vusui/icon/svg";
import "@vusui/icon/svg/style.css";
</script>
```
