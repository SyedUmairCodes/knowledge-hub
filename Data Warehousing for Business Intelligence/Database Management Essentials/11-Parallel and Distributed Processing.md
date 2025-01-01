Parallel and distributed processing are two methods of utilizing multiple computing resources to improve performance and availability, but they differ significantly in their approach and goals.
Parallel Database Processing
●
Definition: Parallel database processing divides a large task into smaller tasks and distributes these among interconnected computers to improve performance. It focuses on using multiple resources (processors, disks, and memory) to perform a single task faster. This is often done using tightly coupled resources with high-speed networks.
●
Goals: The primary goals are to achieve speedup (performing a task faster) and scaleup (performing more work in the same time). It also aims to increase availability by dynamically adjusting to the level of available resources.
○
Speedup is about completing a single task more quickly by using more resources.
○
Scaleup is about increasing the amount of work completed by increasing computing capacity while holding completion time constant. For ideal linear scaleup, increasing computing capacity n times allows completion of n times the amount of work in the same time.
●
Architectures: Common architectures include:
○
Shared Disk (SD): Each processor has its own memory, but the processors share access to all disks.
○
Shared Nothing (SN): Each processor has its own memory and disks. Data must be partitioned among the processors.
○
Clustered Disk (CD): Processors in each cluster share all disks, but nothing is shared across clusters.
○
Clustered Nothing (CN): Processors in each cluster share no resources, but each cluster can be manipulated to work in parallel.
●
Implementation: Parallel DBMSs are designed to use a collection of resources in parallel. They use high-speed networks and storage systems to coordinate work among resources.
●
Transparency: Resource sharing is typically transparent to applications. Application code (SQL and programming language statements) does not need to be changed to take advantage of parallel processing.
●
Challenges: Load balancing (evenly distributing work among processors), cache coherence (maintaining data consistency across multiple caches), and interprocessor communication (synchronizing actions of independent processors) are key challenges.
●
Commercial examples include Oracle Real Application Clusters using the CD architecture and IBM DB2 with the DPF option using the CN architecture.
●
Big Data: Parallel processing is also crucial for handling big data. Tools like Hadoop, MapReduce, Spark, and Hawq enable parallel processing of large, unstructured datasets that are not well-suited to traditional DBMS queries.
Distributed Database Processing
●
Definition: Distributed processing involves the distribution of tasks and data among computers connected by a network. It focuses on enabling different sites to cooperate in providing access to data. It is used to allow local control of data, reduce communication costs, and improve performance.
●
Goals: The primary goals are to provide local control of data, reduce communication costs by locating data closer to where it’s used, and improve performance by allowing multiple sites to work concurrently. Increased data availability is another goal.
●
Architecture: A distributed database has a component architecture composed of local data managers (LDM) at each site, and a distributed data manager (DDM) that manages global requests. The schema architecture includes a global conceptual schema and local schemas for each site.
●
Implementation: Distributed database systems must manage data that are located at different network sites. These systems must handle global requests (queries or transactions that access data at multiple sites).
●
Tightly vs. Loosely Integrated Systems: Tightly integrated systems have homogeneous local DBMSs which allow for more efficient processing of distributed queries and transactions. Loosely integrated systems support data sharing among a mix of modern and legacy DBMSs.
●
Transparency: Transparency refers to the visibility (or invisibility) of the internal details of a service. Levels of transparency include:
○
Fragmentation Transparency: Users can write queries without knowledge of how the data is divided into fragments.
○
Location Transparency: Users do not need to know the physical locations of the data.
○
Local Mapping Transparency: Users are aware of the site names but do not need to know how data are fragmented within each site.
●
Challenges: Distributed database design is complex. Poor design can lead to higher communication costs and poor performance. Distributed transaction processing can add significant overhead, especially for replicated data. Security is a major concern, as multiple sites must be protected from unauthorized access.
●
Query Processing: Distributed query processing involves both local and global optimization, and it must take data movement and site selection into account.
●
Transaction Processing: Distributed transaction processing ensures the ACID properties but introduces new challenges like coordinating across independent sites and handling network failures.
Key Differences
●
Autonomy: Distributed databases provide site autonomy, while parallel databases do not. Autonomy means that each site has local control over its data and operations.
●
Focus: Parallel processing focuses on speeding up a single task by using multiple processors. Distributed processing focuses on allowing multiple sites to cooperate, often for local control and reduced communication costs.
●
Complexity: Distributed databases introduce added complexities like handling data replication and ensuring consistency across multiple sites. Parallel databases focus on optimizing performance in a more tightly controlled environment.
●
Transparency: While parallel processing usually emphasizes transparency, distributed processing provides different levels of transparency, allowing users to be aware of the distributed nature to varying degrees.
●
Network Characteristics: Parallel database processing assumes fast and reliable communication networks, while distributed database processing must cope with networks that may have higher latency and be less reliable.
In summary, parallel processing is about speeding up a single task, while distributed processing is about enabling multiple independent sites to work together. Parallel processing uses tightly coupled resources, while distributed processing uses geographically dispersed resources. Both methods are crucial for modern database management but serve different purposes and have different implementation challenges.