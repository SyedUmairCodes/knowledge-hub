# CAP Theorem
The CAP theorem is a fundamental concept in distributed systems that explains the trade-offs between three desirable properties: consistency, availability, and fault tolerance. The theorem states that it is impossible to achieve all three of these properties simultaneously in a distributed system. You can only guarantee two out of the three. 

- Consistency means that all clients or users of the system see the same data at the same time, even if they are accessing the system from different locations or if there are concurrent updates happening.
- Availability refers to the system's ability to respond to requests in a timely manner, even if some components of the system are down or experiencing failures.
- Fault tolerance means that the system can continue to operate and provide service even if some of its components or network connections fail.

> The choice of which properties to prioritize depends on the specific needs of the application. For instance, banking systems cannot compromise on consistency, while social media platforms might prioritize availability.
