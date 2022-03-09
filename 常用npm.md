# npm

## 前端

> 目前来说，创建一个 React 应用最简单的方式是使用一个叫做 create-react-app 的工具。如果你随着 node 安装的 npm 工具版本号不小于 5.3，你就可以（也不是必须的）在机器上安装 create-react-app 了。

```powershell
npx create-react-app my-app
```

> 也就是说，我们将使用 axios 库来代替浏览器和服务器之间的通信。它的功能类似于 fetch，但是使用起来更友好。使用 axios 的另一个很好的理由是，我们已经熟悉了为 React 项目添加外部库，即使用所谓的 npm 包。

```powershell
npm install axios
```

> 幸运的是 React 有 React-router 库，它为管理 React-application 中的导航提供了一个很好的解决方案。

```powershell
npm install react-router-dom@5.3.0
```

```powershell
npm install react-router-dom@6
```

```powershell
npm install antd --save
```

```powershell
npm install --save @ant-design/icons
```

> 如果我们希望使用 Togglable 组件时，强制给按钮一个 label text 属性值。

```powershell
npm install prop-types
```

## 后端

> 为了提供一个比内置的 http 模块更友好的界面，许多库已经开发出来，以简化使用 Node 作为服务器端开发。这些库致力于为构建后台服务器的一般的用例提供一个更好的抽象，到目前为止，最受欢迎的库是 express。

```powershell
npm install express
```

> nodemon 将监视启动 nodemon 的目录中的文件，如果任何文件发生更改，nodemon 将自动重启 node 应用。

```powershell
npm install --save-dev nodemon
```

> 在你的日志应用中添加 morgan 中间件。将其配置为基于 tiny 配置，将消息记录到控制台。

```powershell
npm install morgan
```

> 我们可以通过使用 Node 的 cors 中间件来允许来自其他源的请求。

```powershell
npm install cors
```

```powershell
npm install eslint-plugin-react-hooks
```

> Mongoose 可以被描述为 object document mapper （ODM），并且将 JavaScript 对象保存为 Mongo 文档对于 Mongoose 库来说很简单。

```powershell
npm install mongoose
```

> 有很多方法可以定义环境变量的值。一个更复杂的方法是使用 dotenv，你可以使用如下命令安装库:

```powershell
npm install dotenv
```

> 在 JavaScript 的世界里，目前主要的静态分析工具又名“linting”是 ESlint。

```powershell
npm install eslint --save-dev
npx eslint --init
```

> 许多公司定义了通过 ESlint 配置文件在整个组织中执行的编码标准。建议不要一遍又一遍地使用重造轮子，从别人的项目中采用现成的配置到自己的项目中可能是一个好主意。最近，很多项目都采用了 Airbnb 的 Javascript 风格指南，使用了 Airbnb 的 ESlint 。

```powershell
npx install-peerdeps --dev eslint-config-airbnb
```

> 人们开始怀疑，是否有可能重构代码以从方法中消除 catch？express-async-errors 库为此提供了一个解决方案。

```powershell
npm install express-async-errors
```

> 让我们来安装 bcrypt 用来生成密码的哈希值。

```powershell
npm install bcrypt
```

替代

```powershell
npm i bcryptjs
```

> 让我们在 Mongoose validator 的帮助下验证用户名的唯一性。正如我们在练习 3.19 中提到的，Mongoose 并没有内置的 validator 来检查某个字段的唯一性。我们可以使用一个现成的解决方案 mongoose-unique-validator 这个 npm 包，先安装一下：

```powershell
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

```powershell
npm install --save-dev jest
```

> 们可以通过如下命令安装 cross-env 作为一个开发依赖包。

```powershell
npm install --save-dev cross-env
```

> 除了 Jest 之外，我们还需要另一个测试库，它将帮助我们以测试目的渲染组件。 目前最好的选择是 react-testing-library ，这个库在最近几年迅速流行起来。

```powershell
npm install --save-dev @testing-library/react @testing-library/jest-dom
```

> 在过去的一年里，E2E 库 Cypress 变得非常流行。 Cypress 是非常容易使用，与 Selenium 相比需要少得多麻烦和头痛问题。
>
> 它的操作原理与大多数 E2E 测试库完全不同，因为 Cypress 测试完全在浏览器中运行。
>
> 其他库在一个 node 进程中运行测试，进程通过一个 API 连接到浏览器。

```powershell
npm install --save-dev cypress
```

> 我们的测试使用的变量 cy 给了我们一个讨厌的 Eslint 错误。
>
> 我们可以通过安装eslint-plugin-cypress作为开发依赖项来摆脱这个报错。

```powershell
npm install eslint-plugin-cypress --save-dev
```
