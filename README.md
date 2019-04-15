# js
一些知识点
1.巧用匿名函数实现JS异步加载
使用场景:设备浏览器监听，A请求返回用户相关信息，B请求响应我们需要的数据。B依赖于A。
所以监听到B请求，需要释放先资源给处理A请求的监听，
2.相关代码
延迟调用B：setTimeout(function(){afterThread(allData,_self)},3000);

