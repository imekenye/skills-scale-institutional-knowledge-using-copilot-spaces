# OctoAcme — Execution & Tracking

## Purpose
Guidance for managing day-to-day execution and tracking progress toward project milestones.

## Team Rhythm
- Daily standups (15 min) — focus on progress, blockers, dependencies
- Weekly delivery sync — show progress, updates, and flagged risks
- Demo/Review at the end of each sprint or milestone

## Workflows
- Use the project board (e.g., GitHub Projects) with columns: Backlog, Ready, In Progress, In Review, QA, Done
- Pull Request workflow:
  - Small PRs (<= 400 lines when possible)
  - Include issue link and acceptance criteria in PR description
  - Run automated tests and linting in CI before requesting review
  - Require at least one approval before merging (or team-defined policy)

## Quality & Testing
- Unit tests for new logic
- Integration tests where applicable
- End-to-end smoke tests for critical flows before release
- Security scanning in CI
- Manual QA for feature acceptance when needed

## Reporting & Metrics
- Track velocity and burndown
- Monitor success metrics identified in the Project One-pager
- Use dashboards for key signals (errors, latency, usage)

## Blocker Escalation
- Level 1: Team-level triage in daily standup
- Level 2: PM escalates to Product Lead and dependent teams
- Level 3: Sponsor-level escalation for business-impacting issues

## Execution Checklist
- [ ] Branching and PR conventions documented in repo
- [ ] CI configured for tests and lint
- [ ] Regular demos scheduled
- [ ] Risk register updated weekly

### Role-Specific Actions

**Developers:**
- [ ] Follow branching and PR conventions
- [ ] Write tests for new features and fixes
- [ ] Keep PR size manageable (≤400 lines)
- [ ] Respond to code review feedback promptly
- [ ] Update documentation for code changes
- [ ] Report blockers in daily standup

**Technical Lead:**
- [ ] Conduct code reviews within SLA (24-48 hours)
- [ ] Monitor code quality metrics and technical debt
- [ ] Provide technical guidance and mentoring
- [ ] Escalate architectural concerns early
- [ ] Review and approve major technical changes

**Product Manager:**
- [ ] Clarify requirements as questions arise
- [ ] Review and accept completed features
- [ ] Adjust priorities based on feedback and data
- [ ] Communicate scope changes to stakeholders
- [ ] Monitor success metrics and user feedback

**Business Analyst:**
- [ ] Answer requirement clarification questions
- [ ] Review implemented features against acceptance criteria
- [ ] Support UAT coordination and execution
- [ ] Document requirement changes and impacts

**UX Designer:**
- [ ] Provide design clarifications during development
- [ ] Review implementation against design specs
- [ ] Conduct usability testing on completed features
- [ ] Update designs based on implementation learnings

**Scrum Master:**
- [ ] Facilitate daily standups and sprint ceremonies
- [ ] Track and remove impediments
- [ ] Monitor team velocity and burndown
- [ ] Coach team on agile practices
- [ ] Facilitate retrospectives and continuous improvement

**Project Manager:**
- [ ] Update project status weekly
- [ ] Manage risk register and escalate issues
- [ ] Coordinate cross-team dependencies
- [ ] Communicate with stakeholders
- [ ] Track milestone progress and timelines

## Cross-Role Collaboration During Execution

### Daily Standup Coordination
**Scrum Master (Facilitator):**
- Keep standup timeboxed to 15 minutes
- Note blockers and action items
- Follow up on impediments after standup

**Team Participation Pattern:**
- Developers: Share progress, blockers, and plan for the day
- Technical Lead: Offer immediate help on technical blockers
- Product Manager: Clarify priorities if questions arise
- Business Analyst: Available for requirement questions
- UX Designer: Clarify design questions or review implementations

**Escalation Flow:**
- Level 1 (Team-Resolved): Scrum Master or Technical Lead resolves within the team
- Level 2 (Cross-Team): Project Manager coordinates with dependent teams
- Level 3 (Leadership): Product Manager escalates business-critical issues to leadership

### Work-in-Progress Collaboration

**Developer ↔ Technical Lead:**
- Pair programming sessions for complex features
- Architecture reviews before major changes
- Code review feedback loops

**Developer ↔ UX Designer:**
- Design review during implementation
- Feedback on design feasibility
- Accessibility and responsive behavior validation

**Developer ↔ Business Analyst:**
- Requirement clarification conversations
- Edge case discussions
- Acceptance criteria validation

**Product Manager ↔ Project Manager:**
- Weekly alignment on scope, risks, and timeline
- Stakeholder communication coordination
- Priority adjustment discussions

### Quality Gates and Handoffs

**Code Complete → Review (Technical Lead/Developers):**
- Automated tests pass
- Code review completed and approved
- Documentation updated

**Review → QA (Business Analyst/UX Designer):**
- Acceptance criteria met
- Design specifications followed
- Ready for testing

**QA → Done (Product Manager):**
- UAT passed
- No critical defects
- Stakeholder acceptance confirmed

### Communication Channels by Purpose

**Real-time Questions:**
- Direct message to Scrum Master or Technical Lead for immediate blockers
- Team chat channel for quick clarifications

**Asynchronous Updates:**
- PR comments for code-specific discussions
- Project board comments for task status
- Email/Slack for stakeholder updates

**Formal Reviews:**
- Sprint review for feature demonstrations
- Weekly status meeting for project health
- Monthly stakeholder briefings for roadmap updates

### Conflict Resolution

**Scope Disagreements:**
- Product Manager has final decision
- Business Analyst provides requirement clarity
- Technical Lead advises on technical impact

**Technical Disagreements:**
- Technical Lead facilitates discussion
- Team votes if consensus not reached
- Document decision in ADR (Architecture Decision Record)

**Priority Conflicts:**
- Product Manager prioritizes feature work
- Scrum Master balances with technical debt
- Project Manager considers dependencies and deadlines

**Resource Constraints:**
- Project Manager assesses options
- Scrum Master adjusts sprint scope
- Product Manager approves de-prioritization


