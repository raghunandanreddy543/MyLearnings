
## Performance Tuning
-   **Database Configuration Tuning.**
	-    The optimum configuration for your organizational workload. Among other things, we examine the block size of different file systems like ZFS, and recommend optimum configuration.
-   **Index Analysis.** 
	-   Indexes can be tricky to handle, especially as your data grows. We analyze your existing indexes and suggest any optimizations. In addition to that, we recommend the addition/removal of indexes according to your organizational needs.
-   **Table Partition Analysis.** 
	-   Table partitions are essential to data management and maximizing efficiency when accessing that data. We analyze and recommend the addition/removal of partitions based on your workloads.
-   **Hardware Usage Analysis.** 
	-   In order to fully utilize the hardware your database is hosted on, we study the configuration and recommend changes which will ensure full utilization of the power your hardware provides.
-   **Connection Pooling Review.** 
	-   Many users and applications will connect to the database to perform functions they are responsible for; we review your connection pooling strategy to ensure that it’s optimized for your specific use case.
-   **Analysis of Slow Running Queries.** 
	-   If there are specific queries that you feel are running slower than expected, we perform a detailed analysis to identify potential optimizations accordingly.
-   **Operating System Configuration Tuning.** 
	-   The OS forms the underlying layer of your database, so configuration parameters for the OS and the hardware it’s hosted on should also be customized for your organizational workload. Among other things, we can use pg_buffercache as our guide and make recommendations about shared_buffer parameter setting to optimize for your workload.
-   **Storage Partition Analysis.**
	-    Building on the OS configuration, storage disk partitions also tend to play a significant role in the performance of any software the OS hosts. We examine existing partitions and provide recommendations on their configuration and structure that will enhance processing efficiency.