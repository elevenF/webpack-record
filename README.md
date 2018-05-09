# webpack学习小记

### webpack基本配置
``` npm init ``` 文件初始化

``` npm install webpack-cli --save-dev ``` 安装webpack

#### js文件编译
``` 
function hello (str) {
    alert(str)
}
```
``` webpack hello.js bundle.js ``` 将hello.js的文件编译到bundle.js中

#### css格式解析
``` npm install css-loader --save-dev ``` 安装css对应的loader

``` npm install style-loader --save-dev ``` 安装解析style对应的loader， **注：不安装html文件无法解析style样式**

hello.js文件中引入以下代码，并进行编译
``` 
require('style-loader!css-loader!./style.css') 
```
