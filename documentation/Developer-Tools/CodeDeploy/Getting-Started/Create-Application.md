## 新建应用及部署组

在“部署应用”页，指定与云主机相同的地域后，点击“新建应用”，

![Alt text](https://github.com/jdcloudcom/cn/blob/codedeploy/image/CodeDeploy/starting5.png)


跳转到“新建应用”页。

在“新建应用”页，首先填写应用信息。应用名称：codedeploy-app-demo01

![Alt text](https://github.com/jdcloudcom/cn/blob/codedeploy/image/CodeDeploy/starting6.png)

点击"创建"，即新建应用。

接下来，在应用中新建部署组，

![Alt text](https://github.com/jdcloudcom/cn/blob/codedeploy/image/CodeDeploy/starting10.png)

有以下选项：

- 部署组名称：请填写部署组名称，codedeploy-group-demo01
- 部署类型：请选择“滚动部署”
- 部署目标：点击“选择”按钮，在弹窗中选择云主机。支持三种选择过滤条件：高可用组、标签、IP。这里请选择在上一步中创建的云主机，即主机名为：codedeploy-demo01
- 使用负载均衡：否
- 并发度：100%
- 高级选项：保持默认选项，详见操作指南

![Alt text](https://github.com/jdcloudcom/cn/blob/codedeploy/image/CodeDeploy/starting8.png)

填写部署组的基本信息后，请点击“创建”，将进行应用中部署组的创建。

创建成功后，将跳转到“应用”页。
