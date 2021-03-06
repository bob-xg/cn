# 搭建IPv4/IPv6双栈私有网络

### 简介

  京东智联云私有网络提供创建同时支持ipv4地址和ipv6地址的私有网络（目前IPv6处于公测中，如需使用，请提交工单，申请公测），两种类型的地址均可通过内网/公网进行访问，下面将介绍如何搭建IPv4/IPv6 私有网络。

### 应用场景

- 需要使用双栈网络或者需要使用IPv6私有网络提供服务。

### 前提条件

  首先您需要有京东智联云的账号，并完成实名认证，若您目前没有账号，请先[注册](https://user.jdcloud.com/register?source=jdcloud&ReturnUrl=https%3A%2F%2Fwww.jdcloud.com)。

### 操作步骤

  本教程将介绍，在京东智联云上部署同时支持IPv6和IPv4云主机的私有网络。首先在创建云主机之前，需创建支持IPv6的私有网络、子网。

​		注：创建的资源如私有网络、子网、路由表、网络ACL、安全组等需在同一地域下进行

  **步骤1：** 进入京东智联云控制台，选择私有网络，创建支持IPv6的私有网络，具体操作参考[配置双栈VPC](https://docs.jdcloud.com/cn/virtual-private-cloud/vpc-configuration)；

  **步骤2：** 在步骤1中创建的私有网络下创建路由表，根据需求在路由表详情页进行配置路由策略（也可后续根据业务再配置），具体操作请参考[路由表配置](https://docs.jdcloud.com/cn/virtual-private-cloud/route-table-configuration)；

  **步骤3：** 在步骤1中创建的私有网络下创建支持IPv6的子网，选择步骤2中创建的路由表，具体操作请参考[配置子网](https://docs.jdcloud.com/cn/virtual-private-cloud/subnet-configuration)；

  **步骤4：**（可选）可根据业务需求进行创建，在步骤1中创建的私有网络下创建网络ACL，关联步骤3中创建的子网，配置ACL出入站规则，具体操作请参考[网络ACL配置](https://docs.jdcloud.com/cn/virtual-private-cloud/network-acl-configuration)；

  **步骤5：** 在步骤1中创建的私有网络下创建安全组，配置安全组出入站规则，具体规则可根据后续业务需求进行修改。具体操作请参考[配置安全组](https://docs.jdcloud.com/cn/virtual-private-cloud/security-group-configuration)；

  **步骤6：** 在步骤2中创建的子网下创建IPv6云主机，设置云主机登录密码，绑定步骤5中创建的安全组。具体操作请参考[创建云主机](https://docs.jdcloud.com/cn/virtual-machines/create-instance)；

  完成上述步骤即完成搭建IPv6私有网络，下面进行测试网络的连通性。


### 测试网络连通性

  使用xshell软件进行测试，登录IPv6云主机，ping一个IPv6服务进行测试。

  **步骤1：** 通过xshell登录IPv6云主机，打开xshell，新建会话，输入云主机名称，主机字段输入云主机IPv6地址；

  **步骤2：** 输入云主机的登录用户名及密码，登录成功后，进行测试；

  **步骤3：** 输入ping -6 [其他ipv6地址]，出现下图结果则连通成功。

![image-20200908203808838](../../../../image/Networking/IPv6/IPv6-05.png))

