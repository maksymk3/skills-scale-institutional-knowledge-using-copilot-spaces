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

### Interactions with Other Roles
- **Product Manager:** Clarifies requirements; accepts completed features
- **QA / Testing:** Provides code and accepts test feedback
- **UX Designer:** Implements design specs; participates in design reviews
- **Solutions Architect:** Consults on technical approach and scalability
- **Release Manager:** Coordinates deployment timing and processes

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

### Interactions with Other Roles
- **Project Manager:** Coordinates delivery timeline; escalates risks
- **Developers:** Defines requirements; reviews implementation
- **QA / Testing:** Defines acceptance criteria; validates quality
- **UX Designer:** Collaborates on user experience and requirements
- **Customer Support:** Gathers customer feedback and issues
- **Solutions Architect:** Evaluates technical feasibility of features

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

### Interactions with Other Roles
- **Product Manager:** Aligns on priorities and scope; manages trade-offs
- **Developers:** Tracks progress; unblocks team impediments
- **QA / Testing:** Coordinates testing schedule; tracks quality metrics
- **Release Manager:** Coordinates deployment readiness and timing
- **Stakeholders:** Provides status updates and escalations

---

## UX Designer

### Role Summary
UX Designers lead the discovery, design, and validation of user-centric solutions. They ensure that products are intuitive, accessible, and meet user needs while aligning with business goals.

### Responsibilities
- Conduct user research and usability testing
- Create wireframes, prototypes, and design specifications
- Design for accessibility (WCAG compliance, keyboard navigation, screen readers)
- Collaborate with developers to ensure design implementation fidelity
- Iterate on designs based on user feedback and testing results
- Define interaction patterns and design systems

### Goals
- Deliver user-centric, accessible, and delightful experiences
- Reduce usability issues and support burden through better design
- Establish consistent design language and interaction patterns

### Typical Communication
- Design reviews and feedback sessions
- Figma/Sketch design assets and specifications
- Accessibility checklists and design system documentation
- Usability testing reports and insights

### Interactions with Other Roles
- **Product Manager:** Aligns on user needs and feature priorities
- **Developers:** Provides design specs; reviews implementation for fidelity
- **QA / Testing:** Participates in UAT; verifies accessibility compliance
- **Project Manager:** Communicates design timeline and dependencies
- **Solutions Architect:** Discusses technical constraints and feasibility

---

## Solutions Architect

### Role Summary
Solutions Architects shape the overall system architecture, evaluate technical trade-offs, and ensure solutions align with enterprise standards, scalability, and security requirements. They guide the technical direction and integration strategy.

### Responsibilities
- Design system architecture and technical approach
- Evaluate technology choices and trade-offs (performance, cost, maintainability)
- Ensure solutions align with enterprise standards, security, and compliance
- Guide integration with existing systems and external services
- Review technical implementation for scalability, performance, and resilience
- Identify technical risks and propose mitigations

### Goals
- Build scalable, secure, and maintainable solutions
- Minimize technical debt and rework
- Ensure alignment with enterprise standards and best practices

### Typical Communication
- Architecture design documents and diagrams
- Technical RFC (Request for Comments) reviews
- Code reviews and architecture reviews
- Technical decision logs

### Interactions with Other Roles
- **Developers:** Guides technical implementation; reviews code
- **Product Manager:** Advises on technical feasibility of features
- **Project Manager:** Identifies technical risks and timeline impacts
- **QA / Testing:** Advises on performance and security testing strategies
- **Release Manager:** Guides deployment architecture and rollback strategy

---

## Release Manager

### Role Summary
Release Managers coordinate release planning, oversee deployment logistics, manage the release calendar, and ensure smooth transitions to production. They minimize release risks through careful planning and communication.

### Responsibilities
- Plan release schedules and coordinate timing across teams
- Prepare deployment procedures and runbooks
- Coordinate staging environment deployments and smoke testing
- Execute production deployments (or orchestrate automated pipelines)
- Monitor post-release health and coordinate incident response
- Communicate release status and changes to stakeholders and support teams
- Manage rollback procedures and contingency planning

### Goals
- Execute smooth, zero-downtime deployments
- Minimize production incidents and their impact
- Maintain clear communication throughout release process

### Typical Communication
- Release readiness checklists and deployment plans
- Release notes and change summaries
- Deployment timelines and communication schedules
- Post-release monitoring and incident reports

### Interactions with Other Roles
- **Developers:** Coordinates code freeze and deployment timing
- **QA / Testing:** Ensures readiness criteria met before deployment
- **Product Manager:** Communicates feature availability to customers
- **Project Manager:** Coordinates release schedule
- **Customer Support:** Briefs on changes and support procedures
- **DevOps:** Executes infrastructure and deployment automation

---

## QA / Testing

### Role Summary
QA and Testing specialists ensure that solutions meet acceptance criteria, quality standards, and performance requirements. They validate functionality, identify issues, and provide assurance before release.

### Responsibilities
- Develop test plans and test cases aligned to acceptance criteria
- Execute functional, integration, performance, and security testing
- Document test results and maintain test artifacts
- Identify, triage, and track defects through resolution
- Validate non-functional requirements (performance, accessibility, security)
- Provide quality metrics and readiness recommendations
- Participate in UAT with stakeholders and end-users

### Goals
- Ensure quality and reliability of delivered solutions
- Identify issues early to reduce production incidents
- Validate that acceptance criteria are met before release

### Typical Communication
- Test plans and test case documentation
- Test execution reports and defect logs
- Quality metrics and release readiness assessments
- UAT coordination and sign-off

### Interactions with Other Roles
- **Developers:** Reports issues; validates fixes; collaborates on edge cases
- **Product Manager:** Clarifies acceptance criteria; prioritizes issues
- **UX Designer:** Verifies design implementation and accessibility
- **Project Manager:** Tracks testing progress and blockers
- **Release Manager:** Confirms readiness for deployment

---

## Customer Support / Customer Success

### Role Summary
Customer Support and Success teams serve as the primary contact for post-release support, gather user feedback, and communicate issues and feature requests back to the product and engineering teams. They ensure customer satisfaction and drive continuous improvement.

### Responsibilities
- Provide technical support to customers and resolve issues
- Gather user feedback and pain points from customer interactions
- Escalate bugs, feature requests, and issues to Product and Engineering teams
- Create and maintain support documentation and FAQs
- Communicate product updates and changes to customers
- Participate in onboarding and training for new customers
- Contribute to retrospectives by sharing customer impact and satisfaction

### Goals
- Maximize customer satisfaction and reduce support burden
- Provide timely feedback loop to product and engineering teams
- Enable customers to succeed with the product

### Typical Communication
- Support tickets and issue reports
- Customer feedback summaries and usage patterns
- Support documentation and runbooks
- Customer communication and announcements

### Interactions with Other Roles
- **Product Manager:** Escalates customer feedback and feature requests
- **Developers:** Reports issues; validates fixes; provides workarounds
- **Project Manager:** Communicates timeline for fixes and features
- **Release Manager:** Receives briefing on releases and coordinates customer communication
- **QA / Testing:** Coordinates UAT with customers (when applicable)

---

## How these personas are used in the exercise
- Use these persona definitions to frame scenarios and sample interactions in the Skills Exercise.
- Each persona can be used as a persona prompt for Copilot Spaces to shape role-specific guidance.
- Reference the interactions section to understand cross-functional dependencies and communication paths.
