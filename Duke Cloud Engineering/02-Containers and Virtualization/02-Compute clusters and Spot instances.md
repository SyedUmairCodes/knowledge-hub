# Spot instances
Spot instances are a cost-saving way to run virtual machines (VMs) on Amazon Web Services (AWS). They allow you to bid on unused EC2 capacity, which can result in savings of up to 90% compared to on-demand pricing.

When you request a spot instance, you specify the maximum price you're willing to pay per hour. This is your "bid." AWS then launches the instance if your bid exceeds the current spot price for the instance type and Availability Zone you've selected.

>[!info]
>It's important to understand that spot prices are dynamic and can fluctuate in real-time based on supply and demand.

If the spot price exceeds your bid, AWS may terminate your instance with a two-minute warning. This is a key consideration when deciding if spot instances are right for your workloads.

# Azure Compute Clusters
Azure Compute Clusters are a type of virtual machine offering from Microsoft Azure specifically designed for demanding computational tasks, such as machine learning model training. They provide a way to create a group of interconnected virtual machines that can work together as a single unit.

Compute Clusters are recommended to be used with bursting workloads and machine learning training.

>[!info]
>Bursting refers to the ability to scale computing resources up or down quickly based on demand.

Similar to other Azure virtual machine offerings, you can choose between CPUs and GPUs for your Compute Clusters. This choice depends on the specific requirements of your workload. Compute Clusters offer the flexibility to select the priority of your virtual machines. You can choose between dedicated or low-priority.



