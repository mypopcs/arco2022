# app

## Project setup
```
yarn install
```

### Compiles and hot-reloads for development
```
yarn serve
```

### Compiles and minifies for production
```
yarn build
```

### Lints and fixes files
```
yarn lint
```

### Customize configuration
See [Configuration Reference](https://cli.vuejs.org/config/).

## CloudStudio提示Invalid Host header
在运行的项目目录下面新建 vue.config.js，并添加以下内容：
```
module.exports = {
    devServer: {
        disableHostCheck: true,
    }
}
```
# main.js 中 完整引入Arco Design
```
import { createApp } from 'vue'
import ArcoVue from '@arco-design/web-vue';
import App from './App.vue';
import '@arco-design/web-vue/dist/arco.css';

const app = createApp(App);
app.use(ArcoVue);
app.mount('#app');
```
引入完成后默认不会显示效果，按照官网教程引用各组件才会显示效果