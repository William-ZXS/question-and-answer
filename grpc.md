什么是rpc：

remote procedure call
远程过程调用

相对应的是本地过程调用：同一进程内
远程过程：不同进程


grpc的底层协议是什么？
HTTP2.0

grpc 的用的序列化协议和http 的json区别
grpc通过protobuf 来序列化数据成二进制，更紧凑
json是文本格式，基于字符的，慢，而且臃肿

RESTful 也可以通过 keep-alive 实现长连接，但是它最大的一个问题是它的request-response模型是阻塞的 ( http1.0 和 http1.1，http 2.0 没这个问题)。

什么是request-response阻塞模型



