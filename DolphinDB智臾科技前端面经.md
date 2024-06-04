# DolphinDB智臾科技前端面经

公司：DolphinDB （个人感觉类似国产redis）

base：杭州

薪资：14k-24k

工作时间：965

面试时长：70分钟

1、websocket 为什么全双工

2、webscoket 和keep-alive的区别，有了 keep-alive为什么还要websocket

3、websockt同时发数据，如何保证收到的数据是当前的

4、客户端和服务端如何关闭websocket

5、websocket如何发送二进制数据

6、如何判断服务端已经处理完毕二进制数据

7、http1和http1.1 使用 keep-alive 客户端发送到服务端 两个请求 有什么区别

8、解释一下三次握手

9、keep-alive服务端收到第一个get和第二个get ，server如何知道第一个请求已经结束了

10、server什么时候应该返回200

11、说一下http 的header有哪些key

12、tcp如何保证不丢包

13、怎么知道重传的条件

14、包丢了会怎么办

15、js两个数相加会不会丢精度

16、大数相加是否会丢精度

17、js 整数什么是溢出

18、a = '1'

​      b = '2' 怎么相加不会丢失精度

19、什么是 a??b

20、a??b和a||b的区别

21、js有哪些值为null的情况  哪些值为false的情况

22、算法题：

/**

​    现在你总共有 n 门课 (0, 1, ..., n-1) 需要选，课程之间有依赖关系，比如软件工程依赖算法课，算法课依赖数学课，算法课还依赖计算机组成原理课，

​    现在已知所有的课程和课程之间的依赖关系，返回你为了学完所有课程所安排的学习顺序。可能会有多个正确的顺序，你只要返回任意一种就可以了。

​    如果不可能完成所有课程，返回一个空数组。

​    

​    用一个依赖数组 prerequisites 表示它们的依赖关系，数组中的每一项为 [i, j] (0 ≤ i ＜ n;  0 ≤ j ＜ n) 的形式，

​    表示在选修课程 i 前必须先选修 j

​    例如，想要学习课程 0 ，你需要先完成课程 1 ，用一个 prerequisity pair 来表示就是 [0, 1]

​    例如 prerequisites = [[0, 1], [1, 2], [0, 2], [2, 3]]

*/

 

function sort (n: number, prerequisites: [number, number][]): number[] {

​    return []

}

23、一棵树建成堆的操作、时间复杂度和堆的插入删除



作者：想要offer的00后很无语
链接：https://www.nowcoder.com/?type=818_1
来源：牛客网