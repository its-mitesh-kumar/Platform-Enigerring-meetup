# Enhance Engineering Productivity with Red Hat Developer Hub

**Mitesh Kumar**  
Senior Software Engineer, Red Hat  
Platform Engineering Meetup Bengaluru - Nov 29, 2025

---

## Agenda (25 mins)

1. The Developer Productivity Challenge (3 mins)
2. What is Backstage? (3 mins)
3. What is Red Hat Developer Hub? (3 mins)
4. Key Features & Capabilities (7 mins)
5. Real-world Use Cases (5 mins)
6. Demo & Architecture (4 mins)
7. Q&A (1 min)

---

## The Developer Productivity Challenge

### Common Pain Points

- **Context Switching**: Developers spend 30-40% of their time navigating between tools
- **Tool Sprawl**: 10+ different tools for monitoring, CI/CD, docs, APIs
- **Onboarding Friction**: New developers take weeks to become productive
- **Knowledge Silos**: Critical information scattered across wikis, Slack, emails
- **Repetitive Tasks**: Creating services, setting up pipelines, configuring infrastructure

### The Cost

- Slower time to market
- Increased cognitive load
- Developer burnout
- Inconsistent practices across teams

---

## What is Backstage?

### Open-Source Developer Portal Framework

**Created by Spotify** in 2016, open-sourced in 2020  
**CNCF Incubating Project** since 2022

### The Origin Story

**Spotify's Problem:**
- 2000+ engineers
- 4000+ microservices
- Exponential complexity
- No single source of truth

**Their Solution:**
Built an internal platform called **Backstage** to unify the developer experience

### Why Backstage?

**The Vision:**
> "End the chaos of different tools, documentation, and processes. Give developers a single, unified portal."

**Core Principles:**
1. **Centralized Software Catalog** - All services, APIs, and resources in one place
2. **Standardized Tooling** - Plugin-based architecture for integrations
3. **Self-Service Actions** - Templates for creating new projects
4. **Extensible Platform** - Build your own features and workflows

### Backstage Architecture

**Three Core Features:**

```
┌─────────────────────────────────────────────────────────┐
│                    BACKSTAGE CORE                        │
│                                                          │
│  ┌────────────────┐  ┌────────────────┐  ┌───────────┐ │
│  │   SOFTWARE     │  │   SOFTWARE     │  │ TECHDOCS  │ │
│  │   CATALOG      │  │   TEMPLATES    │  │           │ │
│  │                │  │                │  │           │ │
│  │ • Discovery    │  │ • Scaffolding  │  │ • Docs    │ │
│  │ • Metadata     │  │ • Automation   │  │ • Search  │ │
│  │ • Ownership    │  │ • Best Practice│  │ • MkDocs  │ │
│  └────────────────┘  └────────────────┘  └───────────┘ │
│                                                          │
│  ┌─────────────────────────────────────────────────────┐│
│  │          PLUGIN ECOSYSTEM (100+ Plugins)            ││
│  │  GitHub • Jenkins • Kubernetes • Prometheus • ...   ││
│  └─────────────────────────────────────────────────────┘│
└─────────────────────────────────────────────────────────┘
```

### Backstage Adoption

**Companies Using Backstage:**
- Spotify (originator)
- Netflix
- American Airlines
- HP
- Epic Games
- Expedia
- Zalando
- DAZN
- And 1000+ more organizations

**Why So Popular?**
- ✅ Open source (Apache 2.0)
- ✅ Battle-tested at scale (Spotify)
- ✅ Active community (100+ contributors)
- ✅ Extensible (plugin architecture)
- ✅ Cloud-agnostic
- ✅ No vendor lock-in

### The Challenge with Backstage

**Backstage is Powerful, BUT...**

**It's a Framework, Not a Product:**
- Requires setup and configuration
- Need to build and maintain
- Plugin integration takes effort
- No enterprise support out of the box
- Security hardening needed
- Scaling requires expertise

**Typical Setup Time:**
- Basic installation: 1-2 days
- Production-ready: 2-4 weeks
- Full customization: 2-3 months

**This is where Red Hat Developer Hub comes in!**

---

## What is Red Hat Developer Hub (RHDH)?

### Backstage + Enterprise = RHDH

**Red Hat Developer Hub** is Backstage, enterprise-ready!

### The Value Proposition

**Backstage:** Powerful framework, requires significant setup  
**RHDH:** Production-ready product, works out of the box

```
┌─────────────────────────────────────────────────────────┐
│         BACKSTAGE (Open Source Framework)                │
│                        +                                 │
│    Red Hat Enterprise Features & Support                │
│                        =                                 │
│         RED HAT DEVELOPER HUB (Product)                  │
└─────────────────────────────────────────────────────────┘
```

### What Red Hat Adds

**1. Enterprise-Ready Out of the Box**
- Pre-configured for production
- Hardened security
- HA deployment configurations
- Performance optimizations

**2. Dynamic Plugin System**
- Load plugins without rebuilding
- Update plugins independently
- No need to fork Backstage

**3. Red Hat Ecosystem Integration**
- OpenShift (native Kubernetes)
- Tekton (cloud-native CI/CD)
- Quay (container registry)
- Ansible (automation)
- Red Hat SSO (identity management)

**4. Enterprise Support**
- Red Hat support team
- SLA guarantees
- Regular security updates
- Migration assistance

**5. Pre-Built Templates & Plugins**
- Ready-to-use service templates
- Common workflow patterns
- Best practices built-in

### Core Philosophy

**"Shift complexity left, but make it invisible"**

- Single pane of glass for developers
- Self-service infrastructure
- Golden paths without guardrails
- Knowledge democratization

### Key Differentiators: RHDH vs Backstage OSS

| Feature | Backstage OSS | RHDH |
|---------|---------------|------|
| **Core Platform** | ✅ | ✅ |
| **Open Source** | ✅ | ✅ |
| **Setup Time** | Days-Weeks | Hours |
| **Production Ready** | DIY | ✅ |
| **Dynamic Plugins** | ❌ | ✅ |
| **Enterprise Support** | ❌ | ✅ |
| **Red Hat Integration** | Partial | ✅ |
| **Pre-configured** | ❌ | ✅ |
| **Security Hardening** | DIY | ✅ |

### Who Should Use What?

**Use Backstage OSS if:**
- You want maximum customization
- You have dedicated platform team
- You're comfortable with DIY approach
- Cost is primary concern

**Use RHDH if:**
- You need production-ready quickly
- You want enterprise support
- You use Red Hat ecosystem
- You prefer product over framework
- You want predictable costs

---

## Architecture Overview

```
┌─────────────────────────────────────────────────────────────┐
│                    RHDH Frontend (React)                    │
│  ┌──────────┐  ┌──────────┐  ┌──────────┐  ┌──────────┐   │
│  │ Software │  │   Tech   │  │   API    │  │  Docs    │   │
│  │ Catalog  │  │   Docs   │  │  Explorer│  │  Search  │   │
│  └──────────┘  └──────────┘  └──────────┘  └──────────┘   │
└─────────────────────────────────────────────────────────────┘
                              │
┌─────────────────────────────────────────────────────────────┐
│                    RHDH Backend (Node.js)                   │
│  ┌──────────┐  ┌──────────┐  ┌──────────┐  ┌──────────┐   │
│  │  Catalog │  │ Template │  │  Search  │  │   Auth   │   │
│  │  Engine  │  │  Engine  │  │  Engine  │  │  Engine  │   │
│  └──────────┘  └──────────┘  └──────────┘  └──────────┘   │
└─────────────────────────────────────────────────────────────┘
                              │
┌─────────────────────────────────────────────────────────────┐
│                    Plugin Ecosystem                          │
│  ┌──────────┐  ┌──────────┐  ┌──────────┐  ┌──────────┐   │
│  │  GitHub  │  │ Jenkins  │  │Kubernetes│  │  Tekton  │   │
│  │  GitLab  │  │   Argo   │  │  Quay    │  │ Ansible  │   │
│  └──────────┘  └──────────┘  └──────────┘  └──────────┘   │
└─────────────────────────────────────────────────────────────┘
```

---

## Key Feature #1: Software Catalog

### Centralized Service Discovery

**What it does:**
- Single source of truth for all software assets
- Components, APIs, Resources, Systems, Domains
- Automatic discovery from Git repositories

**Metadata-Driven**

```yaml
apiVersion: backstage.io/v1alpha1
kind: Component
metadata:
  name: payment-service
  description: Handles payment processing
  tags:
    - java
    - spring-boot
    - critical
  annotations:
    github.com/project-slug: acme/payment-service
spec:
  type: service
  lifecycle: production
  owner: payments-team
  system: e-commerce
```

**Benefits:**
- ✅ "Who owns this service?"
- ✅ "What APIs are available?"
- ✅ "Which services depend on this?"

---

## Key Feature #2: Software Templates

### Self-Service Project Scaffolding

**Golden Path Templates**

Pre-configured project templates with best practices baked in:
- Repository setup (GitHub/GitLab)
- CI/CD pipelines (Tekton, Jenkins, GitHub Actions)
- Infrastructure as Code (Kubernetes manifests, Helm charts)
- Documentation structure
- Security scanning

**Example: Creating a Microservice**

1. Developer selects "Spring Boot Microservice" template
2. Fills in: service name, team, repository location
3. RHDH creates:
   - Git repository with code structure
   - Tekton pipeline for CI/CD
   - Kubernetes deployment manifests
   - Monitoring dashboards
   - Documentation site
4. Developer starts coding in 5 minutes!

**Impact:**
- 🚀 **80% faster** project bootstrapping
- 🎯 **Consistent** practices across teams
- 🔒 **Security** by default

---

## Key Feature #3: TechDocs

### Documentation as Code

**Docs-like-code approach:**
- Markdown files in your repo
- Auto-generated from MkDocs
- Lives alongside source code
- Version controlled

**Features:**
- Full-text search across all docs
- Component-level documentation
- API documentation integration
- Automatic updates on commits

**Example Structure:**
```
my-service/
├── src/
├── docs/
│   ├── index.md
│   ├── architecture.md
│   ├── api.md
│   └── deployment.md
└── mkdocs.yml
```

**Benefits:**
- ✅ Reduced context switching
- ✅ Always up-to-date
- ✅ Discoverable via catalog

---

## Key Feature #4: Plugin Ecosystem

### Extensibility at Core

**100+ Community Plugins**

**DevOps & CI/CD:**
- GitHub Actions, Jenkins, Tekton, ArgoCD
- Real-time build status in catalog

**Cloud & Infrastructure:**
- Kubernetes, OpenShift, AWS, Azure
- Resource topology & health

**Monitoring & Observability:**
- Prometheus, Grafana, Dynatrace
- Service metrics in one view

**Security & Compliance:**
- SonarQube, Snyk, Trivy
- Security scores per component

**Dynamic Plugin System (RHDH)**
- Load plugins without rebuilding
- Enterprise-ready plugins
- Custom plugin development

---

## Key Feature #5: Developer Portal

### Unified Developer Experience

**Single Dashboard View:**

```
┌─────────────────────────────────────────────────────────┐
│  My Services (5)                    My PRs (3)          │
│  ┌──────────────┐ ┌──────────────┐  ┌──────────────┐   │
│  │ payment-svc  │ │ user-api     │  │ PR #234      │   │
│  │ ✓ Healthy    │ │ ⚠ Warning    │  │ Needs Review │   │
│  │ 99.9% uptime │ │ High CPU     │  └──────────────┘   │
│  └──────────────┘ └──────────────┘                     │
│                                                         │
│  Recent Builds                   On-Call Rotation      │
│  ┌──────────────────┐           ┌──────────────────┐   │
│  │ ✓ Build #123     │           │ This week: You   │   │
│  │ ✗ Build #122     │           │ Next: Sarah      │   │
│  └──────────────────┘           └──────────────────┘   │
└─────────────────────────────────────────────────────────┘
```

**Everything a developer needs:**
- Personal dashboard
- Team activity feed
- Shortcuts to common tasks
- Integration with existing tools

---

## Real-World Use Case #1: Fast Onboarding

### Before RHDH

**New Developer - Day 1:**
- Request access to 15 different tools
- Read through 20 confluence pages
- Ask 10+ questions in Slack
- Still confused about architecture

**Week 1:**
- Still setting up local environment
- Don't know which services exist
- Unsure about deployment process

### After RHDH

**New Developer - Day 1:**
- Single SSO login to RHDH
- Browse software catalog
- Understand system architecture visually
- Read up-to-date TechDocs

**Day 2:**
- Create first microservice from template
- Working CI/CD pipeline ready
- Successfully deploy to dev environment
- Contributing code!

**Result: Onboarding time reduced from 2 weeks to 2 days**

---

## Real-World Use Case #2: Microservices Management

### The Challenge

**E-commerce Platform:**
- 150+ microservices
- 30 development teams
- Multiple clouds (AWS, Azure, On-prem)
- No visibility into dependencies

**Problems:**
- "Which services use this API?"
- "Who do I contact when service X is down?"
- "What's the health of our systems?"

### The RHDH Solution

**Software Catalog:**
- All 150 services catalogued
- Ownership clearly defined
- Dependency graphs auto-generated

**Real-time Monitoring:**
- Kubernetes plugin shows pod health
- CI/CD status from Tekton
- Security scores from Quay

**API Discovery:**
- OpenAPI specs automatically imported
- Searchable API documentation
- Try APIs directly from portal

**Impact:**
- ⏱️ **75% faster** incident response
- 📉 **50% reduction** in cross-team questions
- 📈 **3x increase** in API reuse

---

## Real-World Use Case #3: Platform Engineering

### Internal Platform Team Challenge

**Goal:** Build Internal Developer Platform (IDP)
**Problem:** How to provide self-service without chaos?

### RHDH as IDP Foundation

**Golden Path Templates:**
```
Templates Available:
├── Backend Services
│   ├── Java Spring Boot API
│   ├── Node.js Express API
│   └── Python FastAPI
├── Frontend Apps
│   ├── React SPA
│   └── Next.js App
├── Data Pipelines
│   ├── Apache Spark Job
│   └── Airflow DAG
└── Infrastructure
    ├── Kubernetes Cluster
    └── Database Instance
```

**Platform Features:**
- ✅ Standardized project structure
- ✅ Built-in security scanning
- ✅ Automated CI/CD setup
- ✅ Infrastructure provisioning
- ✅ Monitoring & alerting

**Results:**
- 🚀 Developers self-serve 90% of needs
- 📊 Platform adoption: 85% of teams
- ⚡ Service creation: 45 mins → 5 mins
- 👥 Platform team focuses on innovation, not tickets

---

## Integration with Red Hat Ecosystem

### Seamless Red Hat Integration

**OpenShift:**
- Topology view
- Pod logs & metrics
- Deployment status
- Resource quotas

**Quay:**
- Container image scanning
- Vulnerability reports
- Image tags & history

**Tekton:**
- Pipeline runs
- Build status
- Logs & artifacts

**Ansible:**
- Automation jobs
- Playbook execution
- Inventory management

**Red Hat SSO:**
- RBAC integration
- Team permissions
- Audit logging

---

## Demo: Creating a Service in 5 Minutes

### Live Walkthrough

**Step 1: Browse Catalog** (30 sec)
- Navigate to software catalog
- Explore existing services
- View dependencies

**Step 2: Choose Template** (30 sec)
- Go to "Create Component"
- Select "Quarkus Microservice" template

**Step 3: Fill Details** (1 min)
- Service name: `customer-api`
- Owner: `platform-team`
- Repository: `github.com/acme/customer-api`

**Step 4: RHDH Magic** (2 min)
- Creates GitHub repository
- Scaffolds Quarkus project
- Sets up Tekton pipeline
- Creates Kubernetes manifests
- Registers in catalog

**Step 5: Verify** (1 min)
- View new service in catalog
- Check CI/CD pipeline running
- See documentation generated

---

## Best Practices for RHDH Adoption

### 1. Start Small, Think Big

- Begin with 1-2 teams as pilot
- Gather feedback early
- Iterate on templates

### 2. Establish Governance

- Define catalog naming conventions
- Set ownership requirements
- Create template approval process

### 3. Integrate Gradually

- Don't try to integrate everything at once
- Focus on highest-impact integrations first
- Prioritize: Git → CI/CD → Cloud → Monitoring

### 4. Foster Community

- Create inner source culture
- Share templates across teams
- Regular feedback sessions

### 5. Measure Success

**Key Metrics:**
- Time to first commit (new developers)
- Service creation time
- Number of self-service actions
- Developer satisfaction scores

---

## Getting Started with RHDH

### Installation Options

**1. OpenShift (Recommended)**
```bash
# Install RHDH Operator
oc apply -f rhdh-operator.yaml

# Create RHDH instance
oc apply -f rhdh-instance.yaml
```

**2. Kubernetes**
```bash
helm repo add redhat-developer https://redhat-developer.github.io/rhdh-chart
helm install rhdh redhat-developer/developer-hub
```

**3. Docker Compose (Development)**
```bash
git clone https://github.com/redhat-developer/rhdh
cd rhdh
docker-compose up
```

### Quick Start Checklist

- ✅ Set up authentication (OAuth/OIDC)
- ✅ Connect to Git provider (GitHub/GitLab)
- ✅ Import first repository
- ✅ Create first template
- ✅ Add 1-2 plugins
- ✅ Invite team for testing

---

## Resources & Community

### Official Resources

- 🌐 **Website:** https://developers.redhat.com/rhdh
- 📘 **Documentation:** https://docs.redhat.com/documentation/en-us/red_hat_developer_hub
- 💻 **GitHub:** https://github.com/redhat-developer/rhdh
- 📦 **Plugin Hub:** https://developers.redhat.com/rhdh/plugins

### Community

- 💬 **Slack:** #rhdh channel
- 🎥 **YouTube:** Red Hat Developer Hub playlist
- 📝 **Blog:** developers.redhat.com/blog
- 🎓 **Training:** Available on Red Hat Learning

### Backstage Community

- CNCF Backstage: https://backstage.io
- 100+ community plugins
- Weekly community calls

---

## Summary: Why RHDH?

### For Developers

- ✅ Single portal for everything
- ✅ Self-service infrastructure
- ✅ Faster onboarding
- ✅ Less context switching
- ✅ Better collaboration

### For Platform Teams

- ✅ Standardized golden paths
- ✅ Reduced support tickets
- ✅ Better visibility
- ✅ Faster innovation
- ✅ Extensible platform

### For Organizations

- ✅ Increased productivity (30-40%)
- ✅ Faster time to market
- ✅ Better developer experience
- ✅ Reduced operational costs
- ✅ Improved compliance & security

---

## Key Takeaways

1. **Developer Portals are the future of Platform Engineering**
   - Central hub for developer experience
   - Self-service enables scale

2. **RHDH = Backstage + Enterprise Features**
   - Production-ready
   - Red Hat ecosystem integration
   - Support & security

3. **Start your IDP journey today**
   - Begin with catalog & templates
   - Grow organically
   - Measure impact

4. **Productivity gains are real**
   - 80% faster project setup
   - 50% less context switching
   - 2x faster onboarding

---

## Thank You!

### Let's Connect

**Mitesh Kumar**  
Senior Software Engineer, Red Hat

- 📧 Email: [Your email]
- 💼 LinkedIn: [Your LinkedIn]
- 🐙 GitHub: [Your GitHub]

### Questions?

**Live Demo Available!**

---

## Appendix: Technical Deep Dive

### RHDH Architecture Components

**Frontend (React)**
- Material-UI based
- Plugin architecture
- Responsive design
- Progressive Web App

**Backend (Node.js)**
- Express.js framework
- Plugin system
- Database: PostgreSQL/SQLite
- Cache: Redis (optional)

**Deployment**
- Container-native
- HA configuration supported
- Horizontal scaling
- OpenShift/Kubernetes native

### Plugin Development

**Creating a Custom Plugin:**

```typescript
// packages/app/src/plugins/my-plugin.ts
import { createPlugin, createRoutableExtension } from '@backstage/core-plugin-api';

export const myPlugin = createPlugin({
  id: 'my-plugin',
  routes: {
    root: rootRouteRef,
  },
});

export const MyPluginPage = myPlugin.provide(
  createRoutableExtension({
    name: 'MyPluginPage',
    component: () =>
      import('./components/MyComponent').then(m => m.MyComponent),
    mountPoint: rootRouteRef,
  }),
);
```

### Security Features

- RBAC (Role-Based Access Control)
- OAuth/OIDC integration
- Secret management
- Audit logging
- Network policies
- Container scanning

### Performance Considerations

- Caching strategies
- Database optimization
- API rate limiting
- CDN for static assets
- Lazy loading plugins

---

## Backup Slides: Common Questions

### Q: How does RHDH compare to other IDPs?

**RHDH vs Port:**
- RHDH: Open-source based, self-hosted
- Port: SaaS-only, proprietary

**RHDH vs Humanitec:**
- RHDH: Full developer portal + IDP
- Humanitec: Focus on app deployment

**RHDH vs Custom Solution:**
- RHDH: Ready-made, community-driven
- Custom: High maintenance, reinventing wheel

### Q: What's the learning curve?

- **Developers:** 1-2 hours (just browsing)
- **Template Creators:** 1-2 days
- **Plugin Developers:** 1-2 weeks
- **Platform Admins:** 1 week

### Q: Total Cost of Ownership?

**Self-Hosted:**
- Infrastructure costs: ~$500-2000/month
- Admin time: 0.5-1 FTE
- Red Hat subscription (optional but recommended)

**ROI:**
- Typical payback: 3-6 months
- Based on developer time savings

### Q: Can we migrate from Backstage?

Yes! RHDH is Backstage-compatible:
- Same plugin API
- Same catalog format
- Migration path documented
- Additional enterprise features

---

## Notes for Speaker

### Timing Breakdown

- **Slide 1-2:** 3 mins (Problem statement)
- **Slide 3:** 3 mins (What is Backstage)
- **Slide 4:** 3 mins (What is RHDH + comparison)
- **Slide 5-9:** 7 mins (Key features - ~1.5 min each)
- **Slide 10-12:** 5 mins (Use cases)
- **Slide 13-14:** 4 mins (Demo/Integration)
- **Slide 15-17:** 1 min (Wrap up)

**Total: 26 mins** (1 min buffer is fine)

### Demo Tips

- Have demo environment ready beforehand
- Use simple, relatable example (e.g., "todo-api")
- Show both UI and generated artifacts
- Have backup screenshots if demo fails

### Engagement Points

- Ask: "How many tools do you switch between daily?"
- Poll: "Who has onboarding pain?"
- Share: "What's your biggest productivity blocker?"

### Key Messages to Emphasize

1. RHDH reduces cognitive load
2. Self-service = scale
3. Enterprise-ready out of the box
4. Open source community + Red Hat support

### Potential Questions & Answers

**Q: How much effort to maintain?**
A: Minimal after setup. Dynamic plugins reduce upgrade complexity.

**Q: What if our tools aren't supported?**
A: Custom plugin development is straightforward. Community has 100+ plugins.

**Q: Security concerns with centralized portal?**
A: RBAC, audit logs, no credentials stored. Portal proxies, doesn't store.

**Q: Multi-cloud support?**
A: Yes, plugins available for AWS, Azure, GCP, and hybrid environments.

