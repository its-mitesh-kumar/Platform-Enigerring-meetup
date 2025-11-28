# Enhance Engineering Productivity with Red Hat Developer Hub

**Platform Engineering Meetup Bengaluru - Nov 29, 2025**

**Mitesh Kumar**  
Senior Software Engineer, Red Hat

*Slide 1*

---

## 🎯 Agenda (25 mins)

1. The Developer Productivity Challenge
2. What is Backstage?
3. What is Red Hat Developer Hub?
4. Key Features & Capabilities
5. **Real-World Case Studies with Data**
6. Live Demo
7. Q&A

*Slide 2*

---

## 💥 The Developer Productivity Challenge

### Common Pain Points

- **Context Switching**: Developers switch between 10-15 tools daily
- **Tool Sprawl**: Jira, GitHub, Jenkins, Kubernetes, Grafana, Confluence...
- **Onboarding Friction**: New developers take weeks to become productive
- **Knowledge Silos**: Critical information scattered everywhere
- **Repetitive Tasks**: Manual setup for every new project

### The Cost

- 🐌 Slower time to market
- 🧠 Increased cognitive load
- 😓 Developer burnout
- 📉 Inconsistent practices

*Slide 3*

---

## 🎵 What is Backstage?

### Open-Source Developer Portal Framework

**Created by Spotify** in 2016, open-sourced in 2020  
**CNCF Incubating Project** since 2022

### The Origin Story

**Spotify's Problem:**
- 2,000+ engineers
- 4,000+ microservices
- Exponential complexity
- No single source of truth

**Their Solution:**
Built **Backstage** - a unified developer portal

### Why Backstage?

> "End the chaos. Give developers a single, unified portal."

**Core Principles:**
1. **Centralized Software Catalog** - All services in one place
2. **Standardized Tooling** - Plugin-based architecture
3. **Self-Service Actions** - Templates for creating projects
4. **Extensible Platform** - Build your own features

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

### Adoption

**Companies Using Backstage:**
- Spotify (originator)
- Netflix
- American Airlines
- HP
- Epic Games
- Expedia
- **1,000+ organizations worldwide**

*Slide 4*

---

## 🔴 What is Red Hat Developer Hub?

### Backstage + Enterprise = RHDH

**Red Hat Developer Hub** is Backstage, production-ready!

### The Value Proposition

```
┌─────────────────────────────────────────────────────┐
│       BACKSTAGE (Open Source Framework)              │
│                      +                               │
│   Red Hat Enterprise Features & Support            │
│                      =                               │
│       RED HAT DEVELOPER HUB (Product)               │
└─────────────────────────────────────────────────────┘
```

### What Red Hat Adds

**1. Enterprise-Ready Out of the Box**
- Pre-configured for production
- Hardened security & HA deployment

**2. Dynamic Plugin System**
- Load plugins without rebuilding
- Update independently

**3. Red Hat Ecosystem Integration**
- OpenShift, Tekton, Quay, Ansible
- Red Hat SSO

**4. Enterprise Support**
- Red Hat support team & SLAs
- Regular security updates

**5. AI-Powered with Lightspeed**
- Intelligent code assistance
- Context-aware troubleshooting

*Slide 5*

---

## 🔑 Key Feature #1: Software Catalog

### Your Infrastructure's Google

**What it does:**
- Single source of truth for all software assets
- Components, APIs, Resources, Systems
- Automatic discovery from Git

**Example: Service Entry**
```yaml
apiVersion: backstage.io/v1alpha1
kind: Component
metadata:
  name: payment-service
  description: Handles payment processing
  tags: [java, spring-boot, critical]
spec:
  type: service
  lifecycle: production
  owner: payments-team
  system: e-commerce
```

**Benefits:**
✅ "Who owns this service?"  
✅ "What APIs are available?"  
✅ "What depends on this?"

*Slide 6*

---

## 🔑 Key Feature #2: Software Templates

### Self-Service Project Creation

**Golden Path Templates**

Pre-configured with best practices:
- Repository setup (GitHub/GitLab)
- CI/CD pipelines (Tekton, Jenkins)
- Kubernetes manifests
- Documentation structure
- Security scanning

**Example: Creating a Microservice**

1. Select "Spring Boot Microservice" template
2. Fill in: service name, team, location
3. RHDH creates:
   - ✅ Git repository with structure
   - ✅ Tekton pipeline
   - ✅ K8s deployment manifests
   - ✅ Monitoring dashboards
   - ✅ Documentation site
4. **Developer starts coding in 5 minutes!**

*Slide 7*

---

## 🔑 Key Feature #3: TechDocs

### Documentation as Code

**Docs-like-code approach:**
- Markdown files in your repo
- Auto-generated from MkDocs
- Lives alongside source code
- Version controlled
- Full-text search

```
my-service/
├── src/
├── docs/
│   ├── index.md
│   ├── architecture.md
│   └── api.md
└── mkdocs.yml
```

**Benefits:**
✅ No context switching  
✅ Always up-to-date  
✅ Discoverable via catalog

*Slide 8*

---

## 🔑 Key Feature #4: Enterprise Production Features

### What Makes RHDH Production-Ready

**🔌 Dynamic Plugin System**
- Zero-downtime updates
- Load plugins without rebuilding

**🤖 Lightspeed (AI-Powered Assistance)**
- Intelligent, context-aware help
- Natural language queries: "How do I deploy this?"
- Automated documentation generation
- Intelligent troubleshooting & recommendations

**🔐 RBAC (Role-Based Access Control)**
- Fine-grained permissions
- Team-based access control
- Secure enterprise deployments

**📊 Scorecards & Compliance**
- Track service quality metrics
- Compliance monitoring
- Technical health scoring

**🚀 Quick Starts**
- Step-by-step interactive tutorials
- Guided onboarding within the portal
- Learn-by-doing approach
- Reduces onboarding time by 40%

**🌍 Localization**
- Multi-language support (10+ languages)
- Global team enablement
- Localized UI and content
- Support for diverse development teams

*Slide 9*

---

## 📊 Real-World Case Study #1: Spotify

### How Spotify Measures Backstage ROI

**The Study:**
- Analyzed internal GitHub activity
- Compared frequent vs infrequent Backstage users
- Measured over 6-12 months

### 🎯 The Results

**Frequent Backstage Users at Spotify:**

| Metric | Improvement | Impact |
|--------|-------------|--------|
| **Developer Activity** | **2.3x more** GitHub activity | More productive |
| **Code Changes** | **2x more** code changes | Faster delivery |
| **Cycle Time** | **17% faster** code changes | Quicker releases |
| **Retention** | **5% higher** after 12 months | Less turnover |

**💰 ROI Impact:**
> "This efficiency is equivalent to **saving 3 full-time employees** for a team of 10 developers."

**Source:** [Spotify Backstage Blog](https://backstage.spotify.com/discover/blog/how-spotify-measures-backstage-roi/)

*Slide 10*

---

## 📊 Real-World Case Study #2: Infosys Insurance Client

### Large Insurance Company Transformation

**The Challenge:**
- Multiple silos across development teams
- Inconsistent tooling and processes
- Long onboarding times (weeks)
- No unified developer experience

**The Solution:**
Implemented **Backstage** to provide:
- Aggregated view of tool stacks
- Standardization across teams
- Self-service capabilities

### 🚀 The Results

| Metric | Improvement |
|--------|-------------|
| **Onboarding Time** | **40% reduction** |
| **Developer Productivity** | **25-30% increase** |
| **Time to Market** | **25-30% faster** |
| **Collaboration & Automation** | **25% improvement** |
| **Deployment Frequency** | **35% increase** |
| **Lead Time for Changes** | **20% reduction** |

**Source:** [CNCF Case Study](https://www.cncf.io/case-studies/infosysinsurancecustomer/)

*Slide 11*

---

## 📈 Summary: Proven Impact

### Real Numbers from Real Companies

**Spotify (2,000+ engineers):**
- 2.3x more developer activity
- Saves 3 FTE per 10-person team
- 17% faster cycle times

**Infosys Insurance Client:**
- 40% faster onboarding
- 25-30% productivity increase
- 35% more deployments

**Industry Average:**
- Onboarding: 2 weeks → 2 days
- Service creation: 4 hours → 5 minutes
- Tool switching: 10+ tools → 1 portal
- ROI: **3-6 months payback**

*Slide 12*

---

## 🏗️ Red Hat Developer Hub: Full Architecture

**Built on Backstage Core + Enterprise Features**

```
┌─────────────────────────────────────────────────────────────────┐
│                     RHDH Frontend (React)                        │
│  ┌──────────┐ ┌──────────┐ ┌──────────┐ ┌──────────┐ ┌────────┐│
│  │ Software │ │   Tech   │ │   API    │ │  Create  │ │ Quick  ││
│  │ Catalog  │ │   Docs   │ │ Explorer │ │Component │ │ Starts ││
│  └──────────┘ └──────────┘ └──────────┘ └──────────┘ └────────┘│
│  ┌──────────┐ ┌──────────┐ ┌──────────┐ ┌──────────────────────┐│
│  │   RBAC   │ │Scorecards│ │Kubernetes│ │   Lightspeed AI      ││
│  │   UI     │ │Dashboard │ │ Dashboard│ │   Assistant          ││
│  └──────────┘ └──────────┘ └──────────┘ └──────────────────────┘│
└─────────────────────────────────────────────────────────────────┘
                                  │
┌─────────────────────────────────────────────────────────────────┐
│                   RHDH Backend (Node.js)                         │
│                                                                   │
│  ┌──────────────────────────────────────────────────────────┐   │
│  │           Core Services & Engines                         │   │
│  │  ┌────────┐ ┌────────┐ ┌────────┐ ┌────────┐ ┌────────┐ │   │
│  │  │Catalog │ │Template│ │ Search │ │  Auth  │ │TechDocs│ │   │
│  │  │ Engine │ │ Engine │ │ Engine │ │ (SSO)  │ │Builder │ │   │
│  │  └────────┘ └────────┘ └────────┘ └────────┘ └────────┘ │   │
│  │  ┌────────┐ ┌────────┐ ┌────────┐ ┌──────────────────┐  │   │
│  │  │ RBAC   │ │Scaffold│ │Permiss-│ │   Lightspeed     │  │   │
│  │  │ Engine │ │ Action │ │  ions  │ │   AI Engine      │  │   │
│  │  └────────┘ └────────┘ └────────┘ └──────────────────┘  │   │
│  └──────────────────────────────────────────────────────────┘   │
│                                                                   │
│  ┌──────────────────────────────────────────────────────────┐   │
│  │            Dynamic Plugin System                          │   │
│  │  • Hot-reload plugins without restart                     │   │
│  │  • Independent plugin versioning                          │   │
│  │  • Frontend & Backend plugin support                      │   │
│  └──────────────────────────────────────────────────────────┘   │
└─────────────────────────────────────────────────────────────────┘
                                  │
┌─────────────────────────────────────────────────────────────────┐
│                      Data & Storage Layer                        │
│  ┌────────────┐  ┌────────────┐  ┌────────────┐                │
│  │ PostgreSQL │  │    Cache   │  │   Object   │                │
│  │  Database  │  │   (Redis)  │  │  Storage   │                │
│  │ (Catalog)  │  │            │  │  (S3/Blob) │                │
│  └────────────┘  └────────────┘  └────────────┘                │
└─────────────────────────────────────────────────────────────────┘
                                  │
┌─────────────────────────────────────────────────────────────────┐
│               External Integrations (Plugins)                    │
│                                                                   │
│  Source Control        CI/CD              Container & K8s        │
│  ┌────────┐┌────────┐ ┌────────┐┌──────┐ ┌────────┐┌─────────┐│
│  │ GitHub ││GitLab  │ │ Tekton ││ArgoCD│ │  Quay  ││OpenShift││
│  │        ││Bitbkt  │ │Jenkins ││      │ │ Harbor ││  K8s    ││
│  └────────┘└────────┘ └────────┘└──────┘ └────────┘└─────────┘│
│                                                                   │
│  Monitoring           Security            Automation             │
│  ┌────────┐┌────────┐ ┌────────┐┌──────┐ ┌────────┐┌─────────┐│
│  │Grafana ││Prometheus│SonarQube││Vault │ │ Ansible││Terraform││
│  │Datadog ││          │Snyk     ││      │ │        ││         ││
│  └────────┘└────────┘ └────────┘└──────┘ └────────┘└─────────┘│
│                                                                   │
│  Identity & Comms      Docs & Knowledge   Cloud Providers        │
│  ┌────────┐┌────────┐ ┌────────┐┌──────┐ ┌────────┐┌─────────┐│
│  │Red Hat ││  LDAP  │ │Conflue-││Slack │ │  AWS   ││  Azure  ││
│  │  SSO   ││  SAML  │ │  nce   ││Teams │ │  GCP   ││         ││
│  └────────┘└────────┘ └────────┘└──────┘ └────────┘└─────────┘│
└─────────────────────────────────────────────────────────────────┘
```

**Key Architecture Highlights:**
- **Microservices-based**: Container-native, runs on Kubernetes/OpenShift
- **Plugin-driven**: 100+ plugins available, dynamic loading
- **Scalable**: Horizontal scaling for backend services
- **Secure**: RBAC, SSO integration, audit logging
- **Multi-tenant ready**: Team-based isolation and permissions

*Slide 13*

---

## 🎬 Live Demo: Create a Service in 5 Minutes

### What You'll See

**Step 1:** Browse existing services in catalog (30s)

**Step 2:** Select "Quarkus Microservice" template (30s)

**Step 3:** Fill in basic details (1 min)
- Service name: `customer-rewards-api`
- Owner: `platform-team`
- Repository location

**Step 4:** Watch RHDH create (2 min)
- ✅ GitHub repository
- ✅ Project structure
- ✅ Tekton pipeline
- ✅ Kubernetes manifests
- ✅ Documentation

**Step 5:** Verify the result (1 min)

*Slide 14*

---

## 🚀 Getting Started with RHDH

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
helm repo add redhat-developer \
  https://redhat-developer.github.io/rhdh-chart
helm install rhdh redhat-developer/developer-hub
```

**3. Try Online Demo**
Visit: https://developers.redhat.com/rhdh

*Slide 15*

---

## 🎁 Key Takeaways

### For Developers
✅ Single portal for everything  
✅ Self-service infrastructure  
✅ Faster onboarding (2 weeks → 2 days)  
✅ Less context switching  

### For Platform Teams
✅ Standardized golden paths  
✅ 70% reduction in support tickets  
✅ Better visibility across services  
✅ Extensible platform  

### For Organizations
✅ **25-30% increase in productivity** (proven)  
✅ **40% faster onboarding** (real data)  
✅ **35% more deployments** (measurable)  
✅ **3-6 months ROI** (typical)  
✅ Improved developer retention (+5%)  

*Slide 16*

---

## 📚 Resources & Links

### Official Resources

- 🌐 **Website:** https://developers.redhat.com/rhdh
- 📘 **Documentation:** https://docs.redhat.com/documentation/en-us/red_hat_developer_hub
- 💻 **GitHub:** https://github.com/redhat-developer/rhdh
- 🎥 **Demos:** https://developers.redhat.com/products/rhdh/demos

### Case Studies & Data

- 📊 **Spotify ROI Study:** https://backstage.spotify.com/discover/blog/how-spotify-measures-backstage-roi/
- 📈 **Infosys Case Study:** https://www.cncf.io/case-studies/infosysinsurancecustomer/
- 🤖 **Red Hat AI Tools:** https://www.itpro.com/software/development/red-hat-eyes-developer-workflow-efficiency-app-modernization-gains-with-new-ai-tools

### Community

- 💬 **Backstage Community:** https://backstage.io
- 🎓 **Red Hat Learning:** https://developers.redhat.com/learn

*Slide 17*

---

## 🙏 Thank You!

### Let's Connect

**Mitesh Kumar**  
Senior Software Engineer, Red Hat

- 📧 Email: mitesh@redhat.com
- 💼 LinkedIn: [Your LinkedIn]
- 🐙 GitHub: [Your GitHub]

### Questions?

**Try RHDH Today:**  
👉 https://developers.redhat.com/rhdh

*Slide 18*

---

## 🎯 Call to Action

### Next Steps

**For Attendees:**
1. 🔗 Try the RHDH online demo
2. 📖 Read the case studies
3. 💬 Join the community

**For Platform Teams:**
1. 🧪 Run a pilot with 1-2 teams
2. 📊 Measure time-to-first-commit
3. 📈 Track developer satisfaction
4. 🎉 Share results with leadership

**Start Your Developer Portal Journey Today!**

*Slide 19*

---

# Questions?

*Slide 20*

---

# Backup Slides

*Slide 21*

---

## RHDH vs Competitors

| Feature | RHDH | Backstage OSS | Port | Humanitec |
|---------|------|---------------|------|-----------|
| **Open Source** | ✅ | ✅ | ❌ | ❌ |
| **Self-Hosted** | ✅ | ✅ | ❌ | ✅ |
| **Enterprise Support** | ✅ | ❌ | ✅ | ✅ |
| **Dynamic Plugins** | ✅ | ❌ | N/A | N/A |
| **Setup Time** | Hours | Days/Weeks | Minutes | Hours |
| **AI Assistance** | ✅ Lightspeed | ❌ | Varies | Varies |

*Slide 22*

---

## Total Cost of Ownership

**Self-Hosted RHDH:**
- Infrastructure: $500-2,000/month
- Admin time: 0.5-1 FTE
- Red Hat subscription: Contact sales

**ROI:**
- Typical payback: **3-6 months**
- Based on developer time savings
- Reduced support burden
- Faster time to market

**Example:**
- Team of 50 developers
- 30% productivity gain = 15 FTE worth
- Annual value: $3-5M (at $200K/dev)
- Investment: $100-200K
- **ROI: 15-25x**

*Slide 23*

---

## Technical Deep Dive

### Component Types

- **Service:** Backend services, APIs
- **Website:** Frontend applications
- **Library:** Shared code libraries
- **Resource:** Databases, queues, storage
- **API:** OpenAPI/GraphQL specs
- **System:** Collection of components
- **Domain:** Business domain grouping

### Relations

- **ownerOf:** Team owns component
- **dependsOn:** Component depends on another
- **providesApi:** Component provides API
- **consumesApi:** Component consumes API
- **partOf:** Component part of system

*Slide 24*

---

