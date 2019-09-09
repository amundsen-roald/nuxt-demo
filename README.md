# nuxt-demo

> 

## Build Setup

``` bash
# install dependencies
$ npm run install

# serve with hot reload at localhost:3000
$ npm run dev

# build for production and launch server
$ npm run build
$ npm run start

# generate static project
$ npm run generate
```

For detailed explanation on how things work, check out [Nuxt.js docs](https://nuxtjs.org).


## Nuxt.js 项目目录结构

#### assets 资源目录
- 用于组织未编译的静态资源，例如less、sass、javascript

#### component 组件目录
- 用于组织应用的 Vue.js 组件
- Nuxt.js 不会扩展增强该目录下 Vue.js 组件，即这些组件不会像页面组件那样有 asyncData 方法的特性

#### layoputs 布局目录
- 用于组织应用的布局组件
- 若无额外配置，该目录不能被重命名

#### middelware 中间件目录
- 用于存放应用的中间件

#### pages 页面目录
- 用于组织应用的路由及视图
- Nuxt.js 框架读取该目录下所有的 .vue 文件并自动生成对应的路由配置
- 若无额外配置，该目录不能被重命名

#### plugins 插件目录
- 用于组织那些需要在 根vue.js应用 实例化之前需要运行的 Javascript 插件

#### static 静态文件目录
-  用于存放应用的静态文件
- 此类文件不会被 Nuxt.js 调用 Webpack 进行构建编译处理
- 服务器启动的时候，该目录下的文件会映射至应用的根路径 / 下
- 若无额外配置，该目录不能被重命名

#### store 状态管理目录
- 用于组织应用的 Vuex 状态树 文件
- Nuxt.js 框架集成了 Vuex 状态树 的相关功能配置
- 在 store 目录下创建一个 index.js 文件可激活这些配置
- 若无额外配置，该目录不能被重命名

#### nuxt.config.js 文件
- 用于组织Nuxt.js 应用的个性化配置，以便覆盖默认配置
- 若无额外配置，该目录不能被重命名

#### 别名
- ~或@ 指向 srcDir 目录
- ~~或@@ 指向 rootDir 目录
- 默认情况下， srcDir 和 rootDir 相同


## nuxt.config.js 配置

#### build
- Nuxt.js 允许你在自动生成的 vendor.bundle.js 文件中添加一些模块，以减少应用 bundle 的体积。如果你的应用依赖第三方模块，这个配置项是十分实用的。

#### css
- 该配置项用于定义应用的全局（所有页面均需引用的）样式文件、模块或第三方库。

#### dev
- 该配置项用于配置 Nuxt.js 应用是开发还是生产模式。

#### env
该配置项用于定义应用客户端和服务端的环境变量。

#### generate
- 该配置项用于定义每个动态路由的参数，Nuxt.js 依据这些路由配置生成对应目录结构的静态文件。

#### head
- 该配置项用于配置应用默认的meta标签。

#### loading
- 该配置项用于个性化定制 Nuxt.js 使用的加载组件。

#### modules
- 该配置项允许您将Nuxt模块添加到项目中。

#### modulesDir
- 配置项允许您定义Nuxt.js应用程序的node_modules文件夹。

#### plugins
- 该配置项用于配置那些需要在 根vue.js应用 实例化之前需要运行的 Javascript 插件。

#### rootDir
- 该配置项用于配置 Nuxt.js 应用的根目录。

#### router
- 该配置项可用于覆盖 Nuxt.js 默认的 vue-router 配置。

#### server
- 此选项允许您配置Nuxt.js应用程序的服务器实例变量。

#### srcDir
- 该配置项用于配置应用的源码目录路径。

#### dir
- 此选项允许您配置Nuxt.js应用程序的自定义目录。

#### transition
- 该配置项用于个性化配置应用过渡效果属性的默认值。