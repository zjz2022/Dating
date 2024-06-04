# base成都 卫翎科技 前端实习面经

## 卫翎科技

投递渠道: BOSS 直聘

时间线

- 2023-11-23 上午 hr 发起打招呼,遂投递简历,下午约面
- 2023-11-27 一面
- 2023-11-29 上午约二面, 下午二面



**一面**

1. 自我介绍
2. 字节青训项目中最有挑战或者收获的点
3. lint-staged 的主要作用是什么(搭配 husky 在 commit 时进行代码检查,面试官补充说只对暂存区的代码进行检查)
4. Vuex 与 Pinia 的区别 💤 (以为掌握了但答得并不好！)
5. 为什么需要对 axios 进行二次封装
6. 虚拟滚动是如何实现的
7. 项目中的防抖技术做了什么
8. CSS 中 px,rem,em 分别是什么
9. 水平垂直居中的实现方式
10. position 有哪些属性, absolute 是相对于谁的
11. 盒模型
12. 隐藏一个元素的方式: display(回流) / visibility(重绘) / opacity(硬件加速)
13. flex 布局设置元素间隙的方式 `gap`
14. JavaScript 中判断数据类型的方法
15. this 的指向???完全不知道怎么说,让我看代码讲还可以
16. 改变 this 指向的方法 -> call 与 apply 的区别
17. 箭头函数有 this 吗?
18. 讲讲原型和原型链
19. 讲讲 Event Loop
20. script 标签会阻塞 DOM 的解析吗 -> 有什么方式可以解决这个问题
21. 讲讲你对 Promise 的理解 Promise 三种状态: pending / fulfilled / rejected链式调用是如何实现的: then 方法返回的是一个新的 Promise 对象
22. 数据类型的隐式转换 发生时机：算术运算符 / 比较运算符 / 逻辑运算符 / if 语句"1" + 1 的结果("11")"2" - 1 的结果(1)

看代码说结果:

```js
const promise = new Promise((resolve, reject) => {
  resolve("success1");
  reject("error");
  resolve("success2");
});

promise
  .then((res) => {
    console.log("then", res);
  })
  .catch((err) => {
    console.log("catch", err);
  });

// then success1
// Promise 状态改变后就不能再改变,虽然后面的代码还能继续执行.
var name = "World";
(function () {
  if (typeof name === "undefined") {
    var name = "Jack";
    console.log("Goodbye " + name);
  } else {
    console.log("Hello " + name);
  }
})();

// Goodbye Jack
// var 变量提升: 只提升定义不提升赋值,并且之提升到所在的作用域的顶部
function f1() {
  console.time("time span");
}

function f2() {
  console.timeEnd("time span");
}

setTimeout(f1, 100);
setTimeout(f2, 200);
function waitForMs(n) {
  var now = Date.now();
  while (Date.now() - now < n) {}
}
waitForMs(500);

// 在执行 setTimeout(f1, 100) 后会开启一个定时器,并在 100ms 后将 f1 放入宏任务队列, 但是回调函数 f1 并不会立即执行,而是等主线程空闲才会执行.
/**
 * 上述代码的执行过程是:
 * 1. 执行 setTimeout(f1, 100)
 * 2. 执行 setTimeout(f2, 200)
 * 3. 执行 waitForMs(500);
 * 4. 由于 waitForMs(500) 会阻塞主线程 500ms, 此时 f1 与 f2 已经被放入宏任务队列中会被取出并且立即执行,所以 time span 实际上是执行带来的延迟而非定时器的延迟.
 */
```



**二面**

1. 为什么选前端
2. 职业规划，对前端的发展方向有了解吗？
3. Github 活跃一般是在看哪些内容？
4. 介绍一下项目中最有挑战的点
5. 对这份工作有什么期待
6. 有没有关注 AI 相关的内容

emmm，其实就是氛围很轻松的闲聊。

结束后 hr 约线下详谈。



hr 姐姐人真的超级好！！！！！！！![img](https://uploadfiles.nowcoder.com/images/20220815/318889480_1660553763930/8B36D115CE5468E380708713273FEF43)



作者：zbwer
链接：https://www.nowcoder.com/discuss/561487629351395328?sourceSSR=users
来源：牛客网