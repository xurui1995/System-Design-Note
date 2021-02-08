# System-Design-Note




### Scalability

* Performance refers to the capability of a system to provide a certain response time. server a defined number of users or process a certain amount of data. So performance is a software quality metric. Unlike to what many people think it is not vage, but can be defined in numbers.

* Scalability referes to the characteristic of a system to increase performance by adding additional ressources. Very often people think that there system are scalabable out-of-the-box. “If we need to serve more users, we just add additional server” is a typical answer for performance problems.

* Explanation from edu: Scalability is the capability of a system, process or a network to grow and manage increased demand. Any distributed system that can continuously evolve in order to support the growing amount of work is considered to be scalable.

| Horizontal        | Vertical   |
| --------   | -----:  |
| Load balancing required     | N/A|   
| Resilient       |   single point   |  
| network calls (RPC)        |    Inter process communication    |  
| data inconsistency       |    consistent   |  
| scale well as users increase       |    hardware limit   |  

### Reliability
* Reliability is the probability a system will fail in given period. In simple terms, a distributed system is considered reliable if it keeps delivering it's service even when some components fail, any failing machine can always be replaced by another healthy one, ensuring the completion of the requested task

### Availability
* Availability is the time a system remains operational to perform its required function in a specific period. It is a simple measure of percentage of time that a system,service or a machine remains operational under normal conditions.

* Reliability is availability over time considering the full range of possible real-world conditions that can occur. An aircraft that can make is through any possible weather safely is more reliable than one that vulnerabilities to possible conditions

* If a system is reliable, it is available. However, if it is available, it is not necessary reliable.

### Efficiency
* response time

### Serviceable or Manageability
* how easy the system is to operate and maintain. (error notification)


## Load Balancing
* Load Balancing is the process of distributing traffic across multiple servers or databases.
* Important benefits: faster,uninterrupted service, avoid single point failure
* Load balancing algorithms (health checks): least connection method, least response time method, round robin method, weight round robin, Ip hash.

## Cache
* principle: recently requested data us likely to be requested again.
* CDN
* Cache invalidation write-through、write-around、write-back
* Cache eviction policies： FIFO LRU MRU...

