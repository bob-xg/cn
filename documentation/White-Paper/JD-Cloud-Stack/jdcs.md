# 简介

今年2月19日，IDC组织发布了《IDCFutureScape:全球云计算2020年预测——中国启示》中介绍：到2021年，中国90%以上的企业将依赖于本地/专属私有云、多个公有云和遗留平台的组合，以满足其基础设施需求。

为促进云计算技术的发展，2020年4月7日，京东智联云发布《京东智联云专有云JD Cloud Stack 产品白皮书》， 深入介绍了京东智联云专有云的基本架构、产品和模块组成、核心产品功能和优势特点。向政府、组织机构和企业的领导者和核心技术人员介绍京东智联云专有云各产品模块典型应用方法和云平台的整体运维和管理方法，帮助客户了解京东智联云专有云的技术优势。并基于京东智联云和 AI 对行业的理解和技术积淀，分享了智慧城市专有云解决方案、企业专有云解决方案等典型行业解决方案，为客户选择适合自身业务发展的云计算平台提供有价值的参考。

京东智联云的专有云平台 JD Cloud Stack 产品，是汇聚了京东在云计算和大数据领域多年技术积累的核心成果之一，包含60 多个云计算平台资源产品，涵盖基础资源、弹性计算、网络、 存储、数据库与缓存、互联网中间件、大数据、混合云、安全、网络流量接入、用户接入、后台管理平台、运维工具等各个层次，并通过统一的 JD Cloud Stack 服务目录向用户提供IaaS、PaaS、SaaS、DaaS、 AIaaS 等通用和定制化的云计算服务。

基于京东在大规模分布式系统上的长期技术实践积累，京东智联云专有云的平台技术能力、自主可控能力和服务能力在行业内具有领先优势。在平台技术层面，京东智联云拥有全球最大规模之一的 Docker 集群，中国最大的 GPU 集群之一，具备华北北京、华东上海、华东宿迁、华南广州 4 区域 9 可用区布局，承诺 99.95% 的月度服务级别 SLA，并且具有可信赖的云安全纵深智能防御体系；在自主可控层面，京东智联云不仅自研了多款产品，专有云平台还支持国产 CPU、国产服务器、国产操作系统、国产数据库等多层次国产基础软硬件产品；在服务层面，京东智联云向客户提供包括产品、运维、应用开发等全方位技术培训，帮助客户快速打造自身的运营和运维团队，还提供 7 x 24全时段、全方位、立体式的优质服务，为用户提供多维度的技术保障。


# 京东智联云主要优势

京东智联云经过多年的发展，在不断地技术累积与创新下，形成了如下五大核心优势：

![avatar](https://github.com/jdcloudcom/cn/blob/baishi/image/whitepaper/jdcs1.png)

### 高端的技术人才队伍

京东智联云基于京东集团近20年的互联网技术积累，组建了一支成熟稳定的以高端技术人才为核心主力的人才队伍。在一批云计算行业领军人物的带领下，京东智联云技术人才队伍不断拼搏创新，实现业界领先的技术实力和服务能力。

### 完善的基础设施

京东智联云在覆盖全国的4个地域建设了多个设施先进、功能完善的IDC。地域之间通过超高带宽的骨干网络连接，形成巨大的网络数据传输优势。基于稳定可靠的基础设施，京东智联云以一流的技术和运维能力向用户提供安全、专业、稳定、便捷的云计算服务。

### 丰富的云计算产品

经过多年的努力，基于京东智联云对整个行业的深入理解，当前公有云已经为全社会贡献出种类繁多的产品和服务。京东智联云通过人工智能、大数据和物联网等行业领先的高技术产品，为用户业务的快速发展助力赋能。

### 多层次立体式场景支持

京东智联云通过功能丰富的标准产品提供IaaS、PaaS、SaaS 等全栈式云计算服务，能够很好的支持公有云、私有云、混合云、专有云等多种场景，能够对外提供IDC 业务、云计算业务、综合业务等全频段业务服务，还能够针对用户需求提供快速的定制化开发，充分满足用户对云计算的全方位需求。

### 优质的服务体系

京东智联云基于用户服务和通用技术服务等基础服务，以促进用户成功为理念，建立了金牌服务、优质架构服务、应急服务、迁移服务、系统优化服务等高技术价值服务，形成了基础稳固、技术先进、用户满意的层次化服务体系，客户服务更加专注、贴心，技术保障更加有力。

# 平台概述

京东智联云专有云平台JD Cloud Stack与京东智联云公有云平台同根同源，是面向政府和大中型企业客户的大规模商业化高端云平台。JD Cloud Stack基于京东智联云自研的云计算和大数据架构，将经过多年公有云用户实践验证的计算、网络、存储、数据库等产品，通过私有化部署帮助客户在本地自有的数据中心内搭建和京东智联云公有云计算能力相同的云计算平台。

![avatar](https://github.com/jdcloudcom/cn/blob/baishi/image/whitepaper/jdcs2.png)

JD Cloud Stack采用分层管理架构，底层支持高性能的物理服务器集群，通过计算、存储、网络层虚拟化技术对用户提供云计算服务，提供先进的安全、管理、运维、运营支撑，用户可以通过便捷友好的控制台高效管理云计算资源。JD Cloud Stack还为用户提供业界领先的网络流量接入和防护平台，提供高速、安全的网络接入支持。

JD Cloud Stack中的云计算资源产品采用“1+N”模式来实现灵活部署，“1”是最小化云平台底座，“N”是
其他可选装产品集合。客户可以通过JD Cloud Stack天然支持混合云的特性，将业务扩展到京东公有云和其他JD Cloud Stack专有云。


# 产品结构图

京东智联云专有云平台JD Cloud Stack包含了60多个云计算平台资源产品，涵盖基础资源、弹性计算、网络、存储、数据库与缓存、互联网中间件、大数据、混合云、安全、网络流量接入、用户接入、后台管理平台、运维工具等各个层次。

![avatar](https://github.com/jdcloudcom/cn/blob/baishi/image/whitepaper/jdcs3.png)

# 交付与运维
## 平台交付

根据用户的业务需求，包括业务使用场景、业务类型、及实际的需求用量等，制定平台的建设与交付方案。方案中包含平台的规划、部署排期、交付物的确认等信息。将方案部署到实际的机房环境中，并完成平台的验收测试，最终将平台提交给用户使用。京东智联云专有云平台JD Cloud Stack平台交付主要包含前期调研、机房环境部署、平台软件部署、验收测试、归档交付等步骤。

## 平台运维

京东智联云专有云平台上为云上用户提供DevOps自动化运维管理平台产品，帮助云平台上的用户更轻松的对业务系统进行运维管理和监控。DevOps自动化运维管理平台产品提供以CI/CD（持续集成、持续交付）为核心，结合代码管理、自动化测试、智能监控等的一站式DevOps服务。

![avatar](https://github.com/jdcloudcom/cn/blob/baishi/image/whitepaper/jdcs4.png)

# 典型行业解决方案
## 智慧城市专有云解决方案

![avatar](https://github.com/jdcloudcom/cn/blob/baishi/image/whitepaper/jdcs5.png)

智慧城市是现代化城市的发展方向，京东智联云为政府提供智慧城市专有云解决方案，在稳定高效、功能丰富的专有云平台JD Cloud Stack的基础上，京东智联云联合合作伙伴为城市和县区提供交通云、园区云、旅游云、能源云、教育云、融媒云、工业云、林业云、气象云、农业云等多种行业云平台。

## 企业专有云解决方案

![avatar](https://github.com/jdcloudcom/cn/blob/baishi/image/whitepaper/jdcs6.png)

由于技术水平的限制，传统的数据中心服务器的利用时间往往只有总时间的10%~20%，造成巨大的资源浪费和产生远超必需的成本。为了提升系统的数据安全性和满足合规性等目的，很多大中型企业选择采用自建数据中心承载自身的业务系统和企业管理系统。在这种场景下，京东智联云能够为大中型企业提供企业专有云解决方案，在帮助企业大幅提升资源利用率的同时有效降低企业的IT 系统成本。京东智联云基于成熟先进的专有云平台JD Cloud Stack产品，在企业客户的数据中心内实施专有云解决方案，为企业提供强大的技术能力支撑。

在底层，京东智联云为客户提供从设计、验证、实施到运维一站式的专有云JD Cloud Stack 部署服务。并结合京东智联云与合作伙伴的研发能力为企业客户提供完整的上层应用系统解决方案，帮助客户定制开发所需的应用系统和SaaS平台。京东智联云能够快速帮助企业实施采购系统、企业业务应用、企业管理平台、企业创新平台及企业成功平台等主要系统。


# 下载地址

更多详细内容请查看《京东智联云专有云JD Cloud Stack白皮书》。下载地址：http://suo.im/5W58J1


