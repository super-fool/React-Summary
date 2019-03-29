React has been designed from **the start for gradual adoption.**

**you can use as little or as much React as you need.**

---

## <span style="color:red">Error</span>总结：
1. 如果`ReactDOM.render`中没有发现要插入的节点时，会报错：
`Uncaught Invariant Violation: Target container is not a DOM element.`

---

# create-react-app: single page app

不能删的两个文件：
1. `public/index.html` 用来作为HTML模板
2. `src/index.js` 用来作为React入口

可以创建更多的top-level目录，在production的时候不会被构建。

对于IE9，10，11的话，需要polyfill：https://github.com/facebook/create-react-app/blob/master/packages/react-app-polyfill/README.md