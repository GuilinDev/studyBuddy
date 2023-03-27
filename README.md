
Meeting notes for Isabella, Oliver, Joy and me

## 000. Consistent Hashing
**Meeting Date/Time:** 07/25/2021 

**Speaker:** XiuYi 

**Attendees:** Oliver, Isabella, Joy

**Meeting Notes:**

* Scalability
* 服务器的负载均衡算法
* 分布式缓存场景，3万张图片，3个缓存服务器
* 传统Hash取模算法，所有的缓存数据hash值改变，All cache miss
* 一致性hash算法，先hash服务器编号，然后hash文件/请求的名字，只有小部分缓存失效
* 数据倾斜/某台服务器宕机，请求分散
* 代码


## 001. 1) Oliver: 缓存简介，缓存更新策略（上）; 2) Joy：DDIA第一章; 
**Meeting Date/Time:** 07/27/2021 

**Speaker:**  Oliver, Joy

**Attendees:** XiuYi, Isabella

**Meeting Notes:**

Oliver: 缓存简介，缓存更新策略（上）
* [缓存Eviction policies](https://www.educative.io/courses/grokking-the-system-design-interview/3j6NnJrpp5p)
* [缓存失效的更新，Write Through, Write Back, Write Around](https://www.educative.io/courses/grokking-the-system-design-interview/3j6NnJrpp5p)
* [扩展阅读1-Redis小结](https://zhuanlan.zhihu.com/p/59168140)
* [扩展阅读2-双写一致性方案](https://www.cnblogs.com/rjzheng/p/9041659.html)

Joy：DDIA第一章
* Reliability
* Scalability
* Maintainability


## 002. 1) push/pull & Polling; 2) Inverted Index; 
**Meeting Date/Time:** 07/30/2021 

**Speaker:**  Isabella, XiuYi

**Attendees:** Joy, Oliver

**Meeting Notes:**
 
 push/pull & Polling
* short polling/long polling/websocket
* pull/pull各自适用场景

Inverted Index
* 关键词为key，出现地方为value
* lucene，Solr/ElasticSearch

## 003. 1) 如何保证消息的时序性 2) 缓存简介，缓存更新策略（下）
**Meeting Date/Time:** 07/31/2021 

**Speaker:** XiuYi, Oliver

**Attendees:** Isabella, Joy

**Meeting Notes:**

如何保证消息的时序性
* 分布式，集群化部署
* 全局ID generator
* 离线推送

缓存简介，缓存更新策略（下）
* Weak/Eventual/Strong Consistency
* data parition - tweet id
* fail over / replication
* cache aside(write around) / write back / write through / refresh ahead

## 004. 1) API设计要点 2) BQ准备，亚麻16条领导力准则
**Meeting Date/Time:** 08/05/2021 

**Speaker:** Isabella, Xiuyi

**Attendees:** Oliver, Joy

**Meeting Notes:**

API设计要点
* RPC
* SOAP
* REST
* GraphQL

BQ准备，亚麻领导力准则
* 自我介绍
* 1）客户至上； 2） 主人翁精神； 3）创新简化； 4）决策正确

## 005. 1) SDP - Database, RDBMS, NoSQL 2) DDIA第二章
**Meeting Date/Time:** 08/08/2021 

**Speaker:**  Oliver, Joy

**Attendees:** Isabella, Xiuyi

**Meeting Notes:**
1）Oli - SDP - Database
* #1: Relational database management system (RDBMS)
  * master-master, master-slave, federation, sharding
* #2: NoSQL
  * Key-Value Store, Documentation Store, Wide-Column Store, Graph Database  
* #3: SQL or NoSQL
* [SDP](https://github.com/donnemartin/system-design-primer)

2）Joy - DDIA Chapter II 
* SQL/Nosql 
* 关系型 文档型

## 006. 1）Design Chat Service (Grokking) 2）MicroService
**Meeting Date/Time:** 08/12/2021 

**Speaker:** Joy, Isabella

**Attendees:** Oliver, Xiuyi

**Meeting Notes:**
1) Design Chat Service (Grokking)
* polling - WS
* consistency
* store - column based
* partitioning

2）MicroService
* Introduction

## 007. 1)Xiuyi讲Chat Service补漏 2) Oliver分库分表
**Meeting Date/Time:** 08/15/2021  

**Speaker:** Oliver, Xiuyi

**Attendees:** Joy, Isabella

**Meeting Notes:**
1) chat 补充
* polling and websocket
* push vs pull
* 流程图

2) 分库分表
* 策略
* join操作

## 008. 1）Joy讲IG， 2）Xiuyi复习Isabella的topics
**Meeting Date/Time:** 08/19/2021  

**Speaker:** Joy, Xiuyi

**Attendees:** Isabella, Oliver

**Meeting Notes:**
1) 
*
2) 
* 

## 009. 1）Oliver算法模板， 2）Isabella复习Joy的topics
**Meeting Date/Time:** 08/22/2021 

**Speaker:** Oliver， Isabella

**Attendees:** Joy, Xiuyi

**Meeting Notes:**
1) 算法模板
* Binary Search
* Two Pointer
* BFS
* BT/BST
* DP
* Heap
* Union Find
* Trie
2) 
* 

## 010. 1）Joy复习Oliver的topics 2）Xiuyi - Load Balancer
**Meeting Date/Time:** 08/26/2021 

**Speaker:** Joy, Xiuyi

**Attendees:** Oliver， Isabella

**Meeting Notes:**
1) From grokking
* Load Balancer
* caching
* Data Partitioning
* SQL/NoSQL
* CAP
* Long Polling, WB, Server sent events(SSE)

2) 
* Load Balancer必知必会

## 011. 1）Isabella复习Facebook message和IG
**Meeting Date/Time:** 08/29/2021 

**Speaker:**  Isabella, Oliver

**Attendees:** Joy, Xiuyi

**Meeting Notes:**
1) 
* session ID 是否可以用全局ID生成器例如Redis？
* 

## 012. 1）Desgin Youtube 2) pre sum
**Meeting Date/Time:** 09/02/2021 

**Speaker:** Joy，Oliver， 

**Attendees:** Isabella, Xiuyi

**Meeting Notes:**
1) 
* cache storage

2) 
* tech blog

## 013. 1）Notification 2) Job Scheduler
**Meeting Date/Time:** 09/05/2021 

**Speaker:** Xiuyi， Isabella

**Attendees:** Joy, Oliver

**Meeting Notes:**
1) 
*
2) 
* 

## 014. 1）Joy复习Xiuyi的topics 2）多线程
**Meeting Date/Time:** 09/10/2021 

**Speaker:** Joy, Xiuyi

**Attendees:** Oliver， Isabella

**Meeting Notes:**
1) 复习topics
* 一致性hash
* Inverted Index
* Cookie, Session, Token
* Load Balancer
2) 
* 

## 015. 1）Isabella复习Xiuyi的topics 
**Meeting Date/Time:** 09/12/2021 

**Speaker:** Isabella

**Attendees:** Joy, Xiuyi 

**Meeting Notes:**
1) 复习topics
* 
2) 
* Learn and Be Curious
* Earn Trust

## 016. 1）Tiny URL 2）Typeahead
**Meeting Date/Time:** 09/17/2021 

**Speaker:** Joy, Oliver

**Attendees:** Xiuyi, Isabella

**Meeting Notes:**
1) Tiny URL
* 不同短网址在不同网站上，检测访问量
* 一个长网址对应多个短网址(Cassandra等column based)
* 服务器和用户可设置过期时间，不能被猜到
* hash function
* Key generation Service生成短网址的letters， 6个8个等
2) Typeahead
* 

## 017. 1）网络安全基础 2）Design Parking lot
**Meeting Date/Time:** 09/19/2021 

**Speaker:** Xiuyi, Isabella

**Attendees:** Oliver， Joy

**Meeting Notes:**
1) 
* 
2) 
* 

## 018. 1）图论，DP基础 2）Union Find
**Meeting Date/Time:** 09/28/2021 

**Speaker:** Joy, Isabella

**Attendees:** Oliver， Xiuyi

**Meeting Notes:**
1) 图论入门
* Queue
* Priority Queue
2) Union Find
* 

## 019. 1）设计KV Store
**Meeting Date/Time:** 09/30/2021 

**Speaker:**  Xiuyi

**Attendees:** Oliver，Joy, Isabella and many others

**Meeting Notes:**
1) 设计KV Store
* 
* 
2) 
* 

## 020. 1）Grokking新的topics 2）Design Rate Limiter 3)
**Meeting Date/Time:** 08/22/2021 

**Speaker:** Joy, Isabella, Oliver

**Attendees:** Xiu Yi

**Meeting Notes:**
1) 
* Redundancy (server) and Replication(data)
* Bloom Filters - 不为1肯定没有，为1不保证一定有
* Quorum
* Leader and Follower
* Heartbeat
* Checksum - 对TCP/UDP的报文段进行校验/检测nodes之间数据复制是否完整
2) Design Rate Limiter
* Token bucket
* 
3) 
* 

## 021. 1）Isabella复习LB/Consistent Hashing/Partitioning,Sharding 2）Blind 75
**Meeting Date/Time:** 10/07/2021 

**Speaker:**  Isabella, Oliver

**Attendees:** Joy, Xiuyi

**Meeting Notes:**
1) 
* 
* 
2) 
* 


## 022. 1）亚麻领导力LP学习4条
**Meeting Date/Time:** 10/12/2021 

**Speaker:**  Xiuyi 

**Attendees:**  Isabella, Oliver

**Meeting Notes:**
1) 
* Learn and Be Curious 好奇求知
* Hire and Develop The Best 选育贤能
* Insist on the Highest Standards 最高标准
* Think Big 远见卓识


## 023. 1） Design Pastebin 2）复习2
**Meeting Date/Time:** 10/14/2021 

**Speaker:**  Joy，Isabella

**Attendees:** Xiuyi

**Meeting Notes:**
1) 
* paste table + user table
* clean service
2) 
* peer to peer / master slave
* Cahce （缓存淘汰策略，缓存与DB一致性问题 - 先更新DB再删缓存，脏数据最少）

## 024. 1）API的设计 2）读书分享 - Working Effectively with Legacy Coding第一章
**Meeting Date/Time:** 10/19/2021 

**Speaker:**  Xiuyi, Oliver

**Attendees:** Isabella

**Meeting Notes:**
1) 
* 
* 
2) 
* 

## 025. 1）Design Dropbox 2）Idempotency幂等
**Meeting Date/Time:** 10/21/2021 

**Speaker:**  Joy, Xiuyi

**Attendees:** Oliver, Isabella

**Meeting Notes:**
1) 
* 
* 
2) 
* 

## 026. 1）Review basics III - databases 2）读书分享 - Working Effectively with Legacy Coding第二章
**Meeting Date/Time:** 10/24/2021 

**Speaker:**  Isabella, Oliver

**Attendees:** Joy, Xiuyi

**Meeting Notes:**
1) 
* 
* 
2) 
* 

## 027. 1）Mock Job Scheduler 2）Distirbuted Lock
**Meeting Date/Time:** 10/31/2021 

**Speaker:**  Isabella, Xiuyi

**Attendees:** 

**Meeting Notes:**
1) 
* 
* 
2) 
* 

## 028. 1）设计Twitter的补充 2）TopK的设计 3) Multi-threading
**Meeting Date/Time:** 11/07/2021 

**Speaker:**  Joy, Isabella, Xiuyi

**Attendees:** 

**Meeting Notes:**
1) 
* tweets的Sharding - 雪花算法ID
* Cache
* Twitter Search
2) 
* MapReduce
* Count-min Setch
3) 
* 可重入性的问题

## 029. 1）Mock Interview设计Amazon Price Tracker
**Meeting Date/Time:** 11/14/2021 

**Speaker:**  Xiuyi

**Attendees:** Isabella, Joy, Oliver

**Meeting Notes:**
1) 
Amazon price tracker

1k products

requirements: 

1) grab the prices and store prices somewhere

2) we pop these date to customers

Amazon prices -> services to grab the prices -> to our own stores - > services to fetch data from our stores -> pop up for 
ASAP for real time for customer needs

1) pay Amazon to use APIs to get data - alternative for others, we may can use crawlers

2) rest/graphQL APIs to get data in our gateway layers - json objects

3) middle ware service to clean/aggregate/cluster data - pre-compute

4) store

shcema:

	Product: productID, categoryID, price, timestamp;
	
	Price: ID, productID, Array{{price1, time1},{price2, time2},{price3, time3}...}
	
	Category: ID, categoryNames....
	
```sql
Select price From Product Where ProductID = "123" 
```

5) sevices to grab data and do some computing - pick some products/category,save them in the cache -> speed reading for new customers

6) pop to clients

authozation -> free -> can access some limited resources (e.g, overal category prices change in past three months) vs VIP users (have more accesses to all tracks, like all historical data changes for all produces)

![架构图](/meetingPPT/imgs/029Arch.png)

## 030. 1）点赞系统 2）Kafka入门图解
**Meeting Date/Time:** 11/18/2021 

**Speaker:**  Isabella, Xiuyi

**Attendees:** Joy, Oliver

**Meeting Notes:**
1) 
* 
* 
2) 
* kafka不在一个consumer group的消费者怎么消费同一个消息？

## 031. 1）Design slack - 0
**Meeting Date/Time:** 12/02/2021 

**Speaker:**  Xiuyi

**Attendees:** Isabella, Oliver

**Meeting Notes:**
1) 
* 
* 
2) 
* 

## 032. 1）Neayby Friend; 2) 点赞系统 - 续 3) Manage up
**Meeting Date/Time:** 12/05/2021 

**Speaker:**  Joy, Isabella, Xiuyi

**Attendees:** Oliver

**Meeting Notes:**
1) 
* Quad Tree
* 
2) 
*
3)
*

## 033. 1）[Counting system](https://medium.com/pinterest-engineering/building-a-real-time-user-action-counting-system-for-ads-88a60d9c9a
); 2) GeoHash 
**Meeting Date/Time:** 12/05/2021 

**Speaker:**  Isabella, Xiuyi

**Attendees:** Joy, Oliver

**Meeting Notes:**
1) 
* 
* 
2) 
*
3)
*

## 034. 1）Partition之前的一些策略; 2) Design Snapchat/instagram Stories 3) DDIA summary - ch 1,2
**Meeting Date/Time:** 12/05/2021 

**Speaker:**  Joy, Isabella, Xiuyi

**Attendees:** Jasmine

**Meeting Notes:**
1) 
* 
* 
2) 
*
3)
*

## 035. 1）Design What's up app 2) Distributed System Summary + k8s
**Meeting Date/Time:** 01/02/2022

**Speaker:**   Isabella, Xiuyi

**Attendees:** 

**Meeting Notes:**
1) 
* 
* 
2) 
*

## 036. 1）Design What's up app - leftover 2) DDIA ch 3
**Meeting Date/Time:** 01/09/2022

**Speaker:**   Isabella, Xiuyi

**Attendees:** Joy, Oliver, Jasmine

**Meeting Notes:**
1) 
* 
* 
2) 
*

## 037. 1）DDIA ch 4 2) In Memory DB 3) Design Leetcode
**Meeting Date/Time:** 01/16/2022

**Speaker:** Xiuyi, Nick, Isabella

**Attendees:** Joy

**Meeting Notes:**
1) 
* 
* 
2) 
*
3)


## 038. 1）Twitter Architecture
**Meeting Date/Time:** 01/23/2022

**Speaker:** Xiuyi

**Attendees:** Jasmine, Nick, Isabella, Oliver

**Meeting Notes:**
1) 
* 
* 
2) 
*
3)


## 039. 1）Zero Copy 2) Apache Flink 3) Cost Efficiency @ Scale in Big data File Format
**Meeting Date/Time:** 01/30/2022

**Speaker:** Xiuyi, Isabella, Oli

**Attendees:** Jasmine, Nick, Joy

**Meeting Notes:**
1) 
* 
* 
2) 
* https://developer.aliyun.com/article/666052?spm=a2c6h.13262185.0.0.4c7b7e18EzjqIJ

3)
* https://eng.uber.com/cost-efficiency-big-data/

## 040. 1）即时通讯系统y 2) SQL to NoSQL 3) WebAssembly
**Meeting Date/Time:** 02/06/2022

**Speaker:** Nick, Joy

**Attendees:** Jasmine, Vickie, Isabella, Oli, Xiuyi

**Meeting Notes:**
1) 
* 
* 
2) 
* 

3)


## 041. 1）Webassembly
**Meeting Date/Time:** 02/10/2022

**Speaker:** Xiuyi

**Attendees:** Jasmine, Vickie, Isabella, Oli, Nick, Joy, wenruo

**Meeting Notes:**
1) 
* 
* 
2) 
* 

3)
* 

## 042. 1）Apache Beam
**Meeting Date/Time:** 02/20/2022

**Speaker:** Xiuyi

**Attendees:** Jasmine, Isabella, Oli, Nick, Joy, wenruo

**Meeting Notes:**
1) 
* Python版本的'|'问题，应该是语法糖两个进程通信，而不是位操作的或操作
* 
2) 
* 

3)
* 

## 043. 1）FB Outage on 10/04/2021 2) Idempotency - 上
**Meeting Date/Time:** 02/27/2022

**Speaker:** Wenruo, Isabella

**Attendees:** Xiuyi, Nick, Jasmine, Vickie

**Meeting Notes:**
1) 
* 
* 
2) 


## 044. 1）DDIA Ch 5 - 1 2) SP and Trigger 3) MVND
**Meeting Date/Time:** 03/06/2022

**Speaker:** Nick, Joy, Xiuyi

**Attendees:** Wenruo, Isabella, Xiuyi, Jasmine, Vickie

**Meeting Notes:**
1) 
* Kafka从2.4版本开始可以从followers中读取数据，之前版本只能从leader中读；正常的数据库一般是leader只负责写入
* WAL vs binlog
2) 
*
3)


## 045. 1）DDIA Ch 5 - 2 2) Lyft Beam 
**Meeting Date/Time:** 03/13/2022

**Speaker:** Ning, Xiuyi

**Attendees:** Yu, Xiuyi, Wenruo, Isabella, Jasmine, Vickie

**Meeting Notes:**
1) 
* 
* 
2) 
*
3)


## 046. 1）Docker - 上 2) Idempotency - 下
**Meeting Date/Time:** 03/20/2022

**Speaker:** Xiuyi, Isabella， 

**Attendees:** Ning,  Yu, Xiuyi, Wenruo, , Jasmine, Vickie

**Meeting Notes:**
1) 
* 
* 
2) 
* pre-PRC, rpc, post-RPC transaction最后一个步骤失败了怎么办？
* Transaction的操作顺序问题
* master和replicas在payments中同步问题
3)


## 047. 1）Inorder 2) clean code 3) Payment system - 上
**Meeting Date/Time:** 03/27/2022

**Speaker:** Wenruo, Oli Xiuyi

**Attendees:** Ning, Yu, Joy, Isa, Jasmine

**Meeting Notes:**
1) 
* 
* 
2) 
* 
3)


## 048. 1）Inorder Payment system - 下
**Meeting Date/Time:** 04/03/2022

**Speaker:** Xiuyi

**Attendees:** Yu, Joy, Isa, Jasmine, Wenruo, Oli

**Meeting Notes:**
1) 
* 是否可以将Kafka的partition指定给consumer消费？
* 

## 049. 1）PostgresSQL 2) Webhooks
**Meeting Date/Time:** 04/10/2022

**Speaker:** Isabela Xiuyi

**Attendees:** Yu, Jasmine, Wenruo, Yibo, Vickie

**BQ topics - customer obsession**
* Who was your most difficult customer?
* Give me an example of a time when you did not meet a client’s expectation. What happened, and how did you attempt to rectify the situation?
* When you’re working with a large number of customers, it’s tricky to deliver excellent service to them all. How do you go about prioritizing your customers’ needs?
* Tell the story of the last time you had to apologize to someone.

**Meeting Notes:**
1) 
* 
* 

## 050. 1）TCP - DB connections
**Meeting Date/Time:** 04/17/2022

**Speaker:** 

**Attendees:** Isabela, Xiuyi, Yu, Jasmine, Wei, Yibo, Vickie

**Meeting Notes:**
1) 
* RST ARK


## 051. 1）支持亿级流量的高并发IM架构 2) OpenAPI简介
**Meeting Date/Time:** 04/24/2022

**Speaker:** Yu, Xiuxi

**Attendees:** Isabela, Jasmine, Wei, Wenruo, Nick, Oli

**Meeting Notes:**
1) 
* 
2)
* resources

## 052. 1）Learning OAuth2.0 2) DDIA Chapter 6
**Meeting Date/Time:** 04/24/2022

**Speaker:** Wei, Nick

**Attendees:** Yu, Xiuxi, Isabela, Jasmine, Yibo, Wenruo, Oli

**Meeting Notes:**
1) 
* 
2)
* resources

## 053 1) Design chat system. 
**Meeting Date/Time:** 08/28/2022

**Speaker:** Joy 

**Attendees:** Yu, Xiuxi, Isabela, Jasmine, Yibo, Wenruo, Oli

**Meeting Notes:**
1) Meeting Notes:
Types of connections:
1. short polling; (close right after response)
2.long polling; (long and will timeout)
3.WebSocket. (Bi-directional and persistent)
High-level design:
Stateless:
User > LB > services (AMI, Service discovery, User service, Group service)
Stateful:
via WS
Storage:
KV stores 用于水平scaling
KV store 低延迟。
关系型搞不定长尾问题。索引也是坑的一笔。
Table 设计:
dbo.[message] dbo.[group_message]
只要保证group范围内ID唯一，即可躺平。

2) 1.Message 1 to 1 chat workflows,
重点是有个message queue。面向消息队列编程。
2. 如何跨设备同步，实现统一通信？
手机PC（都记录各自收到哪一条了）然后都通过Chat Server1的session来catch up。
3. Small Group chat workflow：
重点是有message queue，
发是发给queue，
收也是收那个queue。
4. Online Presence如何隐身
5s一个heartbeat，30s就当他掉了。
PS: WB开销很大，只考虑建立给active chatting，timeout即可回收资源。

3) Meeting Note三
1.Online Status fanout
Pub-sub模式
更新在线状态非常昂贵，让他们自己手动pull？
Wrap up
加分题：
1.支持文字以外的多媒体。
2.端到端加密。小心老旧机型性能问题。。。
3.Caching。历史数据本地存着？
3. 关系数据库可以存下用户，setting等比较stable的基本数据（靠谱便于维护）。但是像一条条的即时消息，必须上KV store。
4.服务发现
PS：面试时把replica放在back pocket就好。太细节不用摆在桌面。
PS：拜占庭共识？？？
* 

* resources

## 056. 1）Jeopardy Game
**Meeting Date/Time:** 09/25/2022

**Speaker:** XiuYi

**Attendees:** Yu, Wei, Isabela, Vickie, Joy, Yibo, Oli, O.O, Wen, Ju, zhengda

**Meeting Notes:**
1) 
* [Jeopardy Game 1](https://jeopardylabs.com/play/2022-09-24-222)

1. Num!
Isabella
Ju

2. Top1
Joy
Zhengda

3. 找工作
Wei
Wen
Yuan

4. YYV
Yu
Yibo
Vickie

## 067. 1）Design Web Crawler 2) 
**Meeting Date/Time:** 10/02/2022

**Speaker:** Zhengda Wu

**Attendees:** Yu, Wei, Isabela, Guilin, Yibo, Oli, Ning, Joy, Yuan

**Meeting Notes:**
1) Design a web crawler （搜索引擎）
* 如何防止死循环
* MapReduce
* NoSQL存储
* 抓取的数据隔一段时间不同如何处理？ - timestamp
* PageRank
* Load Balancer算法
* 缓存的地方（浏览器。redis，数据库层， CDN， Application）
* Web Server/API Server
* 分布式爬虫? 数以亿计的网站
* crawler在背后一直run，起点是什么？ - 有一些种子links，公司自己定；
* 热门网站如何决定 - 热门网站放在queues里面（deep dive）
* 反爬机制 - 文件/协议

## 068. 1）Design Web Crawler - 上 2) 
**Meeting Date/Time:** 10/09/2022

**Speaker:** Joy, Ding

**Attendees:** Yu, Wei, Isabela, Guilin, Ning, Yuan, Zhengda，Oli

**Meeting Notes:**
1) Design a web crawler 
* 种子URLs - 根据场景来选择
* 准备download的 - URL frontier
* content比较防止重爬 - 文字比对效率太低，利用Hashing结果来对比，MD5比较慢，MurmurHash或者JenkinsHash可用，Lucene用的Lookup3Signature（by JenkinsHash）
* 比对hashing结果非常相近的时候，是否存两次或相同对待；只存关键词和links - fingerprints
* Inverted Indices - 索引关键词，部分网页存cache大部分不存网页本身内容（no content storage）
* 
2) Ding Q&A
* 国内国外工作最大的不同 - 科技类公司，国内工作怕普遍强度高很多
* 

## 069. 1）Prometueus理解和实战
**Meeting Date/Time:** 10/16/2022

**Speaker:** Xiuyi

**Attendees:**  Isabela, Oli, Ning, Ding, Zhengda

**Meeting Notes:**
1) Prometheus + Grafana + SpringBoot
* 联邦监控
* tombstones文件
* Prometheus高级功能

## 070. 1）Design Web Crawler - 下 
**Meeting Date/Time:** 10/23/2022

**Speaker:** Joy

**Attendees:**  Isabela, Xiuyi, Oli, Ning, Ding, Zhengda

**Meeting Notes:**
1) Design Web Crawler - 下
* DFS vs BFS
* Queue Selector - 设定优先级
* 防扒机制 - 大网站
* 不同domain但内容相同 - filter
* Spider Traps - 黑名单
* 两个queues存放问题


## 071. 1）Review Consistent Hashing 和 KV store
**Meeting Date/Time:** 10/30/2022

**Speaker:** Joy

**Attendees:**  Isabela, Xiuyi, Ning, Yu, Wei, Zhengda, Oli

**Meeting Notes:**
1) 
* 

## 072. 1）Prometueus告警实战
**Meeting Date/Time:** 11/13/2022

**Speaker:** Xiuyi

**Attendees:**  Isabela, Oli, Ning, Yu, Zhengda, Joy

**Meeting Notes:**
1) Prometheus + Grafana + Kafka
* SlackBot token
* 
## 073. 1）如何画架构图 - C4 Model
**Meeting Date/Time:** 11/20/2022

**Speaker:** Xiuyi

**Attendees:**  Isabela, Wei, Yuan, Yu, Joy, Oli

**Meeting Notes:**
1) 
* 通常我们会到container（起始）和component（局部展开）这两层

## 074. 1）Design Metrics and Alerting System
**Meeting Date/Time:** 12/04/2022

**Speaker:** Xiuyi

**Attendees:**  Isabela, Wei, Ning, Yu, Joy, Oli, Zhengda

**Meeting Notes:**
1)

## 075. 1）DDIA - Chapter 3 Storage and Retrieval
**Meeting Date/Time:** 12/11/2022

**Speaker:** Wei

**Attendees:**  Isabela, XiuYi, Ning, Yuan, Joy, Oli, Zhengda

**Meeting Notes:**
1) [DDIA第三章笔记](https://github.com/GuilinDev/Notes/blob/master/SystemDesign/DDIA_Chapter03_Notes.md)

## what is clustered index?

## 076. 1）RDBMS Index
**Meeting Date/Time:** 12/18/2022

**Speaker:** XiuYi

**Attendees:**  Isabela, Wei, Ning, Yu

**Meeting Notes:**
1) Index的创建和使用
```sql
-- 创建Person表
SHOW DATABASES;
USE testdb;

drop table IF EXISTS `person`;
create TABLE `person`
(
    `id`          bigint(20)   NOT NULL AUTO_INCREMENT,
    `name`        varchar(255) NOT NULL,
    `score`       int(11)      NOT NULL,
    `create_time` timestamp    NOT NULL,
    PRIMARY KEY (`id`),
    KEY `name_score` (`name`, `score`) USING BTREE,
    KEY `create_time` (`create_time`) USING BTREE
) ENGINE = InnoDB
  DEFAULT CHARSET = utf8mb4;

-- 在本地机器上，循环sp创建100K测试数据，with MySQL8.0.31
-- maintain cost
create
    DEFINER = `root`@`localhost` PROCEDURE `insert_person`()
begin
    declare c_id integer default 1;
    while c_id <= 100000
        do
            insert into person values (c_id, concat('name', c_id), c_id + 100, date_sub(NOW(), interval c_id second));
            set c_id = c_id + 1;
        end while;
end;


-- space cost
select round(((DATA_LENGTH) / 1024 / 1024), 3)  `Data size in MB`,
       round(((INDEX_LENGTH) / 1024 / 1024), 3) `Index size in MB`
from information_schema.TABLES
where TABLE_NAME = 'person';
-- retrieves rows from a table using an index cost
explain select * from person where NAME = 'name1';
explain select NAME, SCORE from person where NAME = 'name1';

-- 索引匹配列前缀
EXPLAIN SELECT * FROM person WHERE NAME LIKE '%name123' LIMIT 100; -- not use index
EXPLAIN SELECT * FROM person WHERE NAME LIKE 'name123%' LIMIT 100; -- use index
-- where后的条件语句
EXPLAIN SELECT * FROM person WHERE LENGTH(NAME) = 7;

-- Joint Index只用一个
EXPLAIN SELECT * FROM person WHERE SCORE > 45678; -- not use index
EXPLAIN SELECT * FROM person WHERE NAME LIKE 'NAME45%'; -- use index
EXPLAIN SELECT * FROM person WHERE SCORE > 45678 AND NAME LIKE 'NAME45%'; -- use index

SHOW TABLE STATUS LIKE 'person';

-- check places for optimization
SET optimizer_trace="enabled=on";
SELECT * FROM person WHERE NAME >'name84059' AND create_time>'2022-12-17 15:00:00';
SELECT * FROM information_schema.OPTIMIZER_TRACE;
SET optimizer_trace="enabled=off";
``````

## 077. 1）AWS Services
**Meeting Date/Time:** 01/08/2023

**Speaker:** Xiuyi

**Attendees:**  Isabela, Wei, Ning, Yu, Joy, Oli, Zhengda, Jasmine

**Meeting Notes:**
1) geohash vs google s2 vs quadra tree


## 078. 1）Proximity Service
**Meeting Date/Time:** 01/22/2023

**Speaker:** Joy

**Attendees:**  Isabela, Wei, Ning, Yu, Xiuyi, Oli

**Meeting Notes:**
1) Proximity Service (Yelp)
2) 

## 079. 1）Nearby Friends/People within x miles
**Meeting Date/Time:** 01/29/2023

**Speaker:** Joy

**Attendees:**  Isabela, Wei, Ning, Yu, Xiuyi, Zhengda, Oli

**Meeting Notes:**
1) peer to peer vs shared backend
2) service discovery

## 080. 1）DDIA - Chapter 5 Replication
**Meeting Date/Time:** 02/05/2023

**Speaker:** Wei

**Attendees:**  Joy, Isabela,  Ning, Yu, Xiuyi, Zhengda, Oli

**Meeting Notes:**
1) Leaders and Followers replication
2) Single Leader replication Logs: Statement based logging; Write ahead logging(WAL); logical (row based) logging; Trigger based logging
3) Multi-leader replication: Performance; Conflict resolution;  Network;
  * Conflict-free replicated data types (CRDTs);
  * Mergeable persistent data structures (MPDSs);
  * Operational transformation (OT);
4) Leaderless replication: 

## 081. 1）Review System Design basics
**Meeting Date/Time:** 02/12/2023

**Speaker:** Isabela

**Attendees:**  Joy, Yu, Xiuyi, Zhengda, Oli

**Meeting Notes:**
1) Load Balancer - Least connection/Least response time/Least Bandwidth/Least Packets/Round Robin/Weighted Round Robin/IP Hash/URL Hash
2) Cache - Client side cache/CDN/Server side cache, Global cache/Distributed Cache (with Request Cache), Local cache
  * Cache Invalidation - Write through (Cache and DB sametime)/Write Around (Write only DB)/Write Back (Write Cache first and then DB)/Cache Aside (Read from Cache first, if not found, read from DB and then write to Cache)
  * Cache Eviction - FIFO/LIFO/LRU/LFU/MRU/RR
  * 先更新数据库再更新缓存 vs 先删除缓存再更新数据库 vs 先更新数据库再删除缓存 （根据不用的use cases来选择）

## 082. 1）Docker Full Course 101
**Meeting Date/Time:** 02/19/2023

**Speaker:** Xiuyi

**Attendees:**  Joy, Yu, Ning, Zhengda, Oli, Jasmine, Isabella

**Meeting Notes:**
1) Container - hotfix mechanism; which to control this process
2) Docker uses Linux Container on Windows - LCOW (not Linux Container - LXC, LCOW refers Hyper-V) to run Linux containers on Windows 
2) TODO: K8S

## 083. 1）Google Map (from Alex Xu)
**Meeting Date/Time:** 02/26/2023

**Speaker:** Joy

**Attendees:**  Joy, Yu, Xiuyi, Ning, Oli, Jasmine, Isabella

**Meeting Notes:**
1) Functional Requirements: User location service, Navigation service including ETA, Map redering
2) Non-functional Requirements: Accuracy, Smoothness, Data and Battery usage, General Availability and scalability
3) Map 101: Geocoding vs Reverse Geocoding; Geohashing, Map rendering (Hirachical routing tiles: zoom in/out, 4个方向，小块为4的n次方)
4) Road data processing for navigation service: Dijistra algorithm, A* algorithm
5) Google Map Architecture: 
  * Frontend: Map rendering, Navigation, Search, User location service
  * Backend: Map data, Navigation data, Search data, User location data
  * Map data: Map tiles, Map features, Map labels, Map images
  * **Navigation Service**: Navigation routes, Navigation labels, Navigation images
  * Search data: Search index, Search labels, Search images
  * **User location Service**: User location, User location labels, User location images
  * CDN for location service
6) Data Models: Routing tiles/Object DB(s3), , user location data/column based(cassandra), geocoding data路的信息/redis, map tiles图片信息
7) Shortest-path service - A* algorithm, BFS
8) ETA service, Ranking service, Updator service
9) Delivery protocol: Websocket, Server-Send Events(SSE)

## 084. 1）Learn Design Patterns
**Meeting Date/Time:** 03/05/2023

**Speaker:** Joy

**Attendees:**  Yu, Xiuyi, Isabella, Ruichen, Zhengda, Joy, Ning, Oli

**Meeting Notes:**
1) SOLID
2) Proxy Pattern
3) Command Pattern

## 085. 1）Cache
**Meeting Date/Time:** 03/12/2023

**Speaker:** Isabella

**Attendees:**  Yu, Xiuyi, Zhengda, Ning, Joy

**Meeting Notes:**
1) Recovery Time Objective (RTO) vs Recovery Point Objective (RPO)
2) Weak consistency vs Strong consistency
3) Reverse Proxy vs Forward Proxy
4) Redis vs Other in-memory cache
5) [supplement - Crash cource in Caching](https://blog.bytebytego.com/p/a-crash-course-in-caching-part-1)

## 085. 1）Kubernetes 101 - 0
**Meeting Date/Time:** 03/19/2023

**Speaker:** Xiuyi

**Attendees:**  Isabella, Yu, Ruichen, Ning, Joy, Oli

**Meeting Notes:**
1) Is K8s Node same as distributed system Node?
2) How do K8s nodes isaolate from each other?
3) sidecar pattern

## 085. 1）Design Distributed MQ
**Meeting Date/Time:** 03/26/2023

**Speaker:** Joy

**Attendees:**  Isabella, Xiuyi, Yu, Zhengda, Oli

**Meeting Notes:**
1) [Design Distributed MQ](https://www.youtube.com/watch?v=Z3X1YQ1YJ0A)
2) Benefits of Distributed MQ
3) 