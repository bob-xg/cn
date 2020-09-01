# 快照计费模式说明



## 计费规则

云硬盘快照提供按用量计费的模式，计费规则如下：

- 按照每个地域快照的实际数据量进行计费，每天每个region生成一份快照账单；每个快照的实际数据量等于该快照的源盘自上一次做快照的时刻到本次做快照的时刻间，总的数据变更量，如果是首次做快照，则等于源盘做快照时刻的实际数据量。

- 账单所采用的快照数据量的计算方式为：在一天中的每个小时进行快照数据量采样，取一天中所有采样数据的平均值，作为当日的快照数据量。

- 最小计费周期为一天，不足一天的，按照一天计算。

- 云硬盘快照将在每个地域创建一个虚拟的快照资源ID，代表该地域下所有的云硬盘快照，前缀为“snapfee-”，每个地域的快照账单将记录在该地域的虚拟快照资源ID中。

- 创建快照时，请确认您的账户余额不少于50元。如账号金额少于50元，将不能成功创建快照，需充值至余额50元及以上，方可正常使用。

- 云硬盘快照暂不支持包年包月的计费方式，不支持续费。

  



## 到期、欠费规则

当您账户的可用余额（含现金余额、可用代金券）不能结清云硬盘快照已出账单时，系统即判定该地域内云硬盘快照欠费，您在该地域内所有的快照均会变为已欠费状态；

当您的云硬盘快照欠费后，您将无法继续创建云硬盘快照；

当您的云硬盘快照欠费后，会向您发送邮件和短信通知您的资源已欠费，请您务必注意查看通知并及时充值，以免造成不必要的损失；

云硬盘快照创建时间距开始欠费时间大于3天的，从该地域快照开始欠费时刻起，快照保留7天，7天后系统回收资源，数据无法找回；云硬盘快照创建时间小于3天的，停服后数据保留时间等于云硬盘快照使用时长（从创建时间到欠费时间的时长），之后系统回收资源，数据无法找回；

当您补缴欠费金额后，云硬盘快照恢复正常计费状态，同时继续累计云硬盘快照使用时长；



## 到期、欠费提醒

**欠费停服通知**

京东智联云将在您欠费后向您推送欠费停服通知。

**释放预警通知**

京东智联云将在云硬盘快照（不包含使用时间小于3天的云硬盘快照）欠费的第4天、第6天将向您推送释放预警通知。

以上通知均会以短信、邮件及站内信方式向您推送，请您关注。