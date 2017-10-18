# jquery-headClone
headhesive.js创建一个按需显示头部。指定当你浏览器滚动到某个位置时显示。

## 如何使用？
Headhesive.js是没有依赖关系一个独立的JavaScript插件。在你的页面的页脚包括headhesive.min.js并初始化它：

//创建Headhesive的一个新实例
var headhesive = new Headhesive('.header');
Styling Headhesive.js
Headhesive.js不注入任何CSS样式，这样你就可以使用自己的完全控制您元素的样式。

选项
自定义Headhesive如何工作通过传递自定义选项。

// Options
var options = {
    offset: 500
}

//创建Headhesive的一个新实例，并传递一些选项
{
    //滚动偏移量。接受号码或“字符串”（类/ID）
    offset: 300, // OR ― offset: '.classToActivateAt',
    //自定义类
    classes: {
        //克隆ELEM类
        clone: 'headhesive',
        // Stick class
        stick: 'headhesive--stick',
        //取消置顶类
        unstick: 'headhesive--unstick'
    },
    //滚动事件触发每250ms的以获得性能的提升
    throttle: 250,
    //回调
    onInit: function() {},
    onStick: function() {},
    onUnstick: function() {},
    onDestroy: function() {},
}
