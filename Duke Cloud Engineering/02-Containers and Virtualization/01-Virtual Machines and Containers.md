# Virtual Machines
Virtual machines (VMs) allow you to run a guest operating system inside of a host operating system.

One use case for virtual machines is running older applications, that you may not want to modify but still need to run in your environment. An example of a monolithic application is an older PHP content management system or web framework.

You could also use a virtual machine to run a specific operating system when your host operating system is different. For example, you can run Linux on a Mac OS 10 host operating system using a virtual machine.
# Containers
Containers are a lightweight way to package your application and its dependencies. They are similar to virtual machines but offer significant advantages.

- Containers include only the runtime and code necessary for your application to run. This makes them significantly smaller and faster than virtual machines
- Containers launch very quickly, in milliseconds, while virtual machines can take seconds to minutes to start.
- Containers are highly portable. Because they are not tied to a specific operating system, they can be easily moved between different environments.
- Containers are well-suited for cloud-native development and micro services.
# Differences

| **Feature**           | **Virtual machines**                                                                                                                                                                                                                       | **Containers**                                                                                                                                                                 |
| --------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| Underlying technology | Virtual machines (VMs) are an older technology that simulates a physical computer system. A VM includes a full copy of the guest operating system, including the kernel, libraries, and system tools, on top of the host operating system. | Containers, provide a more lightweight virtualization approach. They share the host operating system's kernel but isolate the application's code, libraries, and dependencies. |
| Startup time          | VMs have a boot time that ranges from seconds to minutes, as they need to load an entire operating system.                                                                                                                                 | Containers start much faster, often in milliseconds, because they don't have to boot a separate OS and only need to load the application and its dependencies                  |
| Use cases             | VMs are mostly used for running legacy monolithic applications that require an older version of the libraries it runs on.                                                                                                                  | Containers are a good choice for modern, cloud-native applications, especially those built using a microservices architecture.                                                 |
| Security              | VMs provide strong isolation because the guest operating system is entirely separated from the host operating system.                                                                                                                      | While containers offer some level of isolation, they share the host OS kernel, which can potentially create security vulnerabilities if not properly configured.               |
