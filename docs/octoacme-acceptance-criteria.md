# OctoAcme — Acceptance Criteria Template & Quality Standards

## Purpose
Standardize how acceptance criteria are defined, documented, and verified to reduce ambiguity, rework, and quality issues.

## What Are Acceptance Criteria?
Acceptance criteria are the specific, measurable conditions that a feature or deliverable must meet to be considered complete and ready for release. They define the boundary between "done" and "not done."

---

## Acceptance Criteria Template

### Item: [Feature/Task Name]

**User Story (if applicable):**
```
As a [user/role], I want [capability], so that [business value]
```

**Description:**
[Brief summary of what is being delivered]

---

### Functional Acceptance Criteria

**Must-Haves (Required for release):**
- [ ] [Specific behavior/outcome that must occur]
- [ ] [Specific behavior/outcome that must occur]
- [ ] [Any integrations or dependencies that must work]

**Example:**
- [ ] Users can upload files up to 100 MB
- [ ] File upload completes within 30 seconds for a typical 50 MB file
- [ ] Uploaded files are visible in the user's dashboard within 2 seconds

---

### Non-Functional Acceptance Criteria

**Performance:**
- [ ] Page load time < 2 seconds
- [ ] API response time < 500 ms for 95th percentile
- [ ] Support 1000 concurrent users

**Usability & Accessibility:**
- [ ] Compliant with WCAG 2.1 AA standards
- [ ] Keyboard navigable
- [ ] Tested with screen readers

**Security:**
- [ ] All user input validated and sanitized
- [ ] Data encrypted in transit (HTTPS) and at rest
- [ ] Passed security scanning in CI/CD

**Reliability:**
- [ ] 99.5% uptime SLA during business hours
- [ ] Graceful error handling for all failure modes
- [ ] Rollback plan tested

---

### Testing & Verification

**Unit Tests:**
- [ ] Code coverage ≥ 80%
- [ ] All critical paths tested

**Integration Tests:**
- [ ] End-to-end workflows tested
- [ ] Third-party integrations verified

**User Acceptance Testing (UAT):**
- [ ] Product Manager sign-off
- [ ] Design verification (UX Designer)
- [ ] Approved by [Sponsor/Stakeholder Name]

**Security & Compliance:**
- [ ] Security review completed
- [ ] Privacy impact assessment (if data handling changes)
- [ ] Compliance checklist verified

---

### Definition of Done (DoD)

Before marking an item as "Done," verify:
- [ ] All acceptance criteria met and verified
- [ ] Code reviewed and approved by at least one peer
- [ ] Automated tests passing (unit, integration, security)
- [ ] Documentation updated (code comments, README, design docs)
- [ ] Accessibility compliance verified
- [ ] Performance benchmarks met
- [ ] Deployment/infrastructure changes documented
- [ ] Feature flags configured (if applicable)
- [ ] Rollback plan documented
- [ ] Release notes drafted

---

## Writing Effective Acceptance Criteria: Best Practices

### ✅ DO:
- **Be specific:** Use measurable, quantifiable outcomes
  - ✅ "Users receive an email within 2 minutes of signup"
  - ❌ "Users receive an email quickly"

- **Write from the user/system perspective:** Focus on observable behavior
  - ✅ "Dashboard displays real-time metrics"
  - ❌ "Code refactored for performance"

- **Make them testable:** Each criterion should be verifiable
  - ✅ "Search results return within 1 second and show top 10 matches"
  - ❌ "Search works well"

- **Keep them independent:** Each criterion stands on its own
  - ✅ Multiple specific criteria
  - ❌ Nested or dependent criteria

- **Prioritize:** Distinguish must-haves from nice-to-haves
  - Mark critical items as blockers
  - Use labels: "MVP", "Nice-to-have", "Future enhancement"

---

### ❌ DON'T:
- **Use vague language:** Avoid words like "good," "fast," "user-friendly"
- **Include implementation details:** Focus on the "what," not the "how"
- **Create overly complex criteria:** Keep each criterion focused
- **Forget edge cases:** Include error scenarios and boundary conditions

---

## Acceptance Criteria by Role

### Product Manager's Perspective
- Business value and success metrics
- User workflows and scenarios
- Regulatory/compliance requirements
- Priority and dependencies

### Developer's Perspective
- Technical integration points
- Performance and scalability requirements
- Code quality and test coverage
- Deployment and configuration

### QA's Perspective
- Test cases and scenarios
- Edge cases and error handling
- Performance and load testing
- Compliance and security verification

### UX Designer's Perspective
- Design consistency and branding
- Accessibility and usability
- User feedback and testing results
- Visual regression prevention

---

## Examples by Scenario

### Example 1: Feature Addition

**Item:** Add "Remember Me" functionality to login

**User Story:**
```
As a returning user, I want the option to stay logged in, so I don't have to re-enter credentials on every visit
```

**Functional Criteria:**
- [ ] Login form includes optional "Remember Me" checkbox
- [ ] When checked, session persists for 30 days
- [ ] Unchecked by default for security
- [ ] Users can manually logout anytime
- [ ] Session expires after 30 days regardless of activity

**Security Criteria:**
- [ ] Session token securely stored (httpOnly cookie)
- [ ] Token rotation on each login
- [ ] No sensitive data stored client-side

**Testing:**
- [ ] Unit tests for session management (90%+ coverage)
- [ ] Integration tests for cookie handling across browsers
- [ ] Security review: OWASP Top 10 compliance

---

### Example 2: Bug Fix

**Item:** Fix: Dashboard chart fails to load on slow networks

**User Story:**
```
As a user on a slow network, I want the dashboard to load gracefully with a loading indicator, so I know something is happening
```

**Functional Criteria:**
- [ ] Dashboard displays loading skeleton/spinner while fetching data
- [ ] Chart loads within 10 seconds on 3G network (simulated)
- [ ] Error message displayed if fetch times out after 15 seconds
- [ ] Users can retry loading the chart

**Performance Criteria:**
- [ ] Initial page load < 3 seconds on slow network
- [ ] Chart data chunk size optimized (< 500 KB)

**Testing:**
- [ ] Network throttling tests (Fast 3G, Slow 3G, Offline)
- [ ] Error scenario coverage (timeout, 500 error, malformed data)

---

### Example 3: Infrastructure / DevOps

**Item:** Migrate database to managed service

**Acceptance Criteria:**
- [ ] Zero-downtime migration achieved
- [ ] Data integrity verified (row count, checksums)
- [ ] Replication lag < 100 ms
- [ ] Automated backups configured
- [ ] Performance benchmarks met (query latency within 5% of baseline)
- [ ] Disaster recovery tested and documented
- [ ] Cost savings validated vs. current infrastructure

**Rollback Criteria:**
- [ ] Rollback procedure tested and documented
- [ ] Rollback time < 15 minutes
- [ ] No data loss during rollback

---

## Acceptance Criteria Review Checklist

Before moving to development, verify:
- [ ] All criteria are written in clear, non-technical language
- [ ] Acceptance criteria are independent of implementation
- [ ] Success metrics are measurable and achievable
- [ ] Edge cases and error scenarios are included
- [ ] Performance and security requirements are specified
- [ ] Team agrees on priority (MVP vs. enhancements)
- [ ] Owner assigned for each criterion or verification step
- [ ] Timeline is realistic for verification efforts

---

## Verification Process

### During Development
- Developers verify each criterion as work progresses
- QA creates test cases aligned to criteria
- Designer verifies visual/usability criteria

### Before QA Handoff
- Developer: "I believe all criteria are met"
- Code review confirms implementation aligns to criteria

### During QA Testing
- QA executes test cases for each criterion
- QA documents results (pass/fail)
- QA identifies gaps or issues

### Before Release
- Product Manager: Final acceptance sign-off
- UX Designer: Design verification (if applicable)
- Release Manager: Compliance and deployment readiness

---

## Acceptance Criteria Tracking

Track criteria status in your project management tool (GitHub Issues, Jira, etc.):
- [ ] Criterion 1: In Progress (Dev)
- [ ] Criterion 2: In Progress (QA)
- [ ] Criterion 3: Complete ✓
- [ ] Criterion 4: Blocked (awaiting design)

Update status in daily standup and weekly sync.
