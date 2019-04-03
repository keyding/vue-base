# 快速原型开发

### 适用于测试vue新特性，示例项目或组件的快速开发等

>  参考 [官方文档 - 快速原型开发](https://cli.vuejs.org/zh/guide/prototyping.html)


#### 全局安装扩展
```
npm install -g @vue/cli-service-global

或 

yarn global add @vue/cli-service-global (推荐)
```

#### 使用 `vue serve` 进行`*.vue` 单文件的快速开发 
##### 示例位置：src/single_components/single.vue

```bash
# 开发模式启动服务器
vue serve single.vue 

# -o(--open) 自动打开浏览器
vue serve -o single.vue 
```

- `vue serve` 使用和 `vue create` 创建项目时相同的默认设置 (webpack、Babel、PostCSS 和 ESLint)

- 可不指定入口文件名，自动导入入口文件，入口文件是：`main.js`、`index.js`、`App.vue`、`app.vue`，其中的一个，或显示指定入口文件

- 也可以指定一个 `index.html`、`package.json`, 安装并使用本地依赖, 甚至通过配置文件配置 `Babel`、`PostCSS` 和 `ESLint`

#### 还可以直接运行 `*.js` 文件
##### 示例位置：src/single_components/util.js

```
vue serve util.js
```

#### 使用 `vue build` 打包
##### 示例位置：src/single_components/single.vue

```
vue build single.vue
```
可选参数

```bash
# 构建目标，默认app，有 lib 、wc、wc-async 可选
vue build -t lib single.vue
```


