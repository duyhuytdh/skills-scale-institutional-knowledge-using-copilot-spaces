# OctoAcme — Cross-Role Collaboration Guide

## Purpose
Provide clear guidance on how different roles interact, communicate, and hand off work to ensure smooth collaboration and minimize gaps in accountability.

## Key Collaboration Patterns

### Feature Development Workflow

#### Discovery & Definition Phase
**Primary Roles**: Product Manager, UI/UX Designer, Data Analyst, Compliance Lead

**Collaboration Pattern**:
1. **Product Manager** defines problem statement and success metrics
2. **Data Analyst** provides baseline metrics and usage data
3. **UI/UX Designer** conducts user research and creates initial designs
4. **Compliance Lead** reviews for regulatory requirements
5. **Product Manager** finalizes feature requirements and acceptance criteria

**Handoff Artifact**: Feature specification with user stories, designs, metrics, and compliance requirements

---

#### Planning & Estimation Phase
**Primary Roles**: Project Manager, Developers, QA/Testing, SRE, UI/UX Designer

**Collaboration Pattern**:
1. **Project Manager** facilitates planning session with all technical roles
2. **Developers** estimate implementation effort and identify technical risks
3. **SRE** assesses infrastructure and reliability requirements
4. **QA/Testing** defines testing approach and estimates testing effort
5. **UI/UX Designer** confirms design implementation feasibility
6. **Project Manager** creates project timeline and identifies dependencies

**Handoff Artifact**: Project plan with timeline, resource allocation, and risk register

---

#### Implementation Phase
**Primary Roles**: Developers, UI/UX Designer, SRE, QA/Testing

**Collaboration Pattern**:
1. **Developers** implement features according to specifications
2. **UI/UX Designer** reviews implementation for design fidelity
3. **SRE** reviews code for operational concerns (monitoring, scaling, security)
4. **Developers** address feedback and complete implementation
5. **QA/Testing** validates acceptance criteria and performs testing

**Handoff Artifact**: Completed, tested feature ready for release review

---

#### Release & Launch Phase
**Primary Roles**: SRE, Project Manager, Product Manager, Customer Success Manager, Data Analyst

**Collaboration Pattern**:
1. **SRE** prepares production environment and monitoring
2. **Project Manager** coordinates release communication plan
3. **SRE** executes deployment and monitors system health
4. **Customer Success Manager** prepares user communication and training materials
5. **Data Analyst** sets up dashboards to track success metrics
6. **Product Manager** monitors metrics and gathers initial feedback

**Handoff Artifact**: Release notes, deployment verification, monitoring dashboards

---

#### Post-Launch & Iteration Phase
**Primary Roles**: Customer Success Manager, Data Analyst, Product Manager, UI/UX Designer

**Collaboration Pattern**:
1. **Customer Success Manager** collects user feedback and monitors adoption
2. **Data Analyst** analyzes usage patterns and success metrics
3. **UI/UX Designer** identifies usability improvements
4. **Product Manager** synthesizes feedback for roadmap planning
5. **Project Manager** facilitates retrospective with delivery team

**Handoff Artifact**: Retrospective notes, metrics report, iteration priorities

---

## Common Handoff Points

### Design to Development
**From**: UI/UX Designer  
**To**: Developers

**What to hand off**:
- High-fidelity designs and interactive prototypes
- Design specifications (spacing, colors, typography)
- User flows and interaction patterns
- Accessibility requirements
- Assets and design system components

**Review checkpoint**: Design implementation review before code review approval

---

### Development to QA
**From**: Developers  
**To**: QA/Testing

**What to hand off**:
- Feature implementation in test environment
- Acceptance criteria and test cases
- Known limitations or edge cases
- Data setup requirements for testing

**Review checkpoint**: All automated tests passing, feature marked as "ready for QA"

---

### QA to Operations
**From**: QA/Testing  
**To**: SRE

**What to hand off**:
- Test results and coverage report
- Performance test results
- Known issues and workarounds
- Release notes draft

**Review checkpoint**: Release readiness review meeting

---

### Product to Customer Success
**From**: Product Manager  
**To**: Customer Success Manager

**What to hand off**:
- Feature overview and benefits
- Target customer segments
- Expected adoption timeline
- FAQs and talking points
- Training materials or demos

**Review checkpoint**: Pre-launch enablement session

---

## Communication Best Practices

### Synchronous Communication
- **Daily Standups**: Quick status updates, blockers, and coordination (15 min max)
- **Design Reviews**: Collaborative feedback on designs with designers, PMs, and developers
- **Planning Sessions**: Estimation and timeline creation with full delivery team
- **Incident Response**: Real-time coordination during outages or critical issues

### Asynchronous Communication
- **Pull Request Reviews**: Code review with comments and suggestions
- **Project Updates**: Written status reports shared via email or project board
- **Documentation**: Process docs, runbooks, and technical specifications in repo
- **Feedback Collection**: Surveys, forms, and async feedback tools

### Documentation Requirements
- **Feature Specifications**: What problem are we solving? What are the requirements?
- **Technical Design Docs**: How will we build it? What are the trade-offs?
- **Test Plans**: What scenarios will we test? What are pass/fail criteria?
- **Release Notes**: What changed? Who is impacted? What actions are needed?
- **Runbooks**: How do we operate, monitor, and troubleshoot this?

---

## Escalation Matrix

| Issue Type | First Contact | Escalation Path |
|------------|---------------|-----------------|
| Technical blocker | Developer → Tech Lead | Tech Lead → Project Manager → Engineering Manager |
| Design questions | UI/UX Designer | Designer → Product Manager → Design Lead |
| Compliance concern | Compliance Lead | Compliance → Project Manager → Legal |
| Customer escalation | Customer Success Manager | CSM → Product Manager → VP Customer Success |
| Production incident | SRE On-call | SRE → Engineering Manager → Incident Commander |
| Scope change | Project Manager | PM → Product Manager → Stakeholder Sponsor |
| Resource constraint | Project Manager | PM → Engineering Manager → Director |

---

## Tips for Effective Collaboration

1. **Over-communicate on handoffs**: Always confirm receipt and understanding when passing work between roles
2. **Document decisions**: Keep a decision log for significant choices and their rationale
3. **Use shared tools**: Maintain single source of truth (GitHub, project boards, shared docs)
4. **Define "done"**: Each handoff should have clear acceptance criteria
5. **Build in feedback loops**: Regular checkpoints prevent late-stage surprises
6. **Respect expertise**: Trust specialists in their domains while maintaining collaborative dialogue
7. **Make work visible**: Use project boards and status updates to maintain transparency
8. **Celebrate wins together**: Acknowledge cross-functional contributions to team success
