# Designing Data-Intensive Applications
    
## Part 1
1. <ins>Chapter 1</ins>
   * <ins>Reliability:</ins> Is the property of a system to function correctly, even when faced with faults like hardware failures, software bugs, or human errors. A reliable system ensures that users can depend on it to behave as expected without loss of data or disruption of service.<br>
     <ins>Key aspects of ensuring reliability include:</ins>
     * Handling Faults Gracefully:
       1. Faults can arise due to hardware failures, network issues, or software bugs. 
       2. Reliable systems anticipate these faults and are designed to recover or handle them without affecting the user experience.
     * Redundancy:
       1. Replicating data and services ensures that a single failure does not bring down the system. 
       2. Examples include using database replicas or distributed systems.
     * Durability:
       1. Once data is written, it should not be lost, even if a failure occurs. 
       2. Techniques like backups and write-ahead logs help ensure durability.
     * Testing and Monitoring:
       1. Automated testing and real-time monitoring can help detect and resolve issues before they escalate.
      
     > Reliability is ensuring that systems remain functional and resilient in the face of failures, software bugs, and human errors.
     
   * <ins>Scalability:</ins> Is the system’s ability to handle increasing amounts of load efficiently by adapting its resources accordingly. A scalable system can accommodate growth in data volume, traffic, or computational demands without a significant drop in performance. <br>
     <ins>Key aspects of Scalability</ins>
     * Describing Load: Load refers to the demand placed on a system, and it needs to be measured to determine how well a system scales. Common metrics used to describe load include:
       1. Requests per second (RPS) – Number of user requests handled by an application.
       2. Read vs. write ratio – How many operations are read-heavy vs. write-heavy.
       3. Data storage size – The amount of data a system needs to manage.
       4. Concurrent users – Number of users interacting with the system simultaneously.
     * Describing Performance: Performance measures how quickly the system responds under a given load. Important performance metrics include:
       1. Latency – The time it takes to process a request (e.g., database query time).
       2. Throughput – The number of requests a system can handle per unit of time.
       3. Response time distribution – Rather than focusing only on average response time, systems should analyze percentiles (e.g., 95th or 99th percentile) to understand worst-case delays.
     * Approaches for Coping with Load: When a system experiences higher load, there are two fundamental approaches to scaling:
       1. Scaling Up (Vertical Scaling)
          - Involves upgrading a single machine with more CPU, RAM, or storage.
          - Simpler but has hardware limits and can be expensive.
          - Example: Moving a database from a small instance to a more powerful one in AWS (e.g., upgrading an RDS instance).
       2. Scaling Out (Horizontal Scaling)
          - Distributes load across multiple machines (servers or nodes).
          - More cost-effective and resilient to failure.
          - Requires load balancers and distributed systems.
          - Example: Using multiple database replicas for read-heavy applications.

     > Scalability is about ensuring that as load increases, performance remains stable by implementing appropriate scaling strategies. A well-designed scalable system uses a mix of vertical and horizontal scaling, caching, load balancing, and asynchronous processing to handle growing workloads efficiently.   
        
   * <ins>Maintainability:</ins>
   
2. <ins>Chapter 2</ins>

3. <ins>Chapter 3</ins>

4. <ins>Chapter 4</ins>

## Part 2

## Part 3