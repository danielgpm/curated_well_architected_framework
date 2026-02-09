# AWS Well-Architected Framework: Operational Excellence Pillar

**Total Best Practices:** 67

---

## Organization

### Business priorities

#### OPS01-BP01: Evaluate external customer needs

**Description:** Involve key stakeholders, including business, development, and operations teams, to determine where to focus efforts on external customer needs. Ensure that you have a thorough understanding of the support required to achieve business outcomes.

**AWS Documentation:** [OPS01-BP01](https://docs.aws.amazon.com/wellarchitected/latest/operational-excellence-pillar/ops_priorities_ext_cust_needs.html)

---

#### OPS01-BP02: Evaluate internal customer needs

**Description:** Involve key stakeholders, including business, development, and operations teams, when determining where to focus efforts on internal customer needs. Ensure that you have a thorough understanding of the operations support required to achieve business outcomes.

**AWS Documentation:** [OPS01-BP02](https://docs.aws.amazon.com/wellarchitected/latest/framework/ops_priorities_int_cust_needs.html)

---

#### OPS01-BP03: Evaluate governance requirements

**Description:** Ensure that you are aware of guidelines or obligations defined by your organizational governance and external factors, such as regulatory compliance requirements and industry standards, that may mandate or emphasize specific focus.

**AWS Documentation:** [OPS01-BP03](https://docs.aws.amazon.com/wellarchitected/latest/framework/ops_priorities_eval_gov.html)

---

#### OPS01-BP04: Evaluate compliance requirements

**Description:** Regulatory, industry, and internal compliance requirements are an important driver for defining your organization's priorities. Your compliance framework may preclude you from using specific technologies or geographic locations.

**AWS Documentation:** [OPS01-BP04](https://docs.aws.amazon.com/wellarchitected/latest/framework/ops_priorities_eval_compliance.html)

---

#### OPS01-BP05: Evaluate threat landscape

**Description:** Evaluate threats to the business (for example, competition, business risk and liabilities, operational risks, and information security threats) and maintain current information in a risk registry. Include the impact of risks when determining where to focus efforts.

**AWS Documentation:** [OPS01-BP05](https://docs.aws.amazon.com/wellarchitected/latest/framework/ops_priorities_eval_threat_landscape.html)

---

#### OPS01-BP06: Evaluate tradeoffs while managing benefits and risks

**Description:** Evaluate the impact of tradeoffs between competing interests or alternative approaches to help make informed decisions when determining where to focus efforts or choosing a course of action. For example, accelerating speed to market for new features may be emphasized over cost optimization.

**AWS Documentation:** [OPS01-BP06](https://docs.aws.amazon.com/wellarchitected/latest/framework/ops_priorities_eval_tradeoffs.html)

---

### Operating model

#### OPS02-BP01: Team members know what data they are responsible for

**Description:** Understanding data classification schema and organizational policies for data helps team members understand the type of data they are responsible for, and the related compliance requirements or business value.

**AWS Documentation:** [OPS02-BP01](https://docs.aws.amazon.com/wellarchitected/latest/framework/ops_operating_model_def_owernship.html)

---

#### OPS02-BP02: Mechanisms exist to identify responsibility and ownership

**Description:** Have a method of uniquely identifying teams and members within the organization (for example, through tagging, metadata, or resource naming conventions) for tracking ownership and responsibility.

**AWS Documentation:** [OPS02-BP02](https://docs.aws.amazon.com/wellarchitected/latest/framework/ops_operating_model_def_resp_own.html)

---

#### OPS02-BP03: Mechanisms exist to request additions, changes, and exceptions

**Description:** You are able to make requests to team members. Members can make requests of other teams (for example, escalations, expert consultations, and development work) and track the status of those requests.

**AWS Documentation:** [OPS02-BP03](https://docs.aws.amazon.com/wellarchitected/latest/framework/ops_operating_model_def_escalation.html)

---

#### OPS02-BP04: Responsibilities between teams are predefined or negotiated

**Description:** There are defined or negotiated agreements between teams describing how they work with and support each other (for example, response times, service level objectives, or service level agreements). Inter-team communications channels are documented.

**AWS Documentation:** [OPS02-BP04](https://docs.aws.amazon.com/wellarchitected/latest/framework/ops_operating_model_team_culture.html)

---

### Organizational culture

#### OPS03-BP01: Provide executive sponsorship

**Description:** Senior leadership clearly sets expectations for the organization and evaluates success. Senior leadership is the sponsor, advocate, and driver for the adoption of best practices and evolution of the organization.

**AWS Documentation:** [OPS03-BP01](https://docs.aws.amazon.com/wellarchitected/latest/framework/ops_org_culture_exec_sponsor.html)

---

#### OPS03-BP02: Team members are empowered to take action when outcomes are at risk

**Description:** The workload owner has defined guidance and scope empowering team members to respond when outcomes are at risk. Escalation mechanisms are used to get direction when events are outside of the defined scope.

**AWS Documentation:** [OPS03-BP02](https://docs.aws.amazon.com/wellarchitected/latest/framework/ops_org_culture_team_member_empower.html)

---

#### OPS03-BP03: Escalation is encouraged

**Description:** Team members have mechanisms and are encouraged to escalate concerns to decision makers and stakeholders if they believe outcomes are at risk. Escalation should be performed early and often so that risks can be identified, and prevented from causing incidents.

**AWS Documentation:** [OPS03-BP03](https://docs.aws.amazon.com/wellarchitected/latest/framework/ops_org_culture_escalation_encouraged.html)

---

#### OPS03-BP04: Communications are timely, clear, and actionable

**Description:** Mechanisms exist to provide timely notifications to your team of known risks and planned events. Necessary context, details, and time (when possible) are provided to support determining if action is necessary, what action is required, and to take action in a timely manner.

**AWS Documentation:** [OPS03-BP04](https://docs.aws.amazon.com/wellarchitected/latest/framework/ops_org_culture_comms_timely_clear_actnable.html)

---

#### OPS03-BP05: Experimentation is encouraged

**Description:** Experimentation accelerates learning and keeps team members interested and engaged. An undesired result is a successful experiment that has identified a path that will not lead to success.

**AWS Documentation:** [OPS03-BP05](https://docs.aws.amazon.com/wellarchitected/latest/framework/ops_org_culture_exp_success_and_failure.html)

---

#### OPS03-BP06: Team members are enabled and encouraged to maintain and grow their skill sets

**Description:** Teams must grow their skill sets to adopt new technologies, and to support changes in demand and responsibilities in support of your workloads. Growth of skills in new technologies is frequently a source of team member satisfaction and supports innovation.

**AWS Documentation:** [OPS03-BP06](https://docs.aws.amazon.com/wellarchitected/latest/framework/ops_org_culture_team_enc_learn.html)

---

#### OPS03-BP07: Resource teams appropriately

**Description:** Maintain team member resources appropriately to ensure availability for business outcomes. Overtasking team members increases the risk of incidents resulting from human error.

**AWS Documentation:** [OPS03-BP07](https://docs.aws.amazon.com/wellarchitected/latest/framework/ops_org_culture_appropriate_res.html)

---

#### OPS03-BP08: Diverse opinions are encouraged and sought within and across teams

**Description:** Leverage cross-organizational diversity to seek multiple unique perspectives. Use this perspective to increase innovation, challenge your assumptions, and reduce the risk of confirmation bias.

**AWS Documentation:** [OPS03-BP08](https://docs.aws.amazon.com/wellarchitected/latest/operational-excellence-pillar/ops03_bp08.html)

---

## Prepare

### Design telemetry

#### OPS04-BP01: Identify key performance indicators

**Description:** Identify key performance indicators (KPIs) based on desired business outcomes (for example, order rate, customer retention rate, and profit versus operating expense) and customer outcomes (for example, customer satisfaction).

**AWS Documentation:** [OPS04-BP01](https://docs.aws.amazon.com/wellarchitected/latest/framework/ops_observability_identify_kpi.html)

---

#### OPS04-BP02: Implement application telemetry

**Description:** Instrument your application code to emit information about its internal state, status, and achievement of business outcomes. For example, queue depth, error messages, and response times.

**AWS Documentation:** [OPS04-BP02](https://docs.aws.amazon.com/wellarchitected/latest/framework/ops_observability_app_telemetry.html)

---

#### OPS04-BP03: Implement user experience telemetry

**Description:** Implement user experience telemetry (for example, clickstream, heatmap, and user session replay) to have useful data about how your customers use your product or service. You can then identify changes to customer behavior by analyzing this telemetry.

**AWS Documentation:** [OPS04-BP03](https://docs.aws.amazon.com/wellarchitected/latest/framework/ops_observability_user_exp_telemetry.html)

---

#### OPS04-BP04: Implement dependency telemetry

**Description:** Implement telemetry from services and third-party applications that your workload depends on. Examples include Amazon DynamoDB metrics, AWS Lambda function metrics, Amazon API Gateway metrics, and auto scaling events.

**AWS Documentation:** [OPS04-BP04](https://docs.aws.amazon.com/wellarchitected/latest/framework/ops_observability_dependency_telemetry.html)

---

#### OPS04-BP05: Implement distributed tracing

**Description:** Implement distributed tracing to track requests through the workload. Use AWS X-Ray to gain end-to-end visibility of traffic as it flows through your application and its underlying components.

**AWS Documentation:** [OPS04-BP05](https://docs.aws.amazon.com/wellarchitected/latest/framework/ops_observability_dist_trace.html)

---

### Design for operations

#### OPS05-BP01: Use version control

**Description:** Use version control to track changes and releases in your workload code, configuration, Infrastructure as Code (IaC), and other operational documents.

**AWS Documentation:** [OPS05-BP01](https://docs.aws.amazon.com/wellarchitected/latest/framework/ops_dev_integ_version_control.html)

---

#### OPS05-BP02: Test and validate changes

**Description:** Test and validate changes to help limit and detect errors. Automate testing where possible to reduce the time and effort needed.

**AWS Documentation:** [OPS05-BP02](https://docs.aws.amazon.com/wellarchitected/latest/framework/ops_dev_integ_test_val_chg.html)

---

#### OPS05-BP03: Use configuration management systems

**Description:** Use configuration management systems to make and track configuration changes to your workload. These systems reduce errors caused by manual processes and reduce the level of effort needed to deploy changes.

**AWS Documentation:** [OPS05-BP03](https://docs.aws.amazon.com/wellarchitected/latest/framework/ops_dev_integ_config_mgmt.html)

---

#### OPS05-BP04: Use build and deployment management systems

**Description:** Use build and deployment management systems to track and implement change. This reduces errors caused by manual processes and reduces the effort to deploy changes.

**AWS Documentation:** [OPS05-BP04](https://docs.aws.amazon.com/wellarchitected/latest/framework/ops_dev_integ_build_mgmt.html)

---

#### OPS05-BP05: Perform patch management

**Description:** Perform patch management to gain features, address issues, and remain compliant with governance. Automate patch management to reduce errors caused by manual processes, and reduce the level of effort needed to patch.

**AWS Documentation:** [OPS05-BP05](https://docs.aws.amazon.com/wellarchitected/latest/framework/ops_dev_integ_patch_mgmt.html)

---

#### OPS05-BP06: Share design standards

**Description:** Share best practices across teams to increase awareness and maximize the benefits of development efforts. Adopt industry standards that support your development activities.

**AWS Documentation:** [OPS05-BP06](https://docs.aws.amazon.com/wellarchitected/latest/framework/ops_dev_integ_share_design_stds.html)

---

#### OPS05-BP07: Implement practices to improve code quality

**Description:** Implement practices to improve code quality and minimize defects. For example, test-driven development (TDD), code reviews, and standards adoption.

**AWS Documentation:** [OPS05-BP07](https://docs.aws.amazon.com/wellarchitected/latest/framework/ops_dev_integ_code_quality.html)

---

#### OPS05-BP08: Use multiple environments

**Description:** Use multiple environments to experiment, develop, and test your workload. Use increasing levels of controls as environments approach production to gain confidence your workload will operate as intended when deployed.

**AWS Documentation:** [OPS05-BP08](https://docs.aws.amazon.com/wellarchitected/latest/framework/ops_dev_integ_multiple_env.html)

---

#### OPS05-BP09: Make frequent, small, reversible changes

**Description:** Frequent, small, and reversible changes reduce the scope and impact of a change. This eases troubleshooting, enables faster remediation, and provides the option to roll back a change.

**AWS Documentation:** [OPS05-BP09](https://docs.aws.amazon.com/wellarchitected/latest/framework/ops_dev_integ_frequent_small_revers_chg.html)

---

#### OPS05-BP10: Fully automate integration and deployment

**Description:** Automate build, deployment, and testing of the workload. This reduces errors caused by manual processes and reduces the effort to deploy changes.

**AWS Documentation:** [OPS05-BP10](https://docs.aws.amazon.com/wellarchitected/latest/framework/ops_dev_integ_auto_integration_deployment.html)

---

### Mitigate deployment risks

#### OPS06-BP01: Plan for unsuccessful changes

**Description:** Plan to revert to a known good state, or remediate in the production environment if a change does not have the desired outcome. This preparation reduces recovery time through faster responses.

**AWS Documentation:** [OPS06-BP01](https://docs.aws.amazon.com/wellarchitected/latest/framework/ops_mitigate_deployment_risks_plan_for_unsuccessful_changes.html)

---

#### OPS06-BP02: Test deployments

**Description:** Test deployments to identify issues early and ensure changes can be successfully deployed. Use automated testing where possible to reduce errors caused by manual processes.

**AWS Documentation:** [OPS06-BP02](https://docs.aws.amazon.com/wellarchitected/latest/framework/ops_mitigate_deployment_risks_test_validate_chg.html)

---

#### OPS06-BP03: Employ safe deployment strategies

**Description:** Adopt deployment strategies that limit impact on customers during deployments (for example, canary deployments, feature toggles, or blue/green deployments).

**AWS Documentation:** [OPS06-BP03](https://docs.aws.amazon.com/wellarchitected/latest/framework/ops_mitigate_deployment_risks_safe_deployment_strat.html)

---

#### OPS06-BP04: Automate testing and rollback

**Description:** Automate testing of deployed environments to confirm desired outcomes. Automate rollback to previous known good state if outcomes are not achieved to minimize recovery time and reduce errors caused by manual processes.

**AWS Documentation:** [OPS06-BP04](https://docs.aws.amazon.com/wellarchitected/latest/framework/ops_mitigate_deployment_risks_auto_test_and_rollback.html)

---

### Operational readiness

#### OPS07-BP01: Ensure personnel capability

**Description:** Have a mechanism to validate that you have the appropriate number of trained personnel to provide support for operational needs. Train personnel and adjust personnel capacity as necessary to maintain effective support.

**AWS Documentation:** [OPS07-BP01](https://docs.aws.amazon.com/wellarchitected/latest/framework/ops_ready_to_support_ensure_knowledge.html)

---

#### OPS07-BP02: Ensure a consistent review of operational readiness

**Description:** Use Operational Readiness Reviews (ORRs) to validate that you can operate your workload. An ORR is a mechanism developed at Amazon to validate that teams can safely operate their workloads.

**AWS Documentation:** [OPS07-BP02](https://docs.aws.amazon.com/wellarchitected/latest/framework/ops_ready_to_support_consistent_ops_ready_review.html)

---

#### OPS07-BP03: Use runbooks to perform procedures

**Description:** Runbooks are documented procedures to achieve specific outcomes. Enable consistent and prompt responses to well-understood events by documenting procedures in runbooks.

**AWS Documentation:** [OPS07-BP03](https://docs.aws.amazon.com/wellarchitected/latest/framework/ops_ready_to_support_use_runbooks.html)

---

#### OPS07-BP04: Use playbooks to investigate issues

**Description:** Enable consistent and prompt responses to failure scenarios that are not well understood by documenting investigation processes in playbooks. Playbooks are the predefined steps to perform to identify the factors contributing to a failure scenario.

**AWS Documentation:** [OPS07-BP04](https://docs.aws.amazon.com/wellarchitected/latest/framework/ops_ready_to_support_use_playbooks.html)

---

#### OPS07-BP05: Make informed decisions to deploy systems and changes

**Description:** Evaluate the operational readiness of your workload, processes, procedures, and personnel to understand the operational risks related to your workload. Make an informed decision on when to deploy your systems or make changes to your workload.

**AWS Documentation:** [OPS07-BP05](https://docs.aws.amazon.com/wellarchitected/latest/framework/ops_ready_to_support_practice_response.html)

---

## Operate

### Observability

#### OPS08-BP01: Analyze workload metrics

**Description:** Collect metrics from your workload to analyze its behavior and identify potential issues. Use CloudWatch or third-party services to collect and analyze metrics.

**AWS Documentation:** [OPS08-BP01](https://docs.aws.amazon.com/wellarchitected/latest/framework/ops_workload_observability_analyze_workload_metrics.html)

---

#### OPS08-BP02: Analyze workload logs

**Description:** Collect logs from your workload to analyze behavior and identify potential issues. Aggregate logs to a central location for analysis.

**AWS Documentation:** [OPS08-BP02](https://docs.aws.amazon.com/wellarchitected/latest/framework/ops_workload_observability_analyze_workload_logs.html)

---

#### OPS08-BP03: Analyze workload traces

**Description:** Use traces to identify bottlenecks, latency issues, and failures in request processing. Implement AWS X-Ray or third-party distributed tracing services.

**AWS Documentation:** [OPS08-BP03](https://docs.aws.amazon.com/wellarchitected/latest/framework/ops_workload_observability_analyze_workload_traces.html)

---

#### OPS08-BP04: Create actionable alerts

**Description:** Create alerts that activate when thresholds are breached or significant events occur. Design alerts to provide the information necessary to understand the issue and take appropriate action.

**AWS Documentation:** [OPS08-BP04](https://docs.aws.amazon.com/wellarchitected/latest/framework/ops_workload_observability_actionable_alerts.html)

---

#### OPS08-BP05: Create dashboards

**Description:** Create dashboards that show the health and operational status of your workload. Tailor dashboards to the audience to provide relevant information for their needs.

**AWS Documentation:** [OPS08-BP05](https://docs.aws.amazon.com/wellarchitected/latest/framework/ops_workload_observability_create_dashboards.html)

---

### Event management

#### OPS09-BP01: Establish a process for event, incident, and problem management

**Description:** Establish a process for event, incident, and problem management. Define the lifecycle from identification to remediation and lessons learned.

**AWS Documentation:** [OPS09-BP01](https://docs.aws.amazon.com/wellarchitected/latest/framework/ops_operations_health_ops_kpis_metrics.html)

---

#### OPS09-BP02: Have a process per alert

**Description:** Have a well-defined response path (runbook or playbook) for each alert. Document what the alert means, what actions to take, and who should be notified.

**AWS Documentation:** [OPS09-BP02](https://docs.aws.amazon.com/wellarchitected/latest/framework/ops_operations_health_ops_metrics.html)

---

#### OPS09-BP03: Prioritize operational events based on business impact

**Description:** Evaluate the impact of events on business value and customer experience to prioritize response. Respond to events in order of their impact to business outcomes.

**AWS Documentation:** [OPS09-BP03](https://docs.aws.amazon.com/wellarchitected/latest/framework/ops_operations_health_operations_metrics_review.html)

---

#### OPS09-BP04: Define escalation paths

**Description:** Define escalation paths for when the responsible team cannot resolve the event. Include contacts in the escalation path and the criteria for escalation.

**AWS Documentation:** [OPS09-BP04](https://docs.aws.amazon.com/wellarchitected/latest/framework/ops_operations_health_operations_metrics_baselining.html)

---

#### OPS09-BP05: Define a customer communication plan for outages

**Description:** Communicate with customers during events that impact them. Provide status updates and estimated time to resolution.

**AWS Documentation:** [OPS09-BP05](https://docs.aws.amazon.com/wellarchitected/latest/framework/ops_operations_health_expectations_ops_activity.html)

---

#### OPS09-BP06: Communicate status through dashboards

**Description:** Provide dashboards tailored to target audiences to communicate the current operating status of the business and provide metrics of interest.

**AWS Documentation:** [OPS09-BP06](https://docs.aws.amazon.com/wellarchitected/latest/framework/ops_operations_health_ops_outcome_alerts.html)

---

#### OPS09-BP07: Automate responses to events

**Description:** Automate responses to events to reduce human error and time to resolution. Use event-driven architectures to activate automated responses.

**AWS Documentation:** [OPS09-BP07](https://docs.aws.amazon.com/wellarchitected/latest/framework/ops_operations_health_dashboard.html)

---

## Evolve

### Continuous improvement

#### OPS10-BP01: Have a process for continuous improvement

**Description:** Regularly evaluate and prioritize opportunities for improvement to focus efforts where they can provide the most benefits.

**AWS Documentation:** [OPS10-BP01](https://docs.aws.amazon.com/wellarchitected/latest/framework/ops_event_response_event_incident_problem_process.html)

---

#### OPS10-BP02: Perform post-incident analysis

**Description:** Review customer-impacting events and identify the contributing factors and preventative actions. Use this information to develop mitigations to limit or prevent recurrence.

**AWS Documentation:** [OPS10-BP02](https://docs.aws.amazon.com/wellarchitected/latest/framework/ops_event_response_process_per_alert.html)

---

#### OPS10-BP03: Implement feedback loops

**Description:** Include feedback loops in your procedures and workloads to help you identify issues and areas that need improvement.

**AWS Documentation:** [OPS10-BP03](https://docs.aws.amazon.com/wellarchitected/latest/framework/ops_event_response_prioritize_events.html)

---

#### OPS10-BP04: Perform knowledge management

**Description:** Mechanisms exist for team members to discover the information that they are looking for in a timely manner, access it, and identify that it's current and complete.

**AWS Documentation:** [OPS10-BP04](https://docs.aws.amazon.com/wellarchitected/latest/framework/ops_event_response_define_escalation_paths.html)

---

#### OPS10-BP05: Define drivers for improvement

**Description:** Identify drivers for improvement to help you evaluate and prioritize opportunities. Key drivers include customer feedback, compliance requirements, new features, threat landscape, and performance targets.

**AWS Documentation:** [OPS10-BP05](https://docs.aws.amazon.com/wellarchitected/latest/framework/ops_event_response_comms_customer_impacting_events.html)

---

#### OPS10-BP06: Validate insights

**Description:** Review your analysis results and responses with cross-functional teams and business owners. Use these reviews to establish common understanding, identify additional impacts, and determine courses of action.

**AWS Documentation:** [OPS10-BP06](https://docs.aws.amazon.com/wellarchitected/latest/framework/ops_event_response_comms_status.html)

---

#### OPS10-BP07: Perform operations metrics reviews

**Description:** Regularly perform retrospective analysis of operations metrics with cross-team participants from different areas of the business.

**AWS Documentation:** [OPS10-BP07](https://docs.aws.amazon.com/wellarchitected/latest/framework/ops_event_response_automate_response.html)

---

#### OPS10-BP08: Document and share lessons learned

**Description:** Document and share lessons learned from your operations activities so that all teams can use them.

**AWS Documentation:** [OPS10-BP08](https://docs.aws.amazon.com/wellarchitected/latest/operational-excellence-pillar/ops10_bp08.html)

---

#### OPS10-BP09: Allocate time to make improvements

**Description:** Dedicate time and resources within your processes to make continuous incremental improvements possible.

**AWS Documentation:** [OPS10-BP09](https://docs.aws.amazon.com/wellarchitected/latest/operational-excellence-pillar/ops10_bp09.html)

---

#### OPS11-BP01: Have a process for continuous improvement

**Description:** Regularly evaluate and prioritize opportunities for improvement to focus efforts where they can provide the greatest benefits.

**AWS Documentation:** [OPS11-BP01](https://docs.aws.amazon.com/wellarchitected/latest/operational-excellence-pillar/ops_evolve_ops_process_cont_imp.html)

---

#### OPS11-BP02: Perform post-incident analysis

**Description:** Review customer-impacting events, and identify the contributing factors and preventative action items. Use this information to develop mitigations to limit or prevent recurrence.

**AWS Documentation:** [OPS11-BP02](https://docs.aws.amazon.com/wellarchitected/latest/framework/ops_evolve_ops_perform_rca_process.html)

---

#### OPS11-BP03: Implement feedback loops

**Description:** Include feedback loops in your procedures and workloads to help you identify issues and areas that need improvement.

**AWS Documentation:** [OPS11-BP03](https://docs.aws.amazon.com/wellarchitected/latest/operational-excellence-pillar/ops_evolve_ops_feedback_loops.html)

---

#### OPS11-BP04: Perform knowledge management

**Description:** Mechanisms exist for your team members to discover information to support their actions, and to use this knowledge to inform their decision-making.

**AWS Documentation:** [OPS11-BP04](https://docs.aws.amazon.com/wellarchitected/latest/operational-excellence-pillar/ops_evolve_ops_knowledge_management.html)

---
