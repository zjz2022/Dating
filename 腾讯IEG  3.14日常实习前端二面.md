# 腾讯IEG  3.14日常实习前端二面

![img](D:/%E6%96%87%E4%BB%B6/typora%E5%9B%BE%E7%89%87/D2B5CA33BD970F64A6301FA75AE2EB22.png)

上次还说人家是kpi，结果人家给我过了，感谢一面面试官![img](D:/%E6%96%87%E4%BB%B6/typora%E5%9B%BE%E7%89%87/62AF11E48344D159DA608796DA7D39E5.png)

上周三面完一面，第二周周一下午突然给我发了二面邮件，约的周四，二面和一面相差时间八天。

一下子紧张起来了，不得不说今天真的紧张到不行，因为一面面试官都有点kpi摆烂的，搞得我都觉得必挂的，面完就不在乎了，结果能有二面就搞得我好认真好紧张

话说二面，是牛客网面试？？它们竟然还有合作，我一进去看到都是code页面以为要全程手撕代码了

![img](D:/%E6%96%87%E4%BB%B6/typora%E5%9B%BE%E7%89%87/D2B5CA33BD970F64A6301FA75AE2EB22-1710919046967-1.png)

**二面**

面试官开了摄像头，狠狠好评，是个三十多岁的人，感觉比百度二面的那个面试官看着友善一点

上来先是自我介绍，然后直接问我三道业务题（感觉又有点小kpi风格），没让我写，直接口述

第一道是，爬楼梯，问我到十级楼梯有多少方案，我直接就说斐波那契数列1 1 2 3 5 8 ... ，然后问我不是10而是n的话要注意什么，我说要弄个备忘录，以免重复计算。然后又问我n非常大会不会溢出，我想了想会，假如当n-1 + n-2 的值已经大于2^51 -1，那此时就会发生溢出等等问题，我说可以用大数相加解决，转为字符串形式，不会有number的限制，或者使用bigInt。不知道答得咋样这个



第二道是，一千万人，怎么选出前十个成绩最高的。我满脑子都是快排，但是时间复杂度O(nlogn)，一千万已经很夸张了，又说了堆，但感觉都不太好，面试官问能不能一次遍历搞定，我的想法就是维护一个数组，里面存放最大的十个数，不过其实在数组里面选个合适的位置插入也都做不到O(n)。答得挺差的，确实没什么思路



第三道是，做个抽奖系统，一等奖一个概率1%，二等奖两个概率2%，三等奖三个概率3%，问我怎么做。我的想法是用random()来做，0~1一共100个数，random() - 0.99大于0就说明是1，此时为一等奖，同理二三等奖也可以这么获得，就是得用三个random()**，**或者用一个的话得处理一些case。然后面试官问我，random()真的是0~1一共100个数吗，我突然发现不是哦![img](D:/%E6%96%87%E4%BB%B6/typora%E5%9B%BE%E7%89%87/62AF11E48344D159DA608796DA7D39E5.png)就说用random() * 100 再用floor()向下取整，这就获得的就是0~100共100个整数。然后面试官也没说啥就过了



感觉上面三道题都没有回答的特别好，评论区的uu们可以讲下有什么好的解决办法，我只是个菜鸡![img](D:/%E6%96%87%E4%BB%B6/typora%E5%9B%BE%E7%89%87/8B36D115CE5468E380708713273FEF43.png)

然后就开始问前端方面的问题，他问的都很基础基本也很深，会顺着我的回答继续问下去，感觉面试官的专业水平很高

问我对前端的理解，回答的是我自学的路程

问我vue的核心，回答是数据驱动，然后又是经典背八股的数据劫持那些东西

问我长连接有哪些方式，我回答http请求头中的connect: keep-alive。他说不是这个长连接![img](D:/%E6%96%87%E4%BB%B6/typora%E5%9B%BE%E7%89%87/62AF11E48344D159DA608796DA7D39E5.png)![img](https://uploadfiles.nowcoder.com/images/20220815/318889480_1660553763490/62AF11E48344D159DA608796DA7D39E5)![img](https://uploadfiles.nowcoder.com/images/20220815/318889480_1660553763490/62AF11E48344D159DA608796DA7D39E5)又问了我keep-alive的意思，然后问我长连接的意思，我回答是客户端不断向服务端发送信息，其实我是不知道的，但总得蒙一蒙吧![img](https://uploadfiles.nowcoder.com/images/20220815/318889480_1660553763490/62AF11E48344D159DA608796DA7D39E5)然后面试官没说啥就换了下一题，估计看我也不知道

问我向后端请求有什么方式，回答了fetch和ajax，问我还有吗，我知识储备真的不够，真的想不到别的，他问我有没有用过websocket，我说我只听过没有用过，又问我什么是socket，我回答是套接字，但我确实不知道更多了![img](D:/%E6%96%87%E4%BB%B6/typora%E5%9B%BE%E7%89%87/8B36D115CE5468E380708713273FEF43.png)然后也跳过了

问我http和https用了什么协议，http和https有什么不同，简单的讲了下

其它的暂时想不到了



总体面试下来，感觉面试官很专业，也很尊重人，等会面试评价问卷下来给他一个大大的好评![img](D:/%E6%96%87%E4%BB%B6/typora%E5%9B%BE%E7%89%87/A95184503DF1D65798194F12FCEDE5C5.png)，虽然感觉也有一点点点点的kpi，不过感觉从这次面试来说我也学到很多，我还是太菜了，继续努力朋友们![img](D:/%E6%96%87%E4%BB%B6/typora%E5%9B%BE%E7%89%87/8B36D115CE5468E380708713273FEF43.png)

许愿伟大的鹅收留我吧![img](D:/%E6%96%87%E4%BB%B6/typora%E5%9B%BE%E7%89%87/8B36D115CE5468E380708713273FEF43.png)一个大厂对于双非一本的小弱鸡来说吸引力太大了![img](https://uploadfiles.nowcoder.com/images/20220815/318889480_1660553763930/8B36D115CE5468E380708713273FEF43)



[#爱鹅信鹅等鹅#]()



作者：bulletganggang
链接：https://www.nowcoder.com/?type=818_1
来源：牛客网