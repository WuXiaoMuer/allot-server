# allot-server
client->allot->server
### client
#### 1.
>start client.exe
#### 2.
>client.e -> EPL -> client.exe
### allot
#### 1.
>start allot.exe
#### 2.
>allot.e -> EPL -> allot.exe
### server
#### 1.
>start server.exe
#### 2.
>server.e -> EPL -> server.exe
# Start
1. 部署 "server" 在您的服务器，可以选择是否和您的服务器程序端口相同，默认为6666
> port:6666
2. 部署 "allot" 在另一台服务器，添加ip-port指向 "server" ，allot的端口默认为6668
> port:6668
> return: "CPU-U":"CPU+RAM-U"
3. 测试客户端，连接 "allot" port:6668，并发送请求获取最优服务器地址，随后断开连接，连接返回的最优服务器地址和端口；
> 测试内容->"server"
