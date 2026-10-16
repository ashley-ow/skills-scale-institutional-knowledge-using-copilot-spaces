# OctoAcme Personas

This document defines typical roles and responsibilities used in OctoAcme project docs and exercises.

---

## Developers

### Role Summary
Developers design, build, test, and deliver software components. They collaborate with product and project leads to implement features that meet acceptance criteria and quality standards.

### Responsibilities
- Implement features and fixes to meet acceptance criteria
- Write and maintain tests and documentation
- Participate in design and code reviews
- Assist in estimating and planning work
- Help identify technical risks and propose mitigations

### Goals
- Deliver reliable, maintainable code
- Reduce cycle time from idea to production
- Maintain high test coverage and observability

### Typical Communication
- Daily standups and sprint planning
- PR descriptions and code review comments
- Technical design docs when needed

---

## Product Managers

### Role Summary
Product Managers define what should be built to deliver customer and business value. They own the product vision, prioritize the backlog, and measure outcomes.

### Responsibilities
- Define problem statements and success metrics
- Prioritize the roadmap and backlog
- Collaborate with stakeholders and engineering on trade-offs
- Validate solutions through user research and metrics

### Goals
- Maximize customer value and impact
- Make clear, data-driven prioritization decisions
- Ensure product-market fit and usability

### Typical Communication
- Weekly alignment with PM and engineering leads
- Roadmap updates and stakeholder briefings
- Acceptance criteria and feature specs

---

## Project Managers

### Role Summary
Project Managers coordinate delivery activities, manage schedules, risks, and communications. They enable the team to deliver on commitments efficiently.

### Responsibilities
- Create and maintain project plans and timelines
- Manage risks, dependencies, and resource constraints
- Facilitate meetings (kickoff, planning, retrospectives)
- Ensure consistent project documentation and status reporting
- Coordinate cross-team and stakeholder communication

### Goals
- Deliver projects on time and within scope
- Minimize unplanned work and escalations
- Maintain transparency and alignment across stakeholders

### Typical Communication
- Weekly status updates and stakeholder reports
- Risk registers and decision logs
- Coordination via project boards and meeting facilitation

---

## Additional Personas (proposed additions)

The following personas are proposed to add clarity around cross-functional responsibilities, technical coordination, release ownership, observability, and stakeholder-surface points. Each persona description includes a short role summary, responsibilities, and how they interact with existing roles.

### Technical Program Manager (TPM)
Role Summary:
The TPM coordinates cross-team technical dependencies, sequences work across engineering teams, and keeps technical milestones aligned with the project plan.

Responsibilities:
- Maintain cross-team dependency map and technical milestone schedule
- Facilitate technical design alignment and integration planning
- Track technical risks; coordinate mitigations across teams
- Drive technical readiness gates for milestones and releases

Interactions:
- Works with Project Managers on timelines and risk communications
- Partners with Product Managers on scope trade-offs where technical constraints exist
- Coordinates with Engineering Managers and Developers to resolve cross-repo or cross-team blockers
- Escalates unresolved technical dependencies to leadership when necessary

Typical Deliverables / Communication:
- Dependency register, integration plan, milestone readiness checklist
- Regular syncs with engineering leads and PM

### Release Engineer / Release Lead
Role Summary:
Owns the release pipeline and the mechanics of deploying changes safely to environments; responsible for rollback plans and post-release verification.

Responsibilities:
- Maintain and improve CI/CD pipelines and automation
- Author and own release runbooks and rollback procedures
- Coordinate release windows and ensure pre-release checks pass
- Validate post-deploy smoke tests and hand off any incidents

Interactions:
- Works with Developers to ensure PRs meet CI standards
- Collaborates with QA on release verification steps and acceptance checks
- Notifies PM and Support Liaison of release schedules and notable changes

Typical Deliverables / Communication:
- Release checklist, deployment playbooks, post-deploy verification reports

### UX Researcher / Designer
Role Summary:
Validates design assumptions and crafts user experiences that meet product goals; supplies acceptance criteria focused on usability.

Responsibilities:
- Conduct user research and usability testing
- Produce wireframes, prototypes, and design specs
- Define usability acceptance criteria and measure UX outcomes
- Collaborate on accessibility and design consistency

Interactions:
- Partners with Product Managers to translate requirements into user-centered designs
- Works with Developers and QA to ensure designs are implemented faithfully and tested for usability
- Provides artifacts and findings that inform acceptance criteria and success metrics

Typical Deliverables / Communication:
- Research findings, prototypes, design specs, usability test reports

### Data Analyst / Analytics Owner
Role Summary:
Defines and validates success metrics, implements instrumentation, and produces dashboards that inform product decisions.

Responsibilities:
- Define event/metric schema and measurable success criteria
- Validate that telemetry and instrumentation are implemented correctly
- Build dashboards and reports for stakeholders
- Run analyses to support prioritization and post-release evaluation

Interactions:
- Works with Product Managers to define success metrics and KPIs
- Coordinates with Developers on instrumentation work and QA on telemetry tests
- Shares regular insights with PM/PD and the team during planning and retrospectives

Typical Deliverables / Communication:
- Dashboard(s), instrumentation spec, analysis reports, measurement plan

### Security Reviewer / Security Champion
Role Summary:
Performs feature-level security reviews and advocates for secure design throughout the delivery lifecycle.

Responsibilities:
- Lead threat modeling and security reviews for significant features
- Ensure security scans and compliance checks are part of CI gates
- Define remediation steps and advise on secure implementation patterns
- Act as an escalation point for security-related risks and incidents

Interactions:
- Works with Developers to implement remediations and secure coding practices
- Coordinates with Release Lead on security gates for production deployments
- Communicates security risk and mitigation to PM and stakeholders when necessary

Typical Deliverables / Communication:
- Threat model artifacts, security review notes, remediation tickets

### Observability / SRE Liaison
Role Summary:
Ensures system reliability by advising on monitoring, alerts, SLI/SLOs, and operational runbooks for new features.

Responsibilities:
- Define monitoring requirements and alerting thresholds for releases
- Advise on SLI/SLO targets and instrumentation needs
- Help produce runbooks for incident response and post-deploy checks
- Participate in post-incident reviews and propose improvements

Interactions:
- Works with Developers on instrumentation and observability implementation
- Collaborates with Release Lead on post-deploy verification and alerting readiness
- Coordinates with PM on risk and operational readiness for releases

Typical Deliverables / Communication:
- Monitoring pact, runbooks, SLI/SLO definitions, observability checklist

### Support Liaison / Customer Operations Representative
Role Summary:
Represents support and customer-facing operations to ensure smooth handoffs, clear escalation paths, and that user-reported issues are triaged efficiently.

Responsibilities:
- Surface common support issues and customer pain points to the team
- Ensure runbooks and escalation contacts are up-to-date
- Coordinate with PM on prioritization of customer-impacting issues
- Prepare support-facing release notes and known issue guidance

Interactions:
- Works with PM and PdM to prioritize bug fixes and customer requests
- Coordinates with Developers on triage, reproductions, and fixes
- Receives deployment notifications from Release Lead and prepares support channels

Typical Deliverables / Communication:
- Support runbooks, triage notes, customer-impact reports, release notifications

---

## How these personas are used in the exercise
- Use these persona definitions to frame scenarios and sample interactions in the Skills Exercise.
- Each persona can be used as a persona prompt for Copilot Spaces to shape role-specific guidance.
