## STB

Meeting notes for Isabella, Oliver and me

### 000. Consistent Hashing
**Meeting Date/Time:** 07/25/2021 

**Speaker:** XiuYi 

**Attendees:** Oliver, Isabella

**Meeting Notes:**

* Scalability
* 服务器的负载均衡算法
* 分布式缓存场景，3万张图片，3个缓存服务器
* 传统Hash取模算法，所有的缓存数据hash值改变，All cache miss
* 一致性hash算法，先hash服务器编号，然后hash文件/请求的名字，只有小部分缓存失效
* 数据倾斜/某台服务器宕机，请求分散
* 代码


### 001. 待定
**Meeting Date/Time:** 待定

**Speaker:**  Oliver

**Attendees:** XiuYi, Isabella


### 002. 待定
**Meeting Date/Time:** 待定 

**Speaker:**  Isabella

**Attendees:** Oliver, XiuYi


### 003. 待定
**Meeting Date/Time:** 待定 

**Speaker:** XiuYi 

**Attendees:** Oliver, Isabella
