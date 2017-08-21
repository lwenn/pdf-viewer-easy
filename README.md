## pdf.pack.js
对pdf.js的封装，使用更方便，不需要关注内部细节，适配 retina 等高清屏。

另外内嵌了加载样式。

[demo](https://lwenn.github.io/pdf-viewer-easy/)

### API
`PDF(pdfUrl, container, options)`

**param**
* `pdfUrl` {String} 必填，pdf的地址
* `container` {String} 必填，显示pdf的容器id
* `options` {Object}：可选
    - `scale` {Number} 默认值：1
    - `width` {Number} 默认值：'auto'（新增，设置`width`后，`scale`的值会被忽略）
    - `numPages` {Number} 默认值：'auto'
    - `canvasClass` {String}
    - `canvasWrap` {String} 默认值：'div'
    - `canvasWrapClass` {String}
    - `loadBefore` {Function} 加载之前执行
    - `renderAfter` {Function} 渲染完成后执行
