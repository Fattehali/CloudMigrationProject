To begin with migration plan we are currently working on the IT landscape, we are dealing with monolithic ERP system which are characterized by the performance issue, scalability limitation, security risk and so on.

So our migration strategy is to perform either a refactoring or a rehosting

## Migration phases
### 1.	Planning and assessment
### Inventory of Resources:
Tools: Use Google Cloud Migrate for  all on-premises workload

Analyze current workloads with Google Cloud Migrate, including the SQL database cluster, mainframe, e-commerce apps, monolithic ERP, and 150 virtual machines.

VMs: Examine the 150 virtual machines (Windows Server and Linux) to record information about installed apps, CPU, memory, and storage usage, and OS versions.

Monolithic ERP System: Determine the database connections, system components, and particular dependencies (such as on other virtual machines or apps).

Determine the web servers, application servers, and backend connections that make up e-commerce applications.

SQL Database Cluster: Compile data on dependencies, transaction rates, schema, and database size.








## 	Estimate Costs 
Use the cloud provider's pricing calculator to estimate migration and operational costs.



##  Assumptions:
•	Compute Engine VMs: Assumed 5 instances of n1-standard-4 type running continuously.

•	GKE: A cluster with 3 nodes of n1-standard-4 type, operating 24/7.
•	Cloud SQL: One db-n1-standard-4 instance with 500 GB SSD storage and high availability enabled.

•	Cloud Spanner: Configured with 2 nodes and 500 GB storage.
•	BigQuery: 1 TB of storage with 5 TB of data processed in queries per month.

•	Cloud Storage: 2 TB of standard storage with specified operations.

•	Cloud VPN: Two VPN tunnels with 1 TB of egress traffic per month.

•	Cloud Load Balancer: Two forwarding rules handling 5 TB of ingress traffic monthly.

•	Cloud Pub/Sub: Handling 10 million messages totaling 100 GB of data per month.

•	Cloud Operations Suite: Monitoring 150 GB and logging 100 GB of data monthly.




