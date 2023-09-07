# chatserver
可以工作在nginx tcp负载均衡环境中的集群聊天服务器和客户端源码 基于muduo、mysql、redis实现


编译方式
cd build
rm -rf *
cmake ..
make

需要配置nigix tcp的负载均衡
需要启动redis服务
需要启动mysql服务

在nigix/conf/nginx.conf中修改允许连接的服务器ip 和监听端口
