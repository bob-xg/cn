# MariaDB 根据时间点创建实例
在使用云数据库实例的过程中，如果由于软件异常或者某种突发情况导致云数据库实例中的数据出现了脏数据的情况，然后你想恢复到之前某一个时刻的数据的话，就可以通过使用根据时间点创建实例，恢复出一个新的云数据库实例。

## 前提条件
* 已经开通云数据库 RDS 权限。
* 如果创建计费方式为按配置的资源，请确保您的账户余额（或代金券金额）不少于 50 元。
* 选择恢复的时间点最小值为目标实例创建时间往后推 30 分钟。

## 注意事项 
* 新实例的规格不能小于备份所在源实例的规格

## 操作步骤
1. 登录 [云数据库 RDS 控制台](https://rds-console.jdcloud.com/database) 。
2. 在实例列表页， 选择需要根据时间点创建新实例的目标实例，进入到目标实例详情页，点击页面右上角的 ***操作 -》根据时间点创建***，进入创建页。
3. 实例配置的参数说明如下：

* 地域：不可以修改，默认就是备份源实例所在的地域。
* 选择日期：可以选择最近前 7 天的任意一天，但是不能早于目标实例的创建日期，具体以控制台为准。
* 选择时间：如果日期和目标实例的创建时间是同一天，那么只能选择创建时间的后 30 分钟的时刻，具体以控制台为准。
* 数据库类型：新建实例的数据库类型，这里类型不能修改，默认采用目标实例的数据库类型。
* 版本：新建实例的数据库版本，这里版本不能修改，默认采用目标实例的数据库版本。
* 存储类型：不同的存储类对应的实例规格的最大IOPS不同, 请参考 [MariaDB 产品规格](../../../Introduction/Specifications/MariaDB-Specifications.md)。
* 规格：实例的CPU和内存，不同的规格对应不同的最大连接数和最大IOPS；关于规格的详细说明，请参考 [MariaDB 产品规格](../../../Introduction/Specifications/MariaDB-Specifications.md)。
* 存储空间：该存储空间包括数据空间、系统文件空间以及日志文件空间。
* 私有网络：只支持在私有网络中创建。如果用户没有私有网络及子网，可以通过【新建私有网络】和【新建子网】的链接创建私有网络和子网。创建完成后，点击【刷新】，就可以看到新创建的私有网络和子网了。
   * 在选择私有网络的时候，请确保需要连接数据库实例的云主机和数据库实例在同一个私有网络内。
   * 由于管理的需要，选择的子网保留若干剩余IP才允许创建实例。
      - MySQL, Percona, MariaDB：需要4个以上的剩余IP
* 部署方式：目前支持单可用区部署，多可用区部署两种部署方式。
   * 多可用区部署：数据库主从分别位于不同的可用区，可用性更高：一个可用区发生故障，整个实例仍然可提供服务。
   * 单可用区部署：主从位于同一可用区，如果该可用区发生故障，整个实例无法对外提供服务。
* 基本信息
   * 实例名称：允许重复，名称的长度和字符有一定限制，具体以控制台为准。
* 参数组：只能选择和数据库类型一直的参数组，如果当前账户下没有参数组，则系统会默认自动创建一个默认参数组。 
* 购买时长：如计费方式选择包年包月则需选择购买时长，可选择1个月至3年；购买的时长越长，折扣力度越大，具体以控制台为准。

![根据时间点创建](../../../../../../image/RDS/MariaDB-Create-To-Point-In-Time.png)

4. 点击 立即购买 进入订单确认页。
5. 阅读完云数据库 RDS 服务条款，按照提示完成后续操作
    * 包年包月实例：点击立即支付，进入到支付确认页，可以选择多种支付方式，如可以使用代金券，余额，银行卡等等。
    * 按配置实例：点击立即开通，开始创建实例，进入到实例列表页。
