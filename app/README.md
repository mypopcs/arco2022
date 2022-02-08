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