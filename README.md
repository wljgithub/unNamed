# unNamed
I haven't decided the name for repository yet

# purpose

why i create this repository is for collecting some good ideas or questions.it may be just a questions without answer,or a good ideas with implementation


background

I want to know how many and which routers did my datagram go through when i browser the web,so i traced the package  by tracert,here is the result. 

```shell
  1    <1 毫秒   <1 毫秒   <1 毫秒 192.168.1.1
  2     6 ms     4 ms     5 ms  100.64.0.1				-- 保留地址
  3     3 ms     2 ms     2 ms  202.105.155.193			-- 广东省深圳市 电信
  4     7 ms    18 ms    19 ms  202.105.158.85			-- 广东省深圳市 电信
  5     7 ms     6 ms     7 ms  113.96.4.102			-- 广东省广州市 电信
  6     7 ms     6 ms    12 ms  113.96.11.78			-- 广东省广州市 电信
  7     7 ms     6 ms     7 ms  14.29.121.198			-- 广东省广州市 电信
  8     *        *        *     请求超时。				
  9     *        *        *     请求超时。
 10     6 ms     6 ms     6 ms  14.215.177.38			-- 广东省广州市 电信
```

Q:为什么第二行的地址是保留地址，这一跳的路由是哪里。

Q:还有个很有意思的现象，我用tracert追踪数据包的时候，经常在最后的两条路由丢包，这是防火墙吗？