# vue-cli-multipage

## Project setup
```
npm install
```

### Compiles and hot-reloads for development
```
npm run serve
```

### Compiles and minifies for production
```
npm run build
```

### Lints and fixes files
```
npm run lint
```

# 主要功能

```
- 使用了vue-router路由，多页面多路由不冲突
- 使用了vuex状态管理
- 使用axios库，简单封装了一个库
- 使用了eslint代码规范检测 默认关闭 打开在vue.config.js中设置lintOnSave: true
- 配置了css预设器配置项
```
 

# 多页面多路由使用了两种方案  

  你可以根据自己爱好选择其中一种，文件配置目录在vue.config.js中
  
## dist打包目录
- 第一种

```
 dist
  ├─about
  │  └─js
  ├─chunk-vendors
  │  └─js
  ├─img
  ├─index
  │  ├─css
  │  └─js
  ├─page1
  │  ├─css
  │  └─js
  └─page2
      ├─css
      └─js
```
- 第二种

```
dist
  ├─css
  │  └─index.bc622c39.css
  │  └─page1.aaf0ae55.css
  │  └─page2.db92da3f.css
  ├─js
  |  └─about.1644de76.js
  |  └─chunk-vendors.19368321.js
  |  └─index.31851ae9.js
  |  └─page1.0c42efc5.js
  |  └─page2.06218d45.js
  ├─img
  |  └─logo.82b9c7a5.png
  ├─favicon.ico
  ├─index.html
  ├─page1.html
  └─page2.html
```