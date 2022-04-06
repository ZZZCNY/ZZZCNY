# npm

> 让我们运行 npm 审计修复程序，就像报告中建议的那样:

```shell
npm audit fix
```

## 前端

> 目前来说，创建一个 React 应用最简单的方式是使用一个叫做 create-react-app 的工具。如果你随着 node 安装的 npm 工具版本号不小于 5.3，你就可以（也不是必须的）在机器上安装 create-react-app 了。

```shell
npx create-react-app my-app
```

> 也就是说，我们将使用 axios 库来代替浏览器和服务器之间的通信。它的功能类似于 fetch，但是使用起来更友好。使用 axios 的另一个很好的理由是，我们已经熟悉了为 React 项目添加外部库，即使用所谓的 npm 包。

```shell
npm install axios
```

> 幸运的是 React 有 React-router 库，它为管理 React-application 中的导航提供了一个很好的解决方案。

```shell
npm install react-router-dom
```

```shell
npm install react-router-dom@6
```

```shell
npm install antd --save
```

```shell
npm install --save @ant-design/icons
```

> 如果我们希望使用 Togglable 组件时，强制给按钮一个 label text 属性值。

```shell
npm install prop-types
```

> Facebook 有一个 Flux 的实现，但是我们会使用 Redux 库。 它使用相同的原理，但是更简单一些。 Facebook 现在也使用 Redux 而不是原来的 Flux。

```shell
npm install redux
```

> 我们还将添加 deep-freeze 库 ，它可以用来确保 reducer 被正确定义为不可变函数。

```shell
npm install --save-dev deep-freeze
```

> 有多种方法可以与组件共享 redux-store。首先，我们将研究使用最新的，也是最简单的方法，即 react-redux 的 hooks-api。

```shell
npm install react-redux
```

> 在调试时，除了浏览器扩展外，我们还有软件库 redux-devtools-extension。让我们使用如下命令来安装它：

```shell
npm install --save-dev redux-devtools-extension
```

> 这种类型的异步操作可以与 Redux Thunk 库一起使用。使用 Redux 工具包中的 ConfigureStore 函数创建 Redux Store 时，您无需其他配置即可访问库。

```shell
npm install redux-thunk
```

### webpack

> 让我们用下面的命令来安装 webpack:

```shell
npm install --save-dev webpack webpack-cli
```

> 让我们把我们的应用转换成一个最小的 React 应用:

```shell
npm install react react-dom
```

> 让我们将装载器及其所需的包作为开发依赖项安装:

```shell
npm install @babel/core babel-loader @babel/preset-react --save-dev
```

> 值得注意的是，如果捆绑的应用的源代码使用 async/await，浏览器将不会在某些浏览器上渲染任何内容。 谷歌在控制台中搜索错误信息将会在这个问题上给出一些答案。 我们必须再安装一个缺失的依赖项，即@babel/polyfill:

```shell
npm install @babel/polyfill
```

> 让我们添加一个@babel/pressing-env 插件，它包含使用所有最新特性编写代码并将其转化为兼容 ES5 标准的代码所需的所有内容:

```shell
npm install @babel/preset-env --save-dev
```

> 当使用 CSS 时，我们必须使用 CSS 和 style 装载器:

```shell
npm install style-loader css-loader --save-dev
```

> 当前的配置使得开发我们的应用成为可能，但是工作流非常糟糕(以至于它类似于 Java 的开发工作流)。 每次我们对代码进行修改时，我们必须将它捆绑起来并刷新浏览器以测试代码。

```shell
npm install --save-dev webpack-dev-server
```

## 后端

> 为了提供一个比内置的 http 模块更友好的界面，许多库已经开发出来，以简化使用 Node 作为服务器端开发。这些库致力于为构建后台服务器的一般的用例提供一个更好的抽象，到目前为止，最受欢迎的库是 express。

```shell
npm install express
```

> nodemon 将监视启动 nodemon 的目录中的文件，如果任何文件发生更改，nodemon 将自动重启 node 应用。

```shell
npm install --save-dev nodemon
```

> 在你的日志应用中添加 morgan 中间件。将其配置为基于 tiny 配置，将消息记录到控制台。

```shell
npm install morgan
```

> 我们可以通过使用 Node 的 cors 中间件来允许来自其他源的请求。

```shell
npm install cors
```

```shell
npm install eslint-plugin-react-hooks
```

> Mongoose 可以被描述为 object document mapper （ODM），并且将 JavaScript 对象保存为 Mongo 文档对于 Mongoose 库来说很简单。

```shell
npm install mongoose
```

> 有很多方法可以定义环境变量的值。一个更复杂的方法是使用 dotenv，你可以使用如下命令安装库:

```shell
npm install dotenv
```

> 在 JavaScript 的世界里，目前主要的静态分析工具又名“linting”是 ESlint。

```shell
npm install eslint --save-dev
npx eslint --init
```

> 许多公司定义了通过 ESlint 配置文件在整个组织中执行的编码标准。建议不要一遍又一遍地使用重造轮子，从别人的项目中采用现成的配置到自己的项目中可能是一个好主意。最近，很多项目都采用了 Airbnb 的 Javascript 风格指南，使用了 Airbnb 的 ESlint 。

```shell
npx install-peerdeps --dev eslint-config-airbnb
```

> 人们开始怀疑，是否有可能重构代码以从方法中消除 catch？express-async-errors 库为此提供了一个解决方案。

```shell
npm install express-async-errors
```

> 让我们来安装 bcrypt 用来生成密码的哈希值。

```shell
npm install bcrypt
```

替代

```shell
npm i bcryptjs
```

> 让我们在 Mongoose validator 的帮助下验证用户名的唯一性。正如我们在练习 3.19 中提到的，Mongoose 并没有内置的 validator 来检查某个字段的唯一性。我们可以使用一个现成的解决方案 mongoose-unique-validator 这个 npm 包，先安装一下：

```shell
npm install mongoose-unique-validator
```

> 安装 jsonwebtoken 库， 它会允许我们生成 Json Web Token。

```
npm install jsonwebtoken
```

## 测试

> 有许多不同的测试库或者 test runner 可用于 JavaScript。在本课程中，我们将使用一个由 Facebook 内部开发和使用的测试库，这个测试库名为 jest，类似于之前 JavaScript 测试库之王 Mocha。
>
> 对于本课程来说，Jest 是一个自然的选择，因为它可以很好地测试后端，并且在测试 React 应用时表现出色。

```shell
npm install --save-dev jest
```

> 们可以通过如下命令安装 cross-env 作为一个开发依赖包。

```shell
npm install --save-dev cross-env
```

> 除了 Jest 之外，我们还需要另一个测试库，它将帮助我们以测试目的渲染组件。 目前最好的选择是 react-testing-library ，这个库在最近几年迅速流行起来。

```shell
npm install --save-dev @testing-library/react @testing-library/jest-dom
```

> 在过去的一年里，E2E 库 Cypress 变得非常流行。 Cypress 是非常容易使用，与 Selenium 相比需要少得多麻烦和头痛问题。
>
> 它的操作原理与大多数 E2E 测试库完全不同，因为 Cypress 测试完全在浏览器中运行。
>
> 其他库在一个 node 进程中运行测试，进程通过一个 API 连接到浏览器。

```shell
npm install --save-dev cypress
```

> 我们的测试使用的变量 cy 给了我们一个讨厌的 Eslint 错误。
>
> 我们可以通过安装 eslint-plugin-cypress 作为开发依赖项来摆脱这个报错。

```shell
npm install eslint-plugin-cypress --save-dev
```

## React Native

> 在我们的应用开发中，使用到的是 Expo。Expo 是一个简化了 React Native 应用的安装、开发、构建以及部署的平台。我们通过安装 expo-cli 命令行工具来开始吧。

```shell
npm install --global expo-cli
```

> 下一步，我们在 rate-repository-app 文件夹中运行如下命令，来初始化我们的项目。

```shell
expo init rate-repository-app --template expo-template-blank@sdk-40
```

> 通过 React Native 我们可以使用 React router 的核心，包括 hooks 钩子和 components 组件。相比浏览器环境，主要区别是我们要将 BrowserRouter 替换为 React Native 适配的 NativeRouter， 这是由 react-router-native 这个类库提供的。让我们从安装这个 react-router-native 类库开始吧。

```shell
npm install react-router-native
```

## TypeScript

> 在全局范围内同时安装 ts-node 和官方 TypeScript 包。

```shell
npm install -g ts-node typescript
```

> 正如我们在第 3 章中所做的，通过在空目录中运行命令 npm init 来设置 npm 项目。我们可以通过运行如下命令安装依赖：

```shell
npm install --save-dev ts-node typescript
```

> 由于全局变量 process 是由 Node 本身定义的，所以我们可以通过安装包 @types/node 来获得它的类型:

```shell
npm install --save-dev @types/node
```

> 让我们安装 eslint 和它的 TypeScript 扩展:

```shell
npm install --save-dev eslint @typescript-eslint/eslint-plugin @typescript-eslint/parser
```

> 像往常一样运行 npm init 并安装 typescript 包。

```shell
npm install typescript --save-dev
```

> 现在我们可以通过运行如下命令来初始化 tsconfig.json 设置:

```shell
npm run tsc -- --init
```

> 现在我们已经有了首选的配置集，让我们继续安装 express，当然还有 @types/express。由于这是一个真正的项目，并打算随着时间的推移而成长，我们将从一开始就使用 eslint:

```shell
npm install express
npm install --save-dev eslint @types/express @typescript-eslint/eslint-plugin @typescript-eslint/parser
```

> 我们可以在 ts-node 中使用熟悉的 nodemon，但是正如我们前面看到的，ts-node-dev 可以做完全相同的事情，我们也可以继续使用它。

```shell
npm install --save-dev ts-node-dev
```

> 我们可以使用 create-react-app，通过在初始化脚本中添加一个额外的 template 参数，支持使用 TypeScript 创建应用的方法。 因此，为了使用 TypeScript 创建一个 Create React App，运行如下命令:

```shell
npx create-react-app my-app --template typescript
```
