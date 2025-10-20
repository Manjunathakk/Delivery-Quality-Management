The Delivery Quality Assurance (DQA) Dashboard is designed to provide an end-to-end view of IT delivery performance and quality compliance.It combines delivery health metrics, risk and issue tracking, SLA monitoring, and quality gate compliance — empowering delivery managers, PMOs, and business stakeholders to ensure projects meet agreed service levels (MSA/SoW).

**Objectives**
Track overall delivery performance across multiple projects.
Measure and visualize timeliness, cost adherence, and scope stability.
Provide actionable insights into code quality, test coverage, and security compliance.
Monitor SLA adherence and risk severity trends in real time.
Enable data-driven governance through unified Power BI visuals.

**Key DAX calculations used in the dashboard**
% Security Pass Checked = DIVIDE(CALCULATE(COUNTROWS(FILTER('Delivery Quality Mgmt', 'Delivery Quality Mgmt'[SecurityChecksPassed] = "Yes"))), COUNTROWS('Delivery Quality Mgmt'))

% SLA Breached = DIVIDE(CALCULATE(COUNTROWS(FILTER('Delivery Quality Mgmt', 'Delivery Quality Mgmt'[SLA_Breached]="Yes"))), COUNTROWS('Delivery Quality Mgmt'))

Avg Timeline % = AVERAGE('Delivery Quality Mgmt'[TimelinessScore])

Cost Adherence % = AVERAGE('Delivery Quality Mgmt'[CostAdherencePercent])
Customer Satisfaction Trends = AVERAGE('Delivery Quality Mgmt'[CustomerSatisfactionScore])

Quality Gate Pass % = DIVIDE(CALCULATE(COUNTROWS(FILTER('Delivery Quality Mgmt', 'Delivery Quality Mgmt'[QualityGateStatus] = " Passed"))), COUNTROWS('Delivery Quality Mgmt'))

<img width="875" height="470" alt="image" src="https://github.com/user-attachments/assets/db54e24b-1eb8-48c5-bdde-5c5048732cca" />


**Insights for Stakeholders**
Delivery Managers can track deviations early and prevent SLA breaches.
PMOs gain visibility into scope creep, testing quality, and overall cost adherence.
Business Owners can monitor customer satisfaction & quality gate health before deployment.

Data Source : Open AI Generated
