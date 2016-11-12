# bone-act-buble
> buble for bone plugins

[![NPM version](https://img.shields.io/npm/v/bone-act-buble.svg?style=flat)](https://npmjs.org/package/bone-act-buble) [![NPM version](https://img.shields.io/npm/dm/bone-act-buble.svg?style=flat)](https://npmjs.org/package/bone-act-buble) [![travis](https://api.travis-ci.org/wyicwx/bone-act-buble.png)](https://travis-ci.org/wyicwx/bone-act-buble)

### 安装及使用

通过npm安装

```sh
$ npm install bone-act-buble 
```

安装后在`bonefile.js`文件内通过`act()`加载

```js
var bone = require('bone');
var buble = bone.require('bone-act-buble');

bone.dest('dist')
    .src('~/src/es6.jsx')
    .act(buble)
    .rename({
        ext: '.js'
    });
```

### filter

默认设置只针对源文件后缀为`.js`和`.jsx`文件进行处理

### 其他

处理器开发以及使用请参考[处理器](https://github.com/wyicwx/bone/blob/master/docs/plugin.md)