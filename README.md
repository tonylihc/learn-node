## Learn NodeJS

- 1.
nodejs
一个简单的node server
```javascript
    const http = require('http');

    const hostname = '127.0.0.1';
    const port = 3000;

    const server = http.createServer((req, res) => {
        res.statusCode = 200;
        res.setHeader('Content-Type', 'text/plain');
        res.end('Hello World\n');
    });

    server.listen(port, hostname, () => {
        console.log(`Server running at http://${hostname}:${port}/`);
    });
```

    node 中的命令行和浏览器终端是不太一样的，如 node命令行中的 `process` 或者是 浏览器中的 `window` 和 `document`



- 2.
模块 与 Common.js

 依赖关系 ----|　　　　　　　　　　　　定义
 命名空间 --->|  ` 纠结的编程体验 `　　　　　标识
 代码组织 ----|　　　　　　　　　　　　引用
模块的分类
`核心模块`   如  http fs path
`文件模块`   如  var util = require('./util.js')
`第三方模块` 如  var promise = require('bulebird')

- 3.
HTTP




> 2016.11.1 