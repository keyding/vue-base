# 快速原型开发

>  适用于测试vue新特性，示例项目或组件的快速开发等

### 需要全局安装扩展
```bash
npm install -g @vue/cli-service-global

或 

yarn global add @vue/cli-service-global (推荐)
```

### 使用 `vue serve` 进行单文件的快速开发 
##### 示例位置：src/single_components

```bash
# 自动导入入口文件，`main.js`、`index.js`、`App.vue`、`app.vue`，其中一个
vue serve

# *.vue 单文件
vue serve single.vue 

# *.js 单文件
vue serve util.js

# -o(--open) 自动打开浏览器
vue serve -o single.vue 
```
也可以指定一个 `index.html`、`package.json`, 安装并使用本地依赖, 甚至通过配置文件配置 `Babel`、`PostCSS` 和 `ESLint`

### 使用 `vue build` 打包
##### 示例位置：src/single_components

```bash
# 构建目标：app (默认)
vue build single.vue

# 构建目标: lib，库
vue build -t lib single.vue

# 构建目标: lib，库，可指定库名称
vue build -t lib -n SingleLib single.vue
```

### 更多参考

> [官方文档 - 快速原型开发](https://cli.vuejs.org/zh/guide/prototyping.html)<br>
> [官方文档 - 构建目标](https://cli.vuejs.org/zh/guide/build-targets.html#%E5%BA%94%E7%94%A8)