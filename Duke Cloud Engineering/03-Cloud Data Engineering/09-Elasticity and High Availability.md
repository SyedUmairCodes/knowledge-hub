# Elasticity

Elasticity is a defining characteristic of cloud computing, allowing systems to adapt dynamically to changing demands. Elasticity is not just about **scaling up** (adding resources to handle increased load) but also about **scaling down** (removing resources when demand decreases). This dynamic adjustment of resources is crucial for cost optimization and efficient resource utilization in the cloud.

Elasticity is a key attribute of modern best practices for cloud computing.It enables organizations to optimize their infrastructure costs by aligning resource allocation with actual demand.

Conversely, when demand subsides and the CPU load drops below a certain level (e.g., 25%), the system automatically removes nodes to prevent unnecessary resource consumption. 

Elasticity is particularly valuable in scenarios with unpredictable traffic patterns, such as seasonal peaks, special events (like the Super Bowl or Christmas), or sudden surges in user activity. By automating the scaling process, organizations can ensure that their systems can handle these fluctuations without manual intervention, reducing the risk of performance degradation or outages.

# High Availability

High availability (HA) is a crucial concept in cloud computing, referring to the ability of a system to remain operational and accessible for the maximum amount of time possible, minimizing downtime. HA is often quantified using the concept of "nines" in service level agreements (SLAs). Each additional "nine" represents a significant reduction in potential downtime:

* "Five nines" (99.999%) availability translates to approximately five minutes of downtime per year.
* Amazon S3, an object storage service, is said to have "eleven nines" availability, meaning it experiences only a millisecond or so of downtime per year.

> Achieving such high levels of availability requires a robust architecture and strategies to mitigate potential points of failure. 

Redundancy is key to achieving HA. Systems are designed with multiple copies of critical components, including servers, storage, and network connections, distributed across different locations or regions. Load balancing plays a crucial role in distributing traffic across these redundant components. This ensures that if one component fails, the load can be seamlessly shifted to other operational components, preventing service interruption.

Amazon S3's high availability is achieved through a globally distributed architecture, with data replicated across multiple regions.This redundancy ensures that even if an entire region experiences an outage, the service remains accessible from other regions.