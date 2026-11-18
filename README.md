# mini-rmi

一个最小的 Java 远程调用模拟。客户端按接口拿动态代理，服务端收到方法描述后反射执行。

写于 2020 年，用来把「注册节点、生成代理、发起调用」这条链走通。

## 里面有什么

- `RmiServer`：按端口或配置文件启动，接受调用
- `RmiClient#getProxy`：按接口生成代理
- `INode` / `INodeSelector`：选择要连的服务节点

源码在 `easyRmi/src`，包名 `com.mec.mec_rmi`。目录是当时的 Eclipse 工程，没有 Maven 或 Gradle。

## 状态

学习代码，源码按最初上传的样子保留。仓库曾用名 `easyRmi`，旧地址会重定向到这里。
