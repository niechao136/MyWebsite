# MyWebsite
My Website App

```bash

# 安装Vue CLI 3.x
? npm install -g @vue/cli
# 检查是否安装成功
? vue --version

```


```bash

# 以命令行创建项目
? vue create test
# 以图形化界面创建项目
? vue ui

```

```bash

? Please pick a preset: Manually select features
? Check the features needed for your project: Babel, TS, Router, Vuex, CSS Pre-processors, Linter
? Use class-style component syntax? Yes
? Use Babel alongside TypeScript for auto-detected polyfills? Yes
? Use history mode for router? (Requires proper server setup for index fallback in production) No
? Pick a CSS pre-processor (PostCSS, Autoprefixer and CSS Modules are supported by default): Sass/SCSS
? Pick a linter / formatter config: TSLint
? Pick additional lint features: Lint on save, lint and fix on commit
? Where do you profer placing config for Babel, PostCSS, ESLint, etc.? In dedicated config files
? Save this as a preset for future projects? No

```

```bash

├── public                      // 静态页面
├── src                         // 主目录
    ├── api                     // api相关
    ├── assets                  // 静态资源
    ├── components              // 组件
    ├── config                  // 全局变量
    ├── lang                    // 多语言配置
    ├── plugins                 // 插件管理
    ├── routers                 // 路由配置
    ├── stores                  // Vuex 配置
    ├── utils                   // 工具方法
    ├── views                   // 页面
    ├── App.vue                 // 页面主入口
    ├── main.ts                 // 脚本主入口
    ├── shims-tsx.d.ts          // 相关 tsx 模块注入
    └── shims-vue.d.ts          // Vue 模块注入
├── postcss.config.js           // postcss 配置
├── babel.config.js             // babel 配置
├── package.json                // 依赖
├── tsconfig.json               // ts 配置
├── tslint.json                 // tslint 配置
└── vue.config.js               // webpack 配置

```

```json

{
  "name": "ServerMonitor",
  "version": "0.1.0",
  "private": true,
  "scripts": {
    "serve": "vue-cli-service serve",
    "build:dev": "vue-cli-service build --mode development",
    "build:prod": "vue-cli-service build --mode production",
    "build:test": "vue-cli-service build --mode test",
    "lint": "vue-cli-service lint"
  },
  "dependencies": {
    "axios": "^0.19.0",                     // 创建 http 请求
    "core-js": "^2.6.5",
    "crypto-js": "^3.1.9-1",                // 加密解密
    "element-ui": "^2.12.0",                // UI
    "lodash": "^4.17.15",                   // 数组、对象处理
    "moment": "^2.24.0",                    // 时间处理
    "vue": "^2.6.10",
    "vue-class-component": "^7.0.2",
    "vue-cookies": "^1.5.13",               // vue 使用 cookie
    "vue-i18n": "^8.14.1",                  // vue 多语言配置
    "vue-property-decorator": "^8.1.0",
    "vue-router": "^3.0.3",
    "vuex": "^3.0.1",
    "vuex-class": "^0.3.2",                 // vuex 引用装饰器
    "vuex-module-decorators": "^0.10.1"     // vuex 定义装饰器
  },
  "devDependencies": {
    "@types/crypto-js": "^3.1.43",
    "@types/lodash": "^4.14.144",
    "@vue/cli-plugin-babel": "^3.11.0",
    "@vue/cli-plugin-typescript": "^3.11.0",
    "@vue/cli-service": "^3.11.0",
    "file-loader": "^4.2.0",
    "lint-staged": "^8.1.5",
    "sass": "^1.18.0",
    "sass-loader": "^7.1.0",
    "typescript": "^3.4.3",
    "url-loader": "^2.2.0",
    "vue-template-compiler": "^2.6.10"
  },
  "gitHooks": {
    "pre-commit": "lint-staged"
  },
  "lint-staged": {
    "*.ts": [
      "vue-cli-service lint",
      "git add"
    ],
    "*.vue": [
      "vue-cli-service lint",
      "git add"
    ]
  }
}

```

