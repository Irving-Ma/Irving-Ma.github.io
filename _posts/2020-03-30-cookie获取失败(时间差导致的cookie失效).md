## cookie获取失败(时间差导致的cookie失效)

### 问题：

**同样的代码，本地登陆没有浏览器限制，服务和客户端分开在两台电脑，谷歌，edge等登陆失败，火狐是好的。**

### 分析：

1. **debugger跟踪了很多地方，查看日志发现获取cookie失败；**

2. **网上查询资料，说是时间不一致导致的，查看了服务器与本地之间，的确是有十几分钟的时间差；**

<font style="color:red">【注：详情参考[IE、谷歌Cookie获取记录失败，火狐成功](https://blog.csdn.net/bdstjk/article/details/7086588?utm_source=blogxgwz5)，该连接来源网络】</font>

### 解决：

1. **调整客户端及服务器时间一致；**

2. **适当增大cookie的存活时间。**