JS/Pipe 是一个极简的库，使用纯 JavaScript 即可轻松协调复杂并发的事件流和其他数据流。无需回调函数或链式函数。
因此，堆栈跟踪清晰明了，便于调试，同时你还可以使用 try/catch！
JS/Pipe 的灵感来源于 Go 语言中的 Goroutines 和 Channels。
更多信息和在线示例请访问 http://jspipe.org。
开始使用
依赖项
生成器
JS/Pipe 依赖于 ES6 中引入的 JavaScript 生成器。为了让代码在当前 JavaScript 环境中运行，你需要使用一个将 ES6 生成器语法转换为 ES5 语义的转译器。两种流行的选择是 Google Traceur（支持生成器以及许多其他 ES6 特性，如 lambda 语法、解构等）和 Facebook Regenerator（仅专注于生成器支持）。
我们使用 Facebook Regenerator。
构建
克隆此仓库：git clone git@github.com:jspipe/jspipe.git
如有必要，安装 Grunt：npm install -g grunt
安装开发依赖项：npm install
构建：grunt build
构建会生成 ES5 和 ES6 版本（分别位于 dist-es5 和 dist-es6 目录中），并且每种版本的输出都包括 AMD、CommonJS 和模块模式格式的模块。
ES5 兼容文件（*.es5.js）是通过 Facebook 的 Regenerator 工具生成的，该工具用于将（ES6）生成器代码转译为 ES5。你可以从 https://github.com/facebook/regenerator 获取它。

