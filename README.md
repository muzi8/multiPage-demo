# demo

> A Vue.js project

## Build Setup

``` bash
# install dependencies
npm install

# serve with hot reload at localhost:8080
npm run dev

# build for production with minification
npm run build

# build for production and view the bundle analyzer report
npm run build --report
```

For a detailed explanation on how things work, check out the [guide](http://vuejs-templates.github.io/webpack/) and [docs for vue-loader](http://vuejs.github.io/vue-loader).

## just a demo
> 这个demo是用`vue-cli`生成，然后改编里面的`webpack`完成的，仅仅是添加了`home.html`、`src/home.js`、`src/Home.vue`（我这里的版本`vue 2.5.2 webpack 3.6.0`）

`npm run dev`之后，打开8080端口默认走的是`index.html`，也就是说`http://localhost:8080/`和`http://localhost:8080/index.html`显示的是一个，`http://localhost:8080/home.html`显示的就是增加的那个页面的。只需要改变地址就行。<br>
打包之后在`dist`目录下会出现两个html。一个`home.html`一个`index.html`，它们共用一个`static`文件夹的静态资源。<br>
【PS，特别提示一下，如果直接打包，可能会出现静态资源的引用路径问题，这个时候要修改`config/index.js`里`build`那一块中`assetsPublicPath`的值，将`/`改成`./`】