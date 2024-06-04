# 腾讯实习基地-IEG-前端（1h）-一面

3.8

总的来说很少问八股，基本从项目入手，然后考虑一个场景，怎么去实现这个场景

1. 自我介绍
2. 问了我的第一个可视化项目，这个项目做了些什么，我主要负责了哪些模块
3. 聊到了axios请求，问我axios的请求拦截器，响应拦截器，以及向axios底层向请求拦截器数组添加的是什么（对象还是函数） 由于我说到了请求拦截器先进后出，面试官就让我讲为什么要这样设计，我只能说我不知道。。。。

​       \4. 项目中文件切片怎么切的，断点续传怎么续的，如何显示进度等等 

1. 我聊到了localStorage，面试官就问localStorage里面存的是什么，（键值对，值的类型是字符串）
2. 然后又问我localStorage存值取值的方式，我当时心里很不理解为什么要问这个问题。当我答对的时候，面试官非常捧场对我予以肯定（感觉像是幼儿园老师夸小孩![img](D:/%E6%96%87%E4%BB%B6/typora%E5%9B%BE%E7%89%87/A36B51811C2F08F8B587B123A106E546.png)）
3. 聊了一会儿项目，就开始写html+css代码 

​       刚要写动画，我就开始道歉，给面试官说我马上有个会要开，本来以为就直接终止算了，但是面试官很好，跟我又约了时间

3.11(接着上次写)

1. 开始写动画，整个写代码的过程考察的知识点主要是（nth-child，BFC, flex，动画，settimout， setinterval）

​           写的时候遇到不会的，面试官让我查，就这样边查边写边改bug。。。。

```html
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
    <style>
        #con {
            width: 200px;
            height: 200px;
            background-color: skyblue;
            position: absolute;
            transition: 2s;
        }

        .container {
            width: 400px;
            height: 200px;
            background-color: red;
            display: flex;
            justify-content: space-evenly;
        }

        .son {
            width: 50px;
            height: 50px;
            animation: move linear 2s alternate-reverse infinite
        }

        /* .son1 {
            background-color: skyblue;
        }

        .son2 {
            background-color: blue;
        }

        .son3 {
            background-color: pink;
        } */
        .son:nth-child(1) {
            background-color: skyblue;
        }

        .son:nth-child(2) {
            background-color: blue;

        }

        .son:nth-child(3) {
            background-color: pink;
        }

        @keyframes move {

            0%,
            100% {
                transform: translateY(0);
            }

            50% {
                transform: translateY(150px);
            }
        }
    </style>

</head>

<body>
    <div id="con"></div>
    <!-- <div class="container">
        <div class="son son1"></div>
        <div class="son son2"></div>
        <div class="son son3"></div>
    </div> -->
</body>
<script>
    let con = document.getElementById("con");

    // let timer = setInterval(() => {
    //     leftval += 10
    //     con.style.left = leftval + "px";
    //     if (leftval == 40) {
    //         clearInterval(timer)
    //     }
    // }, 1000)

    //改写上面的代码，用setTimeout来实现setInterval
    var leftval = 0
    function move() {
        leftval += 30
        con.style.left = leftval + "px";
    }

    function mySetinterval(fn, delay) {
        let timer;
        const interval = function () {
            fn();
            console.log("@@@")
            timer = setTimeout(interval, delay);
        }
        timer = setTimeout(interval, delay);
        return () => {
            clearInterval(timer);
        }
    }

    let clearinterval = mySetinterval(move, 1000);



</script>

</html>
```

- 然后又问了项目，做过哪些性能优化，怎么实现的。
- 友友们一定要记住项目中的关键技术呀，会问的比较细。
- 给我一个场景，如果一个请求很慢，客户端怎么办
- 讲讲token。。。。

差不多一小时了，开始反问

1. 面试官给我讲了讲部门的业务（游戏运营，文案之类的）
2. 建议我提升的地方（去官方网站查资料，深挖原理吧）

最后：面试官很不错，虽然我很菜，但是面试官会耐心引导。即使是kpi面，也是一次和大牛交流的机会嘛。



作者：超脱的椰子在写总结
链接：https://www.nowcoder.com/?type=818_1
来源：牛客网