# AWS Well-Architected Framework: Performance Efficiency Pillar

**Total Best Practices:** 34

---

## Architecture selection

### Selection process

#### PERF01-BP01: Learn about and understand available cloud services and features

**Description:** Continuously learn about available services and features to understand how they can improve performance efficiency for your workload.

**AWS Documentation:** [PERF01-BP01](https://docs.aws.amazon.com/wellarchitected/latest/framework/perf_architecture_understand_cloud_services_and_features.html)

---

#### PERF01-BP02: Use guidance from your cloud provider or an appropriate partner to learn about architecture patterns and best practices

**Description:** Use cloud company resources, such as solutions architects, professional services, or appropriate partners, to guide your architecture decisions.

**AWS Documentation:** [PERF01-BP02](https://docs.aws.amazon.com/wellarchitected/latest/framework/perf_architecture_guidance_architecture_patterns_best_practices.html)

---

#### PERF01-BP03: Factor cost requirements into decisions

**Description:** Take cost into consideration as you select and configure resources. For example, Amazon RDS can be more cost-effective than a self-managed database.

**AWS Documentation:** [PERF01-BP03](https://docs.aws.amazon.com/wellarchitected/latest/framework/perf_architecture_factor_cost_decisions.html)

---

#### PERF01-BP04: Use policies or reference architectures

**Description:** Maximize the performance and efficiency benefits of resources in the cloud by using architectural patterns and policies based on guidance from your cloud provider.

**AWS Documentation:** [PERF01-BP04](https://docs.aws.amazon.com/wellarchitected/latest/framework/perf_architecture_trade_offs_impact_customers.html)

---

#### PERF01-BP05: Use benchmarking to drive architectural decisions

**Description:** Use internal benchmarking and external analysis or resources, such as published case studies, to drive your architectural choices.

**AWS Documentation:** [PERF01-BP05](https://docs.aws.amazon.com/wellarchitected/latest/framework/perf_architecture_use_policies_reference_architectures.html)

---

#### PERF01-BP06: Use a data-driven approach for architectural choices

**Description:** In AWS, all resources are available as programmable data, which means you can apply a data-driven approach to help improve the performance efficiency of your workload.

**AWS Documentation:** [PERF01-BP06](https://docs.aws.amazon.com/wellarchitected/latest/framework/perf_architecture_use_benchmarking_drive_decisions.html)

---

### Compute architecture

#### PERF02-BP01: Select the best compute options for your workload

**Description:** The optimal compute choice for a workload varies based on application design, usage patterns, and configuration settings. Select compute options aligned with your workload.

**AWS Documentation:** [PERF02-BP01](https://docs.aws.amazon.com/wellarchitected/latest/framework/perf_compute_hardware_select_best_compute_options.html)

---

#### PERF02-BP02: Understand the available compute configuration options

**Description:** Understand the different configuration options available for compute to make sure you select the one that best meets your workload needs.

**AWS Documentation:** [PERF02-BP02](https://docs.aws.amazon.com/wellarchitected/latest/framework/perf_compute_hardware_understand_compute_configuration_features.html)

---

#### PERF02-BP03: Collect compute-related metrics

**Description:** One of the best ways to understand how your compute systems are performing is to record and track key metrics that are related to compute resources.

**AWS Documentation:** [PERF02-BP03](https://docs.aws.amazon.com/wellarchitected/latest/framework/perf_compute_hardware_collect_compute_metrics.html)

---

#### PERF02-BP04: Configure and right-size compute resources

**Description:** Configure compute resources in a manner that matches your performance requirements and adjust their size dynamically to meet changing demands.

**AWS Documentation:** [PERF02-BP04](https://docs.aws.amazon.com/wellarchitected/latest/framework/perf_compute_hardware_right_size.html)

---

#### PERF02-BP05: Use the available elasticity of resources

**Description:** AWS provides you the flexibility to expand or reduce dynamically your resources to meet changes in your workload demands.

**AWS Documentation:** [PERF02-BP05](https://docs.aws.amazon.com/wellarchitected/latest/framework/perf_compute_hardware_elasticity.html)

---

#### PERF02-BP06: Use optimized hardware-based compute accelerators

**Description:** Use hardware accelerators to perform some functions more efficiently than is possible when using general-purpose processors, such as GPUs for graphics processing or FPGAs.

**AWS Documentation:** [PERF02-BP06](https://docs.aws.amazon.com/wellarchitected/latest/framework/perf_compute_hardware_use_hardware_accelerators.html)

---

#### PERF02-BP07: Use the appropriate scaling mechanism

**Description:** Implement the appropriate scaling strategy to meet your workload's performance objectives. Scaling can be either horizontal or vertical.

**AWS Documentation:** [PERF02-BP07](https://docs.aws.amazon.com/wellarchitected/latest/framework/perf_compute_hardware_scaling_policies.html)

---

### Storage architecture

#### PERF03-BP01: Understand storage characteristics and requirements

**Description:** Understand the different storage characteristics and requirements to select the services that best fit your workload, such as object, block, and file storage.

**AWS Documentation:** [PERF03-BP01](https://docs.aws.amazon.com/wellarchitected/latest/framework/perf_data_use_purpose_built_data_store.html)

---

#### PERF03-BP02: Evaluate available configuration options

**Description:** Evaluate the various characteristics and configuration options available for storage services and understand how they relate to your workload requirements.

**AWS Documentation:** [PERF03-BP02](https://docs.aws.amazon.com/wellarchitected/latest/framework/perf_data_evaluate_config_options_data_store.html)

---

#### PERF03-BP03: Make decisions based on access patterns and metrics

**Description:** Choose storage systems based on your workload access patterns and configure them by determining how the workload accesses data.

**AWS Documentation:** [PERF03-BP03](https://docs.aws.amazon.com/wellarchitected/latest/framework/perf_data_collect_data_store_metrics.html)

---

#### PERF03-BP04: Implement strategies to improve query performance

**Description:** Implement strategies such as caching, read replicas, and indexing to improve query performance and reduce latency.

**AWS Documentation:** [PERF03-BP04](https://docs.aws.amazon.com/wellarchitected/latest/framework/perf_data_implement_strategy_improve_query_performance.html)

---

#### PERF03-BP05: Collect and record storage performance metrics

**Description:** Track key metrics to understand the performance of your storage system. Use this data to optimize storage configuration and make informed decisions.

**AWS Documentation:** [PERF03-BP05](https://docs.aws.amazon.com/wellarchitected/latest/framework/perf_data_review_data_store_metrics.html)

---

#### PERF03-BP06: Configure and right-size storage resources

**Description:** Size storage to match workload needs to optimize costs without impacting performance. Right-size storage systems for capacity, throughput, and IOPS.

**AWS Documentation:** [PERF03-BP06](https://docs.aws.amazon.com/wellarchitected/latest/framework/perf_data_right_size_data_store.html)

---

#### PERF03-BP07: Use the available elasticity of resources

**Description:** Use storage that can scale to meet your changing needs. Cloud storage systems can elastically scale to handle growing data and changing workload requirements.

**AWS Documentation:** [PERF03-BP07](https://docs.aws.amazon.com/wellarchitected/latest/framework/perf_data_elasticity_data_store.html)

---

### Database architecture

#### PERF04-BP01: Understand data characteristics

**Description:** Understand data characteristics including: structure, velocity, volume, transactional vs analytical requirements, object size, access patterns, latency, throughput, and durability.

**AWS Documentation:** [PERF04-BP01](https://docs.aws.amazon.com/wellarchitected/latest/framework/perf_database_use_purpose_built_database.html)

---

#### PERF04-BP02: Evaluate the available options

**Description:** Evaluate database and storage services available on AWS for your workload. The optimal database solution varies based on requirements for availability, consistency, partition tolerance, latency, durability, scalability, and query capability.

**AWS Documentation:** [PERF04-BP02](https://docs.aws.amazon.com/wellarchitected/latest/framework/perf_database_evaluate_config_options.html)

---

#### PERF04-BP03: Collect and record database performance metrics

**Description:** Use tools and metrics to understand database performance. Metrics like queries per second, latency of queries, and CPU and memory utilization help you understand if performance is meeting requirements.

**AWS Documentation:** [PERF04-BP03](https://docs.aws.amazon.com/wellarchitected/latest/framework/perf_database_collect_metrics.html)

---

#### PERF04-BP04: Choose data storage based on access patterns

**Description:** Use multiple purpose-built data stores and optimize each data store with the access patterns required by your workload. For example, choose analytical and transactional stores differently.

**AWS Documentation:** [PERF04-BP04](https://docs.aws.amazon.com/wellarchitected/latest/framework/perf_database_select_based_access_patterns.html)

---

#### PERF04-BP05: Optimize data storage based on access patterns and metrics

**Description:** Optimize data storage configuration to match access patterns. Use caching, read replicas, database sharding, and data partitioning to improve performance.

**AWS Documentation:** [PERF04-BP05](https://docs.aws.amazon.com/wellarchitected/latest/framework/perf_database_optimize_storage.html)

---

#### PERF04-BP06: Implement strategies to improve query performance

**Description:** Use strategies such as key distribution, caching, partitioning, and data compression to improve query performance. Consider connection pooling and query optimization.

**AWS Documentation:** [PERF04-BP06](https://docs.aws.amazon.com/wellarchitected/latest/framework/perf_database_optimize_query_performance.html)

---

### Network architecture

#### PERF05-BP01: Understand how networking impacts performance

**Description:** Understand network characteristics including latency, throughput, jitter, and bandwidth to effectively optimize network resources for your workload.

**AWS Documentation:** [PERF05-BP01](https://docs.aws.amazon.com/wellarchitected/latest/framework/perf_networking_understand_network_requirements.html)

---

#### PERF05-BP02: Evaluate available networking features

**Description:** Evaluate networking features that increase performance. Measure the impact of these features through testing. Network protocols, dedicated vs shared connectivity, frame sizes, network management, and placement groups can impact performance.

**AWS Documentation:** [PERF05-BP02](https://docs.aws.amazon.com/wellarchitected/latest/framework/perf_networking_use_networking_features.html)

---

#### PERF05-BP03: Choose appropriately sized dedicated connectivity or VPN for hybrid workloads

**Description:** When there is a requirement for on-premises communication, make sure that you have adequate bandwidth for workload performance. A single dedicated connection or multiple connections may be needed.

**AWS Documentation:** [PERF05-BP03](https://docs.aws.amazon.com/wellarchitected/latest/framework/perf_networking_choose_hybrid_network.html)

---

#### PERF05-BP04: Use load balancing to distribute traffic across resources

**Description:** Distribute traffic across multiple resources or services to allow your workload to take advantage of the elasticity that AWS provides. You can also use load balancing for offloading encryption termination.

**AWS Documentation:** [PERF05-BP04](https://docs.aws.amazon.com/wellarchitected/latest/framework/perf_networking_choose_load_balancing_dns.html)

---

#### PERF05-BP05: Choose network protocols to improve performance

**Description:** Make decisions about protocols for communication between systems and networks based on the impact on workload performance. Using less verbose protocols, caching, and connection pooling can improve performance.

**AWS Documentation:** [PERF05-BP05](https://docs.aws.amazon.com/wellarchitected/latest/framework/perf_networking_choose_network_protocols.html)

---

#### PERF05-BP06: Choose your workload's location based on network requirements

**Description:** Use the AWS Region, Availability Zones, placement groups, and edge locations such as AWS Outposts, AWS Local Zones, and AWS Wavelength that allow you to run applications close to end users.

**AWS Documentation:** [PERF05-BP06](https://docs.aws.amazon.com/wellarchitected/latest/framework/perf_networking_choose_location_placement.html)

---

#### PERF05-BP07: Optimize network configuration based on metrics

**Description:** Use collected and analyzed data to make informed decisions about optimizing your network configuration. Measure the impact of those changes and use the impact measurements to make future decisions.

**AWS Documentation:** [PERF05-BP07](https://docs.aws.amazon.com/wellarchitected/latest/framework/perf_networking_measure_monitor_network_performance.html)

---

#### PERF05-BP08: Use dedicated connectivity and network devices when required

**Description:** When deploying mission-critical workloads to AWS, consider deploying resources that provide dedicated capacity and throughput, such as AWS Direct Connect or enhanced networking with the Elastic Network Adapter.

**AWS Documentation:** [PERF05-BP08](https://docs.aws.amazon.com/wellarchitected/latest/framework/perf_networking_use_dedicated_connectivity.html)

---
