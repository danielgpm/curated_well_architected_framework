# AWS Well-Architected Framework: Reliability Pillar

**Total Best Practices:** 65

---

## Foundations

### Manage service quotas and constraints

#### REL01-BP01: Aware of service quotas and constraints

**Description:** Be aware of your default quotas and manage your quota increase requests for your workload architecture. Know which cloud resource constraints, such as disk or network, are potentially impactful.

**AWS Documentation:** [REL01-BP01](https://docs.aws.amazon.com/wellarchitected/latest/framework/rel_manage_service_limits_aware_quotas_and_constraints.html)

---

#### REL01-BP02: Manage service quotas across accounts and regions

**Description:** If you are using multiple AWS accounts or AWS Regions, make sure you request the appropriate quotas in all environments in which you plan to run your production workloads.

**AWS Documentation:** [REL01-BP02](https://docs.aws.amazon.com/wellarchitected/latest/framework/rel_manage_service_limits_limits_considered.html)

---

#### REL01-BP03: Accommodate fixed service quotas and constraints through architecture

**Description:** Be aware of unchangeable service quotas and physical resources, and architect to prevent these from impacting reliability.

**AWS Documentation:** [REL01-BP03](https://docs.aws.amazon.com/wellarchitected/latest/framework/rel_manage_service_limits_aware_fixed_limits.html)

---

#### REL01-BP04: Monitor and manage quotas

**Description:** Evaluate your potential usage and increase your quotas appropriately, allowing for planned growth in usage.

**AWS Documentation:** [REL01-BP04](https://docs.aws.amazon.com/wellarchitected/latest/framework/rel_manage_service_limits_monitor_manage_limits.html)

---

#### REL01-BP05: Automate quota management

**Description:** Implement tools to alert you when thresholds are being approached. You can automate quota increase requests by using Service Quotas APIs.

**AWS Documentation:** [REL01-BP05](https://docs.aws.amazon.com/wellarchitected/latest/framework/rel_manage_service_limits_auto_monitor_manage_limits.html)

---

#### REL01-BP06: Ensure that a sufficient gap exists between the current quotas and the maximum usage to accommodate failover

**Description:** When a resource fails, it may still be counted against quotas until its successfully terminated. Ensure that your quotas cover the overlap of all failed resources with replacements before the failed resources are terminated.

**AWS Documentation:** [REL01-BP06](https://docs.aws.amazon.com/wellarchitected/latest/framework/rel_manage_service_limits_suff_buffer_limits.html)

---

### Plan network topology

#### REL02-BP01: Use highly available network connectivity for your workload public endpoints

**Description:** These endpoints and the routing to them must be highly available. To achieve this, use highly available DNS, content delivery networks (CDNs), API Gateway, load balancing, or reverse proxies.

**AWS Documentation:** [REL02-BP01](https://docs.aws.amazon.com/wellarchitected/latest/framework/rel_planning_network_topology_ha_conn_users.html)

---

#### REL02-BP02: Provision redundant connectivity between private networks in the cloud and on-premises environments

**Description:** Use multiple AWS Direct Connect (DX) connections or VPN tunnels between separately deployed private networks. Use multiple DX locations for high availability.

**AWS Documentation:** [REL02-BP02](https://docs.aws.amazon.com/wellarchitected/latest/framework/rel_planning_network_topology_ha_conn_private.html)

---

#### REL02-BP03: Ensure IP subnet allocation accounts for expansion and availability

**Description:** Amazon VPC IP address ranges must be large enough to accommodate workload requirements, including factoring in future expansion and allocation of IP addresses to subnets across Availability Zones.

**AWS Documentation:** [REL02-BP03](https://docs.aws.amazon.com/wellarchitected/latest/framework/rel_planning_network_topology_ip_subnet.html)

---

#### REL02-BP04: Prefer hub-and-spoke topologies over many-to-many mesh

**Description:** If more than two network address spaces (for example, VPCs and on-premises networks) are connected via VPC peering, AWS Direct Connect, or VPN, then use a hub-and-spoke model, like that provided by AWS Transit Gateway.

**AWS Documentation:** [REL02-BP04](https://docs.aws.amazon.com/wellarchitected/latest/framework/rel_planning_network_topology_prefer_hub.html)

---

#### REL02-BP05: Enforce non-overlapping private IP address ranges in all private address spaces where they are connected

**Description:** The IP address ranges of each of your VPCs must not overlap when peered or connected via VPN. You must similarly avoid IP address conflicts between a VPC and on-premises environments or with other cloud providers.

**AWS Documentation:** [REL02-BP05](https://docs.aws.amazon.com/wellarchitected/latest/framework/rel_planning_network_topology_no_overlap_ip.html)

---

## Workload architecture

### Design workload service architecture

#### REL03-BP01: Choose how to segment your workload

**Description:** Workload segmentation is important when determining the resilience requirements of your application. Monolithic architectures should be avoided. Instead, carefully consider which application components can be broken into microservices.

**AWS Documentation:** [REL03-BP01](https://docs.aws.amazon.com/wellarchitected/latest/framework/rel_service_architecture_monolith_soa_microservice.html)

---

#### REL03-BP02: Build services focused on specific business domains and functionality

**Description:** Service-oriented architectures (SOA) and microservices build services with well-delineated functions defined by business needs. Microservices use domain-driven design to identify these functions.

**AWS Documentation:** [REL03-BP02](https://docs.aws.amazon.com/wellarchitected/latest/framework/rel_service_architecture_business_domains.html)

---

#### REL03-BP03: Provide service contracts per API

**Description:** Service contracts are documented agreements between producers and consumers that define functional interfaces and include availability and performance SLAs. A contract versioning strategy allows consumers to continue using the existing API and migrate their applications to a newer API when they are ready.

**AWS Documentation:** [REL03-BP03](https://docs.aws.amazon.com/wellarchitected/latest/framework/rel_service_architecture_api_contracts.html)

---

## Change management

### Design interactions to prevent failures

#### REL04-BP01: Identify the kind of distributed systems you depend on

**Description:** Distributed systems include services, applications, and cloud resources that your workload depends upon. Understanding dependencies allows you to choose interaction patterns that increase reliability.

**AWS Documentation:** [REL04-BP01](https://docs.aws.amazon.com/wellarchitected/latest/framework/rel_prevent_interaction_failure_distributed_system.html)

---

#### REL04-BP02: Implement loosely coupled dependencies

**Description:** Dependencies such as queuing systems, streaming systems, workflows, and load balancers are loosely coupled. Loose coupling helps isolate behavior of a component from other components that depend on it, increasing resiliency and agility.

**AWS Documentation:** [REL04-BP02](https://docs.aws.amazon.com/wellarchitected/latest/framework/rel_prevent_interaction_failure_loosely_coupled.html)

---

#### REL04-BP03: Do constant work

**Description:** Systems can fail when there are large, rapid changes in load. A system that constantly polls or send messages is more reliable than one that only does work in response to infrequent requests.

**AWS Documentation:** [REL04-BP03](https://docs.aws.amazon.com/wellarchitected/latest/framework/rel_prevent_interaction_failure_constant_work.html)

---

#### REL04-BP04: Make mutating operations idempotent

**Description:** An idempotent service promises that each request is processed exactly once, such that making multiple identical requests has the same effect as making a single request. This makes it easier for a client to implement retries without fear that a request is erroneously processed multiple times.

**AWS Documentation:** [REL04-BP04](https://docs.aws.amazon.com/wellarchitected/latest/framework/rel_prevent_interaction_failure_idempotent.html)

---

### Implement change

#### REL08-BP01: Use runbooks for standard activities such as deployment

**Description:** Runbooks are documented procedures to achieve specific outcomes. Enable consistent and prompt responses to well-understood events by documenting procedures in runbooks.

**AWS Documentation:** [REL08-BP01](https://docs.aws.amazon.com/wellarchitected/latest/framework/rel_tracking_change_management_use_runbooks.html)

---

#### REL08-BP02: Integrate functional testing as part of your deployment

**Description:** Functional tests are run as part of automated deployment. If success criteria are not met, the pipeline is halted or rolled back.

**AWS Documentation:** [REL08-BP02](https://docs.aws.amazon.com/wellarchitected/latest/framework/rel_tracking_change_management_functional_testing.html)

---

#### REL08-BP03: Integrate resiliency testing as part of your deployment

**Description:** Resiliency tests (including chaos engineering) are run as part of the automated deployment pipeline in a pre-production environment.

**AWS Documentation:** [REL08-BP03](https://docs.aws.amazon.com/wellarchitected/latest/framework/rel_tracking_change_management_resilience_testing.html)

---

#### REL08-BP04: Deploy using immutable infrastructure

**Description:** Immutable infrastructure is a model that mandates that no updates, security patches, or configuration changes happen in-place on production workloads. When a change is needed, the architecture is built onto new infrastructure and deployed into production.

**AWS Documentation:** [REL08-BP04](https://docs.aws.amazon.com/wellarchitected/latest/framework/rel_tracking_change_management_immutable_infrastructure.html)

---

#### REL08-BP05: Deploy changes with automation

**Description:** Deployments and patching are automated to eliminate negative impact. Making changes to production systems is one of the largest risk areas for many organizations.

**AWS Documentation:** [REL08-BP05](https://docs.aws.amazon.com/wellarchitected/latest/framework/rel_tracking_change_management_automated_change.html)

---

## Failure management

### Design interactions to mitigate failures

#### REL05-BP01: Implement graceful degradation to transform applicable hard dependencies into soft dependencies

**Description:** When a component's dependencies are unhealthy, the component itself can still function, although in a degraded manner. For example, when a dependency call fails, instead fail open and use cached data or return a default value.

**AWS Documentation:** [REL05-BP01](https://docs.aws.amazon.com/wellarchitected/latest/framework/rel_mitigate_interaction_failure_graceful_degradation.html)

---

#### REL05-BP02: Throttle requests

**Description:** Throttle requests to mitigate resource exhaustion. Use API Gateway to throttle incoming requests or use AWS WAF for rate limiting.

**AWS Documentation:** [REL05-BP02](https://docs.aws.amazon.com/wellarchitected/latest/framework/rel_mitigate_interaction_failure_throttle_requests.html)

---

#### REL05-BP03: Control and limit retry calls

**Description:** Use exponential backoff to retry requests at progressively longer intervals between each retry. Introduce jitter between retries to randomize retry intervals. Limit the maximum number of retries.

**AWS Documentation:** [REL05-BP03](https://docs.aws.amazon.com/wellarchitected/latest/framework/rel_mitigate_interaction_failure_limit_retries.html)

---

#### REL05-BP04: Fail fast and limit queues

**Description:** If the service cannot successfully respond to a request, then fail fast. This allows resources to be freed, and keeps the service from having to maintain state about requests that cannot be served. For queues, limit the size so that resources are freed for other requests.

**AWS Documentation:** [REL05-BP04](https://docs.aws.amazon.com/wellarchitected/latest/framework/rel_mitigate_interaction_failure_fail_fast.html)

---

#### REL05-BP05: Set client timeouts

**Description:** Set timeouts appropriately, verify them systematically, and do not rely on default values as they are generally set to accommodate uncommon cases.

**AWS Documentation:** [REL05-BP05](https://docs.aws.amazon.com/wellarchitected/latest/framework/rel_mitigate_interaction_failure_client_timeouts.html)

---

#### REL05-BP06: Make services stateless where possible

**Description:** Services should either not require state, or should offload state such that between different client requests, there is no dependence on locally stored data on disk or in memory. This enables servers to be replaced at will without causing an availability impact.

**AWS Documentation:** [REL05-BP06](https://docs.aws.amazon.com/wellarchitected/latest/framework/rel_mitigate_interaction_failure_stateless.html)

---

### Monitor workload resources

#### REL06-BP01: Monitor all components for the workload (Generation)

**Description:** Monitor the components of the workload with Amazon CloudWatch or third-party tools. Monitor AWS services with AWS Health Dashboard.

**AWS Documentation:** [REL06-BP01](https://docs.aws.amazon.com/wellarchitected/latest/framework/rel_monitor_aws_resources_system_wide.html)

---

#### REL06-BP02: Define and calculate metrics (Aggregation)

**Description:** Store log data and apply filters where necessary to calculate metrics, such as counts of a specific log event, or latency calculated from log event timestamps.

**AWS Documentation:** [REL06-BP02](https://docs.aws.amazon.com/wellarchitected/latest/framework/rel_monitor_aws_resources_automate_monitoring.html)

---

#### REL06-BP03: Send notifications (Real-time processing and alarming)

**Description:** Organizations that need to know when events occur in a workload can use notifications. These notifications can be sent using multiple channels (for example, email and SMS).

**AWS Documentation:** [REL06-BP03](https://docs.aws.amazon.com/wellarchitected/latest/framework/rel_monitor_aws_resources_notification.html)

---

#### REL06-BP04: Automate responses (Real-time processing and alarming)

**Description:** Use automation to take action when an event is detected, for example, to replace failed components.

**AWS Documentation:** [REL06-BP04](https://docs.aws.amazon.com/wellarchitected/latest/framework/rel_monitor_aws_resources_automate_response_monitor.html)

---

#### REL06-BP05: Conduct reviews regularly

**Description:** Frequently review how workload monitoring is implemented and update it as needs change. Effective monitoring is driven by key business metrics. Ensure your monitoring is capturing those key metrics.

**AWS Documentation:** [REL06-BP05](https://docs.aws.amazon.com/wellarchitected/latest/framework/rel_monitor_aws_resources_conduct_reviews.html)

---

#### REL06-BP06: Monitor end-to-end tracing of requests through your system

**Description:** Distributed applications require a way to trace a request as it moves through the various services that make up the application. AWS X-Ray enables end-to-end tracing of requests.

**AWS Documentation:** [REL06-BP06](https://docs.aws.amazon.com/wellarchitected/latest/framework/rel_monitor_aws_resources_end_to_end.html)

---

#### REL06-BP07: Monitor end-to-end tracing of requests through your system

**Description:** Use AWS X-Ray or third-party tools so that developers can more easily analyze and debug distributed systems to understand how their applications and its underlying services are performing.

**AWS Documentation:** [REL06-BP07](https://docs.aws.amazon.com/wellarchitected/latest/framework/rel_monitor_aws_resources_tracing.html)

---

### Adapt to changes in demand

#### REL07-BP01: Use automation when obtaining or scaling resources

**Description:** When replacing impaired resources or scaling your workload, automate the process by using managed AWS services, such as Amazon S3 and AWS Auto Scaling. You can also use third-party tools and AWS SDKs to automate scaling.

**AWS Documentation:** [REL07-BP01](https://docs.aws.amazon.com/wellarchitected/latest/framework/rel_adapt_to_changes_in_demand_autoscale_adapt.html)

---

#### REL07-BP02: Obtain resources upon detection of impairment to a workload

**Description:** Scale resources reactively when necessary if availability is impacted, to restore workload availability.

**AWS Documentation:** [REL07-BP02](https://docs.aws.amazon.com/wellarchitected/latest/framework/rel_adapt_to_changes_in_demand_reactive.html)

---

#### REL07-BP03: Obtain resources upon detection that more resources are needed for a workload

**Description:** Scale resources proactively to meet demand and avoid availability impact.

**AWS Documentation:** [REL07-BP03](https://docs.aws.amazon.com/wellarchitected/latest/framework/rel_adapt_to_changes_in_demand_proactive.html)

---

#### REL07-BP04: Load test your workload

**Description:** Adopt a load testing methodology to measure if scaling activity meets workload requirements.

**AWS Documentation:** [REL07-BP04](https://docs.aws.amazon.com/wellarchitected/latest/framework/rel_adapt_to_changes_in_demand_load_tested.html)

---

### Back up data

#### REL09-BP01: Identify and back up all data that needs to be backed up, or reproduce the data from sources

**Description:** Understand and use the backup capabilities of the data services and resources used by your workload. Most services provide capabilities to back up data.

**AWS Documentation:** [REL09-BP01](https://docs.aws.amazon.com/wellarchitected/latest/framework/rel_backing_up_data_identified_backups.html)

---

#### REL09-BP02: Secure and encrypt backups

**Description:** Detect access using authentication and authorization, such as AWS IAM, and detect data integrity compromise by using encryption.

**AWS Documentation:** [REL09-BP02](https://docs.aws.amazon.com/wellarchitected/latest/framework/rel_backing_up_data_secured_backups.html)

---

#### REL09-BP03: Perform data backup automatically

**Description:** Configure backups to be taken automatically based on a periodic schedule informed by the Recovery Point Objective (RPO), or by changes in the dataset. Critical datasets with low data loss requirements need to be backed up automatically on a frequent basis.

**AWS Documentation:** [REL09-BP03](https://docs.aws.amazon.com/wellarchitected/latest/framework/rel_backing_up_data_automated_backups.html)

---

#### REL09-BP04: Perform periodic recovery of the data to verify backup integrity and processes

**Description:** Validate that your backup process implementation meets your recovery time objectives (RTO) and recovery point objectives (RPO) by performing a recovery test.

**AWS Documentation:** [REL09-BP04](https://docs.aws.amazon.com/wellarchitected/latest/framework/rel_backing_up_data_periodic_recovery.html)

---

### Use fault isolation

#### REL10-BP01: Deploy the workload to multiple locations

**Description:** Distribute workload data and resources across multiple Availability Zones or, where necessary, across AWS Regions. These locations can be as diverse as required.

**AWS Documentation:** [REL10-BP01](https://docs.aws.amazon.com/wellarchitected/latest/framework/rel_fault_isolation_multiaz_region_system.html)

---

#### REL10-BP02: Select the appropriate locations for your multi-location deployment

**Description:** For high availability, always (when possible) deploy your workload components to multiple Availability Zones (AZs). For workloads with extreme resilience requirements, carefully evaluate the options for a multi-Region architecture.

**AWS Documentation:** [REL10-BP02](https://docs.aws.amazon.com/wellarchitected/latest/framework/rel_fault_isolation_select_location.html)

---

#### REL10-BP03: Automate recovery for components constrained to a single location

**Description:** If components of the workload can only run in a single Availability Zone or in an on-premises data center, you must implement the capability to do a complete rebuild of the workload within your defined recovery objectives.

**AWS Documentation:** [REL10-BP03](https://docs.aws.amazon.com/wellarchitected/latest/framework/rel_fault_isolation_single_az_system.html)

---

#### REL10-BP04: Use bulkhead architectures

**Description:** Like compartments on a ship, bulkhead architectures isolate portions of your workload such that in case of a failure, impact is limited to the affected components.

**AWS Documentation:** [REL10-BP04](https://docs.aws.amazon.com/wellarchitected/latest/framework/rel_fault_isolation_use_bulkhead.html)

---

### Withstand component failures

#### REL11-BP01: Monitor all components of the workload to detect failures

**Description:** Continuously monitor the health of your workload so that you and your automated systems are aware of degradation or complete failure as soon as they occur. Monitor for key performance indicators (KPIs) based on business value.

**AWS Documentation:** [REL11-BP01](https://docs.aws.amazon.com/wellarchitected/latest/framework/rel_withstand_component_failures_monitoring_health.html)

---

#### REL11-BP02: Fail over to healthy resources

**Description:** Ensure that if a resource failure occurs, that healthy resources can continue to serve requests. For location impairments (such as Availability Zone or AWS Region), ensure you have systems in place to fail over to healthy resources in unimpaired locations.

**AWS Documentation:** [REL11-BP02](https://docs.aws.amazon.com/wellarchitected/latest/framework/rel_withstand_component_failures_failover.html)

---

#### REL11-BP03: Automate healing on all layers

**Description:** Upon detection of a failure, use automated capabilities to perform actions to remediate. This remediation should be automatic when failure is detected.

**AWS Documentation:** [REL11-BP03](https://docs.aws.amazon.com/wellarchitected/latest/framework/rel_withstand_component_failures_auto_healing_all_layers.html)

---

#### REL11-BP04: Rely on the data plane and not the control plane during recovery

**Description:** The control plane is used to configure resources, whereas the data plane is used to access resources. Design your architecture with the understanding that recovery processes must function with only the data plane, not the control plane.

**AWS Documentation:** [REL11-BP04](https://docs.aws.amazon.com/wellarchitected/latest/framework/rel_withstand_component_failures_control_vs_data_plane.html)

---

#### REL11-BP05: Use static stability to prevent bimodal behavior

**Description:** Bimodal behavior is when your workload exhibits different behavior under normal and failure modes, for example, relying on launching new instances if an Availability Zone fails. Static stability means that the workload only has a single mode of behavior.

**AWS Documentation:** [REL11-BP05](https://docs.aws.amazon.com/wellarchitected/latest/framework/rel_withstand_component_failures_static_stability.html)

---

#### REL11-BP06: Send notifications when events impact availability

**Description:** Notifications are sent upon the detection of thresholds breached, even if the issue caused by the event is automatically resolved.

**AWS Documentation:** [REL11-BP06](https://docs.aws.amazon.com/wellarchitected/latest/framework/rel_withstand_component_failures_notifications.html)

---

#### REL11-BP07: Architect your product to meet availability targets and uptime service level agreements (SLAs)

**Description:** Architect your product with a focus on the components necessary to achieve your specific availability target or SLA. This is dependent on the needs of your workload.

**AWS Documentation:** [REL11-BP07](https://docs.aws.amazon.com/wellarchitected/latest/framework/rel_withstand_component_failures_availability_objectives.html)

---

### Test reliability

#### REL12-BP01: Use playbooks to investigate failures

**Description:** Playbooks are documented investigation processes used to identify the factors that contribute to a failure scenario. Playbooks are used by responders to investigate issues reported by monitors.

**AWS Documentation:** [REL12-BP01](https://docs.aws.amazon.com/wellarchitected/latest/framework/rel_testing_resiliency_playbook_resiliency.html)

---

#### REL12-BP02: Perform post-incident analysis

**Description:** Review customer-impacting events, and identify the contributing factors and preventative action items. This information is used to develop mitigations to limit or prevent recurrence. Develop procedures for prompt and effective responses.

**AWS Documentation:** [REL12-BP02](https://docs.aws.amazon.com/wellarchitected/latest/framework/rel_testing_resiliency_rca_resiliency.html)

---

#### REL12-BP03: Test functional requirements

**Description:** Use techniques such as unit tests and integration tests that validate required functionality.

**AWS Documentation:** [REL12-BP03](https://docs.aws.amazon.com/wellarchitected/latest/framework/rel_testing_resiliency_test_functional.html)

---

#### REL12-BP04: Test scaling and performance requirements

**Description:** Use techniques such as load testing to validate that the workload meets scaling and performance requirements.

**AWS Documentation:** [REL12-BP04](https://docs.aws.amazon.com/wellarchitected/latest/framework/rel_testing_resiliency_test_performance.html)

---

#### REL12-BP05: Test resiliency using chaos engineering

**Description:** Run chaos experiments regularly in environments that are as close to production as possible. Use runbooks to execute and investigate failures.

**AWS Documentation:** [REL12-BP05](https://docs.aws.amazon.com/wellarchitected/latest/framework/rel_testing_resiliency_failure_injection_resiliency.html)

---

### Plan for disaster recovery (DR)

#### REL13-BP01: Define recovery objectives for downtime and data loss

**Description:** The workload has a recovery time objective (RTO) and recovery point objective (RPO).

**AWS Documentation:** [REL13-BP01](https://docs.aws.amazon.com/wellarchitected/latest/framework/rel_planning_for_recovery_objective_defined_recovery.html)

---

#### REL13-BP02: Use defined recovery strategies to meet the recovery objectives

**Description:** A disaster recovery (DR) strategy has been defined to meet objectives. Choose a strategy such as: backup and restore, pilot light, warm standby, or multi-site active/active.

**AWS Documentation:** [REL13-BP02](https://docs.aws.amazon.com/wellarchitected/latest/framework/rel_planning_for_recovery_disaster_recovery.html)

---

#### REL13-BP03: Test disaster recovery implementation to validate the implementation

**Description:** Regularly test failover to DR to ensure that RTO and RPO are met.

**AWS Documentation:** [REL13-BP03](https://docs.aws.amazon.com/wellarchitected/latest/framework/rel_planning_for_recovery_dr_tested.html)

---

#### REL13-BP04: Manage configuration drift at the DR site or region

**Description:** Ensure that the infrastructure, data, and configuration are as needed at the DR site or region. For example, check that AMIs and service quotas are up to date.

**AWS Documentation:** [REL13-BP04](https://docs.aws.amazon.com/wellarchitected/latest/framework/rel_planning_for_recovery_config_drift.html)

---

#### REL13-BP05: Automate recovery

**Description:** Use AWS or third-party tools to automate system recovery and route traffic to the DR site or region.

**AWS Documentation:** [REL13-BP05](https://docs.aws.amazon.com/wellarchitected/latest/framework/rel_planning_for_recovery_auto_recovery.html)

---
