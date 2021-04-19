


## <img src="assets/info-circle-solid.svg" width="30px"> 个人信息

<table style="border: none;margin-left: auto; margin-right: auto;">
    <tr style="border: none;">
        <td style="border: none;">
            姓名：王鹤涵
        </td>
        <td style="border: none;">
            年龄：28
        </td>
    </tr>
     <tr style="border: none;">
        <td style="border: none;">
            学历：本科
        </td>
        <td style="border: none;">
            工作年限：6年
        </td>
    </tr>
    <tr style="border: none;">
        <td style="border: none;">
            电话：17600108055
        </td>
        <td style="border: none;">
            邮箱：524259885@qq.com
        </td>
    </tr>
</table>

## <img src="assets/tools-solid.svg" width="30px"> 技能清单

- **熟练掌握** Java编程(JUC,JVM)，Spring全家桶(Spring Cloud)，Mybatis，Mybatis-Plus等框架的使用。阅读过部分源码，提交过Mybatis-Plus框架pr。
- **熟练掌握** Mysql ，Redis等数据库，Kakfa等常用MQ的优化。
- **熟练掌握** 常用设计模式 ，常用重构手法的使用。https://www.edrawsoft.cn/viewer/public/s/8c21b017655819
- **熟悉掌握** 数据结构与算法 ，基本Linux命令，阅读英文文档无障碍。
- **熟悉掌握** Netty,Vertx等响应式编程框架 并基于Zk+Netty实现了简单的rpc框架 https://github.com/hehan-wang/LightRpc
- **基本掌握** Clickhouse，MongoDB等数据库的使用。Docker，K8s，Gitlab CI/CD的使用。Golang开发。

## <img src="assets/briefcase-solid.svg" width="30px"> 工作经历

- **乐元素科技有限公司，广告投放部门，高级Java开发工程师，2019.12~至今**
    1. 乐投广告投放平台后端架构搭建。
    2. 一周内从0学习并搭建K8s+Gitlab CI/CD 自动化容器部署。
    3. 两周内从0学习Golang并使用异步编程完成打点SDK的编写。
    4. 编写Java异步打点SDK 并封装成spring-boot-starter自动装配使用。
    5. 完成在线项目不停机迁移数据库(使用队列+双写+代理)。
    
- **上海太睿科技有限公司，产品研发部门，开发组长，2019.06~2019.12**
    1. 穿云箭微服务平台架构搭建以及编写。   
    
    2. 协调开发，测试，上线整体流程。
    
- **上海魔邑诚广告有限公司，产品研发部门，Java开发，2016.12~2019.06**
    1. 效果类DSP Golden Traffic(投放微博 B站 陌陌等HERO APP) 投放引擎以及管理后台编写。
    
    2. 海外API 管理后台的编写。
    
- **北京凯新科技有限公司，产品研发部门，后端开发，2015.07~2016.12**
    1. 参与部分项目的概要设计，详细设计，需求文档的编写。
    2. 对任务模块进行代码设计与实现及单元测试。

## <img src="assets/project-diagram-solid.svg" width="30px"> 项目经历

- **乐投广告平台(2019.12~至今)**  

  * **技术选型：** Spring-boot,Vue,Mybatis-plus,Docker,k8s,Gitlab CI/CD,Mysql,Redis,Rabbitmq,Clickhouse

  * **项目介绍： ** 该平台提高广告投放成效（类似于监测归因平台）。对接三方Marketing API 拉取媒体成本等数据，以及实时收集广告点击数据与公司数仓中的新增设备**匹配归因**后，统计ROI等指标导入Clickhouse以报表形式展现。提供广告投放需要的一系列工具等功能。

  * **责任描述：** 任务模块以及api模块开发，技术选型，项目搭建，测试上线。

  * **项目难点：** 

    1. 多地部署架构：由于管理系统在国内，对外接口服务分部在国内海外，采用了多地部署架构。所有的写请求使用RPC调用主库节点的写服务，从库节点Mysql通过binlog同步主库节点的数据。
    2. 幂等设计：由于网络波动等原因RPC存在失败重试。使用Redis存储幂等号来实现下游幂等，防止数据重复
    3. 外部接口不一致：由于对接媒体众多以及各家媒体协议完全不一致，使用策略模式(借助spring工厂)对接多个媒体，使新接入一个媒体的成本降低到最小。

  * **成果收获：**

    3. 归因模块数据库不停机迁移。

    4. 可以帮助解决团队内很多业务和技术问题，系统保质保量完成。

       

- **穿云箭平台(2019.06~2019.12)**

  * **技术选型：** Spring-cloud-alibaba(nacos,feign,gateway),Mybatis-Plus,Docker,Mysql,Redis,Mongodb,Rabbitmq,Nginx,Spring-security-oauth

  * **项目介绍：** 该平台为程序化购买TD（Trading Desk）平台。对接多家Marketing API批量创建广告，拉取广告报表等功能一站式投放平台。

  * **责任描述：** 需求分析 库表设计 项目搭建 项目开发 协调开发测试上线

  * **项目难点：** 

    1. 开发周期短：产品需求会讨论 Backlog，评估所有功能实现切分Story。一周一个Sprint，把本周的Story拆分成Task。每日站立会同步开发进度。完成的Task同步产品同学并行测试。Bug优先级高的优先解决，优先级不高的跟下次上线一起测试。

  * **成果收获：**

    1. 由于开始做之前考虑的多以及使用一些设计模式使代码易扩展易维护，在初期仅有两名开发 后期只有4名开发的情况下依然按时上线。

    2. 一个人从0搭建一套微服务架构，以及整个小组业务开发进度。

       

- **GT DSP投放引擎(2018.01~2019.6)**

  * **技术选型：** Vertx,Guice,Docker,Redis,RocktsDB,Kafka
  
  * **项目介绍：** 该系统为DSP投放引擎，负责接受媒体传过来的竞价/展示/点击请求，以及上报点击请求到广告主并接受广告主的激活归因结果。
  
    1. 使用响应式编程框架Vertx组件搭建整个项目。
    2. 使用Guice管理模块依赖。
    3. Redis作为与业务模块交互的数据总线。
    4. RocktsDB存储海量的设备包信息。
    5. 请求响应原始日志落Kafka用来做监控，回溯。
  
  * **责任描述：** 项目搭建，维护，ADX对接
  
  * **项目难点：** 
  
    1. 高并发：使用基于多路复用IO的Netty的响应式编程框架Vertx，一个线程管理多个连接提高QPS。
    2. 低延迟：由于RTB广告要求响应时间在100ms以下，要求投放引擎读写低延迟，采取了读纯内存的Redis，批量顺序写磁盘的Kafka，读LSM-Tree+BloomFilter结构的RocksDB降低RT
  
  * **成果收获：**
    
    1. 使用vertx支撑单节点7000+qps。
    
    2. 对RTB理解加深 可以承担RTB广告整体开发。
    
       
  
- **Mex ADX(2017.01~2018.1)**

  * **技术选型：** Vertx,Guice,Docker,Redis,Kafka
  * **项目介绍：** 该系统为ADX广告交易平台。对接SSP/ADX流量方，放给下游DSP/ADX。
    1. 根据DSP设施的QPS和前置定向信息过滤可用的DSP列表
    2. 发送BidRequest接受BidResponse
    3. 校验BidResponse格式
    4. 处理竞价取第二高价
    5. 处理价格的宏替换发送给DSP win-notice/impression
  * **责任描述：** 项目维护，媒体对接
  * **项目难点：** 
    1. 高并发，低延迟
  * **成果收获：**
    1. 熟悉响应式编程思路
    2. 了解adx实现逻辑

## <img src="assets/graduation-cap-solid.svg" width="30px"> 教育经历

- 本科，沈阳工业大学，电气工程及其自动化专业，2011.9~2015.7


## <img src="assets/rss-solid.svg" width="30px"> 自我评价

 - 责任心强 能吃苦 有团队意识。遵循团队开发规范并加入自身思考。
 - 有学习能力 适应能力强  喜欢研究技术 能很快融入新项目。
 - 对自己产出项目质量有一定要求。选用合适的技术选型以及设计模式。
 - **Stay hungry、stay foolish.**

