```
官网：https://cn.vuejs.org
```
```
依靠数据驱动
多用于pc端
是一套用于构建用户界面的渐进式框架
```
引入
```
<script>直接引入
①    <script src="vue.js"></script>
CDN(内容分发网络)引入
②    <script src="https://cdn.jsdelivr.net/npm/vue@2.5.17/dist/vue.js"></script>
NPM引入
③    $ npm install vue
```
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta http-equiv="X-UA-Compatible" content="ie=edge">
    <title>Document</title>
</head>
<body>
    <div id="app">
        {{msg}}
    </div>
    <script src="vue.js"></script>
    <script>
        let vm = new Vue({
            el:'#app',
            data:{
                msg:''
            }
        });
    </script>
</body>
</html>
```
