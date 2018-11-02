# 需求
在大家加入开发组之前我们先做一个小练习当门槛吧。

需求是这样的，现在你要完成一个评论页面，包括评论的输入和显示。

![](https://coding.net/u/wuancake/p/wuancake/git/raw/master/tests/1608297fa1b24431.png)

# 要求
1. 样式之类的不需要过多的做，只需要功能就行，毕竟考察的主要是Vue。
2. 组件化，别写在一坨。
3. 要求显示的时候显示发布者、发布时间以及内容。

# 数据格式参考
## 评论数据格式
```Javascript
{
    id: 123,   // 这个你们可以随机生成
    publisher: "梁王",
    content: "玩蛇TV",
    created_at: "2017-12-23T09:01:47.053Z" // ISO date
}

```