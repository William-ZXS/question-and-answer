## http1.0 和http1.1区别？

1.  1.0只支持短连接，1.1默认长连接，同一个tcp连接可以支持多个请求
2. 缓存处理不一样了
3. 1.1支持Host头，不再用IP作为请求方标志
4. 状态码增多了

HTTP 1.0中默认是关闭的，需要在 HTTP 头加入" Connection: Keep-Alive"，才能启用 Keep-Alive ；HTTP 1.1中默认启用 Keep-Alive ，如果加入"Connection: close "，才关闭。目前大部分浏览器都是用 HTTP 1.1协议，也就是说默认都会发起 Keep-Alive 的连接请求了，所以是否能完成一个完整的 Keep-Alive 连接就看服务器设置情况。


浏览器一次最多同时发起6个请求

http1.1 和http2.0区别？

http2.0的多路复用为什么比1.1快

1.1文件传输是request-response ，顺序进行，如果第一个获取的文件耗时很长，后面的都会等待

