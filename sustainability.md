# AWS Well-Architected Framework: Sustainability Pillar

**Total Best Practices:** 8

---

## Best practices

### Region selection

#### SUS01-BP01: Choose Regions based on both business requirements and sustainability goals

**Description:** Consider sustainability goals when you select Regions for your workloads in addition to business factors such as cost, latency, and regulatory compliance.

**AWS Documentation:** [SUS01-BP01](https://docs.aws.amazon.com/wellarchitected/latest/framework/sus_sus_region_a2.html)

---

### Alignment to demand

#### SUS02-BP01: Scale infrastructure to meet demand

**Description:** Scale infrastructure dynamically to match demand for compute and storage capacity, avoiding overprovisioning.

**AWS Documentation:** [SUS02-BP01](https://docs.aws.amazon.com/wellarchitected/latest/framework/sus_sus_user_a2.html)

---

#### SUS02-BP02: Align service levels to customers needs

**Description:** Confirm that you have a clear understanding of your customers' needs for latency, burst capacity, and other factors to properly design your service levels.

**AWS Documentation:** [SUS02-BP02](https://docs.aws.amazon.com/wellarchitected/latest/framework/sus_sus_user_a3.html)

---

#### SUS02-BP03: Optimize your code for maximum data set usage

**Description:** Optimize application code to minimize data processing requirements and improve efficiency.

**AWS Documentation:** [SUS02-BP03](https://docs.aws.amazon.com/wellarchitected/latest/framework/sus_sus_user_a4.html)

---

### Software and architecture

#### SUS03-BP01: Optimize software and architecture for asynchronous and scheduled jobs

**Description:** Use efficient software patterns and architectures to minimize the footprint of scheduled and asynchronous jobs.

**AWS Documentation:** [SUS03-BP01](https://docs.aws.amazon.com/wellarchitected/latest/framework/sus_sus_software_a2.html)

---

#### SUS03-BP02: Remove or refactor workload components with low or no use

**Description:** Remove components that are unused and refactor components with little utilization to minimize waste.

**AWS Documentation:** [SUS03-BP02](https://docs.aws.amazon.com/wellarchitected/latest/framework/sus_sus_software_a3.html)

---

#### SUS03-BP03: Optimize geographic placement of workloads based on their networking requirements

**Description:** Analyze network access patterns and identify how to minimize the total network distance traveled by data to reduce the environmental impact.

**AWS Documentation:** [SUS03-BP03](https://docs.aws.amazon.com/wellarchitected/latest/framework/sus_sus_software_a4.html)

---

#### SUS03-BP04: Optimize team member resources for activities performed

**Description:** Optimize resources provided to team members to minimize the environmental sustainability impact while supporting their needs.

**AWS Documentation:** [SUS03-BP04](https://docs.aws.amazon.com/wellarchitected/latest/framework/sus_sus_software_a5.html)

---
