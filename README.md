React has been designed from **the start for gradual adoption.**

**you can use as little or as much React as you need.**

---

## <span style="color:red">Error</span>总结：
1. 如果`ReactDOM.render`中没有发现要插入的节点时，会报错：
`Uncaught Invariant Violation: Target container is not a DOM element.`

---

# react

## JSX

JSX也是一个表达式，编译后变成一个函数调用并执行后成为一个对象。

你可以将JSX作为**参数，变量，返回对象**

JSX判断字符串和JS表达式
```js
// 字符串可以用引号，对象可以用{}.
const ele = <h1 data-name="name" src={user.avatarUrl}></h1>
// 这里的JSX和Vue的区别：Vue是通过v-bind进行辨别，而react是通过花括号 curly braces。
```

JSX可以防止**Injection Attacks**

---

# create-react-app: single page app

不能删的两个文件：
1. `public/index.html` 用来作为HTML模板
2. `src/index.js` 用来作为React入口

可以创建更多的top-level目录，在production的时候不会被构建。

对于IE9，10，11的话，需要polyfill：https://github.com/facebook/create-react-app/blob/master/packages/react-app-polyfill/README.md