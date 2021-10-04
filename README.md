
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

## 021. 1）Joy复习Xiuyi的topics 2）多线程
**Meeting Date/Time:** 08/22/2021 

**Speaker:** Joy, Xiuyi

**Attendees:** Oliver， Isabella

**Meeting Notes:**
1) 复习topics
* 一致性hash
* 
2) 
* 
