#### 根据小程序的WXSS修改的TailwindCSS

1. 基于TailwindCSS 2.0.1版本；
2. 去掉了所有Variants： 比如```focus：``` ```hover：```等（在小程序中可以使用组件的属性实现，比如[button](https://developers.weixin.qq.com/miniprogram/dev/component/button.html)组件```hover-class```属性）；
3. 去掉了所有的media query: 比如```sm:``` ```md:```等（在小程序中可以使用[MediaMatch](https://developers.weixin.qq.com/miniprogram/dev/component/match-media.html )组件代替）；
4. 重命名了一些样式:
   - 小数点： 比如 ```1.2``` => ```1dot2```;
   - 斜杆： 比如 ```1/2```=> ```1on2```;

#### 用法（以Taro示意）

1. 将tailwind.css添加到项目中，在app.tsx 或 app.jsx中 ```import "../tailwind.css";```
2. 在vscode中安装插件```IntelliSense for CSS class names in HTML```即可实现样式名称的补全；



