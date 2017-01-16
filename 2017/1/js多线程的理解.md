简单说
1. 单窗口只有一个js线程
2. 浏览器不是单线程，浏览器引擎除了js执行引擎还会有其他线程
3. 异步任务执行的时候会去调用浏览器的其他线程，如渲染、http请求等，执行结果会体现在设置的回调函数中。
4. 回调函数在窗口线程排队，等待处理。

参考：

[http://www.cnblogs.com/yasmi/articles/5064588.html](http://www.cnblogs.com/yasmi/articles/5064588.html)

[http://www.ruanyifeng.com/blog/2014/10/event-loop.html](http://www.ruanyifeng.com/blog/2014/10/event-loop.html)