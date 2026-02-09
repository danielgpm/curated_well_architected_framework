# AWS Well-Architected Framework: Security Pillar

**Total Best Practices:** 60

---

## Identity and access management

### Identity management

#### SEC01-BP01: Use strong sign-in mechanisms

**Description:** Enforce minimum password length, and train users to avoid common or reused passwords. Enforce multi-factor authentication (MFA) with software or hardware mechanisms to provide an additional layer.

**AWS Documentation:** [SEC01-BP01](https://docs.aws.amazon.com/wellarchitected/latest/framework/sec_identities_enforce_mechanisms.html)

---

#### SEC01-BP02: Use temporary credentials

**Description:** Require identities to dynamically acquire temporary credentials. For workforce identities, use AWS Single Sign-On, or federation with IAM roles to access AWS accounts.

**AWS Documentation:** [SEC01-BP02](https://docs.aws.amazon.com/wellarchitected/latest/framework/sec_identities_credentials.html)

---

#### SEC01-BP03: Store and use secrets securely

**Description:** For credentials that you cannot or have not been able to rotate to IAM roles, use a service designed to handle credentials such as AWS Secrets Manager.

**AWS Documentation:** [SEC01-BP03](https://docs.aws.amazon.com/wellarchitected/latest/framework/sec_identities_secrets.html)

---

#### SEC01-BP04: Rely on a centralized identity provider

**Description:** For workforce identities, rely on an identity provider that allows you to manage identities in a centralized place. This makes it easier to manage access across multiple applications.

**AWS Documentation:** [SEC01-BP04](https://docs.aws.amazon.com/wellarchitected/latest/framework/sec_identities_identity_provider.html)

---

#### SEC01-BP05: Audit and rotate credentials periodically

**Description:** When you cannot rely on temporary credentials and require long-term credentials, audit credentials to ensure that the defined controls are enforced.

**AWS Documentation:** [SEC01-BP05](https://docs.aws.amazon.com/wellarchitected/latest/framework/sec_identities_audit.html)

---

#### SEC01-BP06: Employ user groups and attributes

**Description:** Place users with common security requirements in groups defined by your identity provider, and put mechanisms in place to ensure that user attributes are correct and updated.

**AWS Documentation:** [SEC01-BP06](https://docs.aws.amazon.com/wellarchitected/latest/framework/sec_identities_groups_attributes.html)

---

### Permissions management

#### SEC01-BP07: Grant least privilege access

**Description:** Grant only the access that identities require by allowing access to specific actions on specific AWS resources under specific conditions.

**AWS Documentation:** [SEC01-BP07](https://docs.aws.amazon.com/wellarchitected/latest/framework/sec_permissions_least_privileges.html)

---

#### SEC01-BP08: Share resources securely

**Description:** Govern the consumption of shared resources across accounts or within your AWS Organization. Monitor shared resources and review shared resource access.

**AWS Documentation:** [SEC01-BP08](https://docs.aws.amazon.com/wellarchitected/latest/framework/sec_permissions_share_securely.html)

---

#### SEC09-BP01: Define access requirements

**Description:** Each component or resource of your workload needs to be accessed by administrators, end users, or other components. Have a clear definition of who or what should have access.

**AWS Documentation:** [SEC09-BP01](https://docs.aws.amazon.com/wellarchitected/latest/framework/sec_permissions_define.html)

---

#### SEC09-BP02: Grant least privilege access

**Description:** Grant only the access that identities require by allowing access to specific actions on specific AWS resources under specific conditions.

**AWS Documentation:** [SEC09-BP02](https://docs.aws.amazon.com/wellarchitected/latest/framework/sec_permissions_least_privileges.html)

---

#### SEC09-BP03: Establish emergency access process

**Description:** Create a process that allows emergency access to your workload in the unlikely event of an automated process or pipeline issue.

**AWS Documentation:** [SEC09-BP03](https://docs.aws.amazon.com/wellarchitected/latest/framework/sec_permissions_emergency_process.html)

---

#### SEC09-BP04: Reduce permissions continuously

**Description:** As teams and workloads determine what access they need, remove permissions they no longer use and establish a review process to achieve least privilege.

**AWS Documentation:** [SEC09-BP04](https://docs.aws.amazon.com/wellarchitected/latest/framework/sec_permissions_continuous_reduction.html)

---

#### SEC09-BP05: Define permission guardrails for your organization

**Description:** Establish common controls that restrict access to all identities in your organization. For example, you can restrict access to specific AWS Regions or prevent deletion of common resources.

**AWS Documentation:** [SEC09-BP05](https://docs.aws.amazon.com/wellarchitected/latest/framework/sec_permissions_org_guardrails.html)

---

#### SEC09-BP06: Manage access based on lifecycle

**Description:** Integrate access controls with operator and application lifecycle and your centralized federation provider to grant access in a timely manner.

**AWS Documentation:** [SEC09-BP06](https://docs.aws.amazon.com/wellarchitected/latest/framework/sec_permissions_lifecycle.html)

---

## Detection

### Configure service and application logging

#### SEC02-BP01: Configure service and application logging

**Description:** Configure logging throughout the workload, including application logs, resource logs, and AWS service logs to detect anomalies and indicators.

**AWS Documentation:** [SEC02-BP01](https://docs.aws.amazon.com/wellarchitected/latest/framework/sec_detect_investigate_events_app_service_logging.html)

---

### Analyze logs centrally

#### SEC02-BP02: Analyze logs, findings, and metrics centrally

**Description:** All logs, metrics, and telemetry should be collected centrally, and automatically analyzed to detect anomalies and indicators of unauthorized activity.

**AWS Documentation:** [SEC02-BP02](https://docs.aws.amazon.com/wellarchitected/latest/framework/sec_detect_investigate_events_central_analyze.html)

---

### Implement actionable security events

#### SEC02-BP03: Implement actionable security events

**Description:** Create alerts that are sent to and can be actioned by your team. Ensure alerts include relevant information for the team to take action.

**AWS Documentation:** [SEC02-BP03](https://docs.aws.amazon.com/wellarchitected/latest/framework/sec_detect_investigate_events_actionable.html)

---

### Automate response to events

#### SEC02-BP04: Automate response to events

**Description:** Automate the response to events to reduce organizational response time and ensure a consistent, accurate, and fast response.

**AWS Documentation:** [SEC02-BP04](https://docs.aws.amazon.com/wellarchitected/latest/framework/sec_detect_investigate_events_automate_response.html)

---

### Implement new detections

#### SEC02-BP05: Implement new detections

**Description:** Regularly review detection mechanisms to detect new threats and attack vectors. Iterate on your detection mechanisms to improve detection.

**AWS Documentation:** [SEC02-BP05](https://docs.aws.amazon.com/wellarchitected/latest/framework/sec_detect_investigate_events_implement_detections.html)

---

### Review and adapt

#### SEC02-BP06: Conduct reviews regularly

**Description:** Frequently review the details and configure alerts according to the findings of your reviews to continually refine your threat detection.

**AWS Documentation:** [SEC02-BP06](https://docs.aws.amazon.com/wellarchitected/latest/framework/sec_detect_investigate_events_review.html)

---

### Threat detection

#### SEC10-BP01: Configure service and application logging

**Description:** Configure logging throughout the workload, including application logs, resource logs, and AWS service logs to detect anomalies and indicators.

**AWS Documentation:** [SEC10-BP01](https://docs.aws.amazon.com/wellarchitected/latest/framework/sec_detect_investigate_events_app_service_logging.html)

---

#### SEC10-BP02: Analyze logs, findings, and metrics centrally

**Description:** All logs, metrics, and telemetry should be collected centrally and automatically analyzed to detect anomalies and indicators of unauthorized activity.

**AWS Documentation:** [SEC10-BP02](https://docs.aws.amazon.com/wellarchitected/latest/framework/sec_detect_investigate_events_central_analyze.html)

---

#### SEC10-BP03: Implement actionable security events

**Description:** Create alerts that are sent to and can be actioned by your team. Ensure that alerts include relevant information for the team to take action.

**AWS Documentation:** [SEC10-BP03](https://docs.aws.amazon.com/wellarchitected/latest/framework/sec_detect_investigate_events_actionable.html)

---

#### SEC10-BP04: Implement detections

**Description:** Use detective controls to identify potential security threats or incidents. They are an essential part of detective controls for governance and compliance.

**AWS Documentation:** [SEC10-BP04](https://docs.aws.amazon.com/wellarchitected/latest/framework/sec_detect_investigate_events_implement_detections.html)

---

#### SEC10-BP05: Automate response to events

**Description:** Automate the response to events detected to reduce organizational response time and ensure a consistent, accurate response.

**AWS Documentation:** [SEC10-BP05](https://docs.aws.amazon.com/wellarchitected/latest/framework/sec_detect_investigate_events_automate_response.html)

---

## Infrastructure protection

### Protecting networks

#### SEC03-BP01: Create network layers

**Description:** Group components that share reachability requirements into layers. For example, a database cluster in a VPC with no need for internet access should be placed in subnets with no route to or from the internet.

**AWS Documentation:** [SEC03-BP01](https://docs.aws.amazon.com/wellarchitected/latest/framework/sec_network_protection_create_layers.html)

---

#### SEC03-BP02: Control traffic at all layers

**Description:** Apply controls for controlling both ingress and egress traffic, including data loss prevention. For Amazon VPC, this includes security groups, Network ACLs, and subnets.

**AWS Documentation:** [SEC03-BP02](https://docs.aws.amazon.com/wellarchitected/latest/framework/sec_network_protection_control_traffic.html)

---

#### SEC03-BP03: Automate network protection

**Description:** Automate protection mechanisms to provide a self-defending network based on threat intelligence and anomaly detection.

**AWS Documentation:** [SEC03-BP03](https://docs.aws.amazon.com/wellarchitected/latest/framework/sec_network_protection_auto_protect.html)

---

#### SEC03-BP04: Implement inspection and protection

**Description:** Inspect and filter your traffic at each layer. For example, use a web application firewall to help protect against common attacks targeting the application layer.

**AWS Documentation:** [SEC03-BP04](https://docs.aws.amazon.com/wellarchitected/latest/framework/sec_network_protection_inspection.html)

---

### Protecting compute

#### SEC03-BP05: Control compute resource access

**Description:** Configure compute resources to limit access through operating system and application configurations, such as hardening, minimizing components, and managing permissions.

**AWS Documentation:** [SEC03-BP05](https://docs.aws.amazon.com/wellarchitected/latest/framework/sec_infrastructure_compute_access.html)

---

#### SEC03-BP06: Automate compute protection

**Description:** Automate your protective compute mechanisms including vulnerability management, reduction in attack surface, and management of resources.

**AWS Documentation:** [SEC03-BP06](https://docs.aws.amazon.com/wellarchitected/latest/framework/sec_infrastructure_compute_auto.html)

---

#### SEC03-BP07: Implement managed services

**Description:** Implement services that manage resources, such as Amazon RDS, AWS Lambda, and Amazon ECS, to reduce security maintenance tasks as part of the shared responsibility model.

**AWS Documentation:** [SEC03-BP07](https://docs.aws.amazon.com/wellarchitected/latest/framework/sec_infrastructure_compute_managed.html)

---

### Resource protection

#### SEC11-BP01: Protect configuration

**Description:** Ensure you have a secure baseline for your cloud workload configuration. You can use AWS service-native solutions or partner services to enforce compliance.

**AWS Documentation:** [SEC11-BP01](https://docs.aws.amazon.com/wellarchitected/latest/framework/sec_infrastructure_protect_configuration.html)

---

#### SEC11-BP02: Use resource tagging

**Description:** Tag your resources to help you identify ownership and classify resources, which enables you to manage your workload effectively.

**AWS Documentation:** [SEC11-BP02](https://docs.aws.amazon.com/wellarchitected/latest/framework/sec_infrastructure_protect_tagging.html)

---

#### SEC11-BP03: Validate software integrity

**Description:** Implement mechanisms to validate software integrity to verify that the software in use is from a trusted source and has not been tampered with.

**AWS Documentation:** [SEC11-BP03](https://docs.aws.amazon.com/wellarchitected/latest/framework/sec_infrastructure_protect_validate_software.html)

---

## Data protection

### Data classification

#### SEC04-BP01: Identify the data within your workload

**Description:** You need to understand the type and classification of data your workload is processing, the associated business processes, where it's stored, and the resulting controls that are needed.

**AWS Documentation:** [SEC04-BP01](https://docs.aws.amazon.com/wellarchitected/latest/framework/sec_data_classification_identify.html)

---

#### SEC04-BP02: Define data protection controls

**Description:** Protect data according to its classification level. For example, secure data classified as public by denying non-approved write access, and secure sensitive data using additional controls.

**AWS Documentation:** [SEC04-BP02](https://docs.aws.amazon.com/wellarchitected/latest/framework/sec_data_classification_define_protection.html)

---

#### SEC04-BP03: Automate identification and classification

**Description:** Automating the identification and classification of data can help you implement the correct controls. Using automation for this instead of direct access reduces human error.

**AWS Documentation:** [SEC04-BP03](https://docs.aws.amazon.com/wellarchitected/latest/framework/sec_data_classification_auto_classify.html)

---

#### SEC04-BP04: Define data lifecycle management

**Description:** Your defined lifecycle strategy should be based on sensitivity level as well as legal and organization requirements for retention and destruction.

**AWS Documentation:** [SEC04-BP04](https://docs.aws.amazon.com/wellarchitected/latest/framework/sec_data_classification_lifecycle.html)

---

### Protecting data at rest

#### SEC05-BP01: Implement secure key management

**Description:** By defining an encryption approach that includes the storage, rotation, and access control of keys, you can help provide protection for your content against unauthorized access.

**AWS Documentation:** [SEC05-BP01](https://docs.aws.amazon.com/wellarchitected/latest/framework/sec_protect_data_rest_key_mgmt.html)

---

#### SEC05-BP02: Enforce encryption at rest

**Description:** You should enforce your encryption requirements based on the latest standards and recommendations to help protect your data at rest.

**AWS Documentation:** [SEC05-BP02](https://docs.aws.amazon.com/wellarchitected/latest/framework/sec_protect_data_rest_encrypt.html)

---

#### SEC05-BP03: Automate data at rest protection

**Description:** Use automated tools to validate and enforce data at rest controls continuously, for example, verify that there are only encrypted storage resources.

**AWS Documentation:** [SEC05-BP03](https://docs.aws.amazon.com/wellarchitected/latest/framework/sec_protect_data_rest_auto_protect.html)

---

#### SEC05-BP04: Enforce access control

**Description:** To help protect your data at rest, enforce access control using mechanisms such as isolation and versioning, and apply the principle of least privilege.

**AWS Documentation:** [SEC05-BP04](https://docs.aws.amazon.com/wellarchitected/latest/framework/sec_protect_data_rest_access_control.html)

---

#### SEC05-BP05: Use mechanisms to keep people away from data

**Description:** Keep all users away from directly accessing sensitive data and systems under normal operational circumstances. For example, use change management workflows to manage instances.

**AWS Documentation:** [SEC05-BP05](https://docs.aws.amazon.com/wellarchitected/latest/framework/sec_protect_data_rest_people_away.html)

---

### Protecting data in transit

#### SEC06-BP01: Implement secure key and certificate management

**Description:** Store encryption keys and certificates securely and rotate them at appropriate time intervals with strict access control.

**AWS Documentation:** [SEC06-BP01](https://docs.aws.amazon.com/wellarchitected/latest/framework/sec_protect_data_transit_key_cert_mgmt.html)

---

#### SEC06-BP02: Enforce encryption in transit

**Description:** Enforce your encryption requirements based on appropriate standards and recommendations to help you meet organizational, legal, and compliance requirements.

**AWS Documentation:** [SEC06-BP02](https://docs.aws.amazon.com/wellarchitected/latest/framework/sec_protect_data_transit_encrypt.html)

---

#### SEC06-BP03: Automate detection of unintended data access

**Description:** Use tools such as GuardDuty to automatically detect attempts to move data outside of defined boundaries based on DNS and network activity.

**AWS Documentation:** [SEC06-BP03](https://docs.aws.amazon.com/wellarchitected/latest/framework/sec_protect_data_transit_auto_detect.html)

---

#### SEC06-BP04: Authenticate network communications

**Description:** Verify the identity of communications by using protocols that support authentication, such as Transport Layer Security (TLS) or IPsec.

**AWS Documentation:** [SEC06-BP04](https://docs.aws.amazon.com/wellarchitected/latest/framework/sec_protect_data_transit_authenticate.html)

---

## Incident response

### Design goals of cloud response

#### SEC07-BP01: Identify key personnel and external resources

**Description:** Identify internal and external personnel, resources, and legal obligations that would help your organization respond to an incident.

**AWS Documentation:** [SEC07-BP01](https://docs.aws.amazon.com/wellarchitected/latest/framework/sec_incident_response_identify_personnel.html)

---

#### SEC07-BP02: Develop incident management plans

**Description:** Create plans to help you respond to, communicate during, and recover from an incident. For example, you can start an incident response plan with the most likely scenarios.

**AWS Documentation:** [SEC07-BP02](https://docs.aws.amazon.com/wellarchitected/latest/framework/sec_incident_response_develop_mgmt_plans.html)

---

#### SEC07-BP03: Prepare forensic capabilities

**Description:** Identify and prepare forensic investigation capabilities that are suitable, including external specialists, tools, and automation.

**AWS Documentation:** [SEC07-BP03](https://docs.aws.amazon.com/wellarchitected/latest/framework/sec_incident_response_prepare_forensic.html)

---

#### SEC07-BP04: Automate containment capability

**Description:** Automate containment and recovery of an incident to reduce response times and organizational impact.

**AWS Documentation:** [SEC07-BP04](https://docs.aws.amazon.com/wellarchitected/latest/framework/sec_incident_response_auto_contain.html)

---

#### SEC07-BP05: Pre-provision access

**Description:** Ensure that incident responders have the correct access pre-provisioned into AWS to reduce the time for investigation through to recovery.

**AWS Documentation:** [SEC07-BP05](https://docs.aws.amazon.com/wellarchitected/latest/framework/sec_incident_response_pre_provision_access.html)

---

#### SEC07-BP06: Pre-deploy tools

**Description:** Ensure that security personnel have the right tools pre-deployed into AWS to reduce the time for investigation through to recovery.

**AWS Documentation:** [SEC07-BP06](https://docs.aws.amazon.com/wellarchitected/latest/framework/sec_incident_response_pre_deploy_tools.html)

---

#### SEC07-BP07: Run game days

**Description:** Practice incident response game days (simulations) regularly, incorporate lessons learned into your incident management plans, and continuously improve.

**AWS Documentation:** [SEC07-BP07](https://docs.aws.amazon.com/wellarchitected/latest/framework/sec_incident_response_run_game_days.html)

---

## Application security

### Application security

#### SEC08-BP01: Train for application security

**Description:** Provide training to the builders in your organization on common practices for the secure development and operation of applications.

**AWS Documentation:** [SEC08-BP01](https://docs.aws.amazon.com/wellarchitected/latest/framework/sec_app_security_train.html)

---

#### SEC08-BP02: Automate testing throughout the development and release lifecycle

**Description:** Automate the testing of security properties throughout development and release. Automation makes it easier to identify issues early and perform consistent testing.

**AWS Documentation:** [SEC08-BP02](https://docs.aws.amazon.com/wellarchitected/latest/framework/sec_app_security_auto_testing.html)

---

#### SEC08-BP03: Perform regular penetration testing

**Description:** Perform regular penetration testing of your applications. This helps identify potential software issues that cannot be detected by automated testing or manual code review.

**AWS Documentation:** [SEC08-BP03](https://docs.aws.amazon.com/wellarchitected/latest/framework/sec_app_security_pen_testing.html)

---

#### SEC08-BP04: Manual code reviews

**Description:** Conduct manual code reviews of your application code, and include this as part of the code review process. Manual code review complements automated tooling.

**AWS Documentation:** [SEC08-BP04](https://docs.aws.amazon.com/wellarchitected/latest/framework/sec_app_security_manual_review.html)

---

#### SEC08-BP05: Centralize services for packages and dependencies

**Description:** Use a centralized service to manage packages and dependencies to improve software supply chain security and maintain a software bill of materials (SBOM).

**AWS Documentation:** [SEC08-BP05](https://docs.aws.amazon.com/wellarchitected/latest/framework/sec_app_security_package_dependencies.html)

---
