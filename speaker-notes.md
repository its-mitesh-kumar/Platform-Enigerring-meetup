# Speaker Notes: Enhance Engineering Productivity with Red Hat Developer Hub
## Platform Engineering Meetup Bengaluru - Nov 29, 2025

**Duration:** 25 minutes  
**Format:** Talk (20 min) + Demo (4 min) + Q&A (1 min)

---

## Pre-Presentation Checklist (5 minutes before)

- [ ] Demo environment tested and accessible
- [ ] Browser tabs open (RHDH, GitHub, backup screenshots)
- [ ] Microphone and audio tested
- [ ] Presentation mode enabled (hide bookmarks/toolbar)
- [ ] Zoom set to 125% for visibility
- [ ] Water bottle ready
- [ ] Clicker/keyboard shortcuts tested
- [ ] Deep breath and smile!

---

## Opening (Before Slide 1) - 30 seconds

**What to Say:**

> "Good morning everyone! Before we start, quick question - show of hands: How many different tools do you switch between on a typical workday? GitHub, Jira, Jenkins, Kubernetes dashboard, Grafana, Confluence... anyone using 10 or more?"

**Why:** Immediately engage audience and make the problem relatable.

**Expected Response:** Most hands will go up - acknowledge this with "That's what I thought. That's the problem we're solving today."

---

## Slide 1: Title Slide - 30 seconds

### What's On Screen:
- Title: "Enhance Engineering Productivity with Red Hat Developer Hub"
- Your name and title
- Date and event

### What to Say:

> "Good morning! I'm Mitesh Kumar, Senior Software Engineer at Red Hat. Today, I'm going to show you how Red Hat Developer Hub can dramatically improve your developer productivity - and I'm not talking about theoretical improvements. I have real data from companies like Spotify and Infosys showing 2-3x productivity gains."

> "This is the last Platform Engineering meetup of 2025, so let's make it count!"

### Key Points:
- Introduce yourself warmly
- Set expectation: this is practical, data-driven
- Show enthusiasm - this is exciting technology!

### Body Language:
- Stand confidently, shoulders back
- Make eye contact with different sections of room
- Smile - you're excited to share this

**Transition:** "Let me show you the agenda for the next 25 minutes."

---

## Slide 2: Agenda - 30 seconds

### What's On Screen:
1. The Developer Productivity Challenge
2. What is Backstage?
3. What is Red Hat Developer Hub?
4. Key Features & Capabilities
5. Real-World Case Studies with Data
6. Live Demo
7. Q&A

### What to Say:

> "Here's what we'll cover: First, I'll paint the problem - the productivity challenges developers face today. Then I'll introduce Backstage, the open-source foundation. After that, Red Hat Developer Hub and what makes it enterprise-ready. We'll dive into key features including the software catalog, templates, documentation, and enterprise production features like Quick Starts, Lightspeed AI, and Localization. But most importantly - I'll share real case studies with actual numbers. Then a quick live demo, and we'll wrap with Q&A."

> "I know 25 minutes is tight, so I'll keep it focused. Hold your questions until the end, but feel free to catch me afterward for deeper discussions."

### Key Points:
- Set clear expectations
- Emphasize the data-driven approach
- Acknowledge time constraints

**Transition:** "So, what's the problem we're solving?"

---

## Slide 3: The Developer Productivity Challenge - 2 minutes

### What's On Screen:
- Common Pain Points (5 bullets)
- The Cost (4 bullets)

### What to Say:

> "Let's talk about the elephant in the room. Modern developers are drowning in complexity."

**Point to first bullet:**

> "**Context switching.** Developers spend 30-40% of their day just navigating between tools. Think about it - you're coding in VS Code, you switch to GitHub for PRs, then Jira for tickets, then Jenkins for builds, then Kubernetes dashboard for deployments, then Grafana for metrics, then Confluence for docs. Each switch takes mental energy."

**Point to second bullet:**

> "**Tool sprawl.** The average organization uses 10-15 different tools in the development lifecycle. Each has its own login, its own UI, its own way of doing things. It's exhausting."

**Point to third bullet:**

> "**Onboarding friction.** Raise your hand if onboarding a new developer in your organization takes more than a week? [pause for hands] Exactly. New developers spend weeks just figuring out where things are and how things work."

**Point to fourth bullet:**

> "**Knowledge silos.** Critical information is scattered - some in Confluence, some in Slack, some in someone's head, some in README files that haven't been updated in two years."

**Point to fifth bullet:**

> "**Repetitive tasks.** Every time someone creates a new service, they manually set up the repo, configure CI/CD, write Kubernetes manifests, set up monitoring. It's the same thing over and over, but slightly different every time."

**Move to 'The Cost' section:**

> "What's the cost of all this? Slower time to market - obviously. But also increased cognitive load, which leads to burnout. And because everyone does things slightly differently, you get inconsistent practices across teams, which creates more problems down the line."

### Key Points:
- Make it personal and relatable
- Use pauses for emphasis
- Watch for nodding heads - this validates the problem

### Body Language:
- Use hands to show "switching" motion (chaos)
- Show frustration when talking about pain points
- Make eye contact - "you know this problem"

**Transition:** "So how do we solve this? Let me introduce you to Backstage."

---

## Slide 4: What is Backstage? - 3.5 minutes

### What's On Screen:
- Title, origin story, why Backstage, architecture diagram, adoption stats

### What to Say:

**Part 1: Introduction (30 seconds)**

> "Backstage is an open-source developer portal framework. But that doesn't tell you much. Let me tell you the story behind it."

**Part 2: Origin Story (1 minute)**

> "Backstage was created by Spotify back in 2016. Picture this: Spotify had 2,000 engineers working on 4,000 microservices. The complexity was exponential. Engineers were spending more time navigating the infrastructure than building features. They had no single source of truth - information was everywhere and nowhere."

> "So they built Backstage - an internal developer portal that unified everything. It worked so well that in 2020, they open-sourced it. In 2022, it became a CNCF Incubating Project. That's a big deal - it means the Cloud Native Computing Foundation, the folks behind Kubernetes, recognized Backstage as a critical piece of modern infrastructure."

**Part 3: Why Backstage? (45 seconds)**

> "The vision is simple but powerful: [read quote] 'End the chaos of different tools, documentation, and processes. Give developers a single, unified portal.'"

> "It's built on four core principles:"

**Point to each:**
1. "**Centralized Software Catalog** - Think of it as Google for your internal services. Everything in one searchable place."
2. "**Standardized Tooling** - Plugin-based architecture so you can integrate with anything."
3. "**Self-Service Actions** - Developers can create new projects from templates without waiting for platform teams."
4. "**Extensible Platform** - Build your own features and workflows on top."

**Part 3.5: Backstage Architecture (45 seconds)**

> "[Point to architecture diagram] Let me show you how Backstage is structured. At its core, Backstage has three foundational features:"

> "[Point to Software Catalog] **Software Catalog** - for service discovery, metadata management, and ownership tracking."

> "[Point to Software Templates] **Software Templates** - for scaffolding new projects, automation, and enforcing best practices."

> "[Point to TechDocs] **TechDocs** - for documentation as code, search, and using MkDocs."

> "[Point to Plugin Ecosystem] And underneath, a rich plugin ecosystem with over 100 plugins - GitHub, Jenkins, Kubernetes, Prometheus, and many more. This is what makes Backstage so powerful and extensible."

**Part 4: Adoption (45 seconds)**

> "And this isn't some obscure tool. Over 1,000 organizations use Backstage today. Spotify obviously, but also Netflix, American Airlines, HP, Epic Games, Expedia. These are serious engineering organizations."

> "Why so popular? It's open source with Apache 2.0 license - no vendor lock-in. It's battle-tested at scale - Spotify runs it for 2,000+ engineers. It has an active community with 100+ contributors. And it's cloud-agnostic - works anywhere."

**Part 5: The Challenge (transition to next slide)**

> "So you've seen the core Backstage architecture - catalog, templates, docs, plugins. Powerful foundation, right?"

> "But here's the thing - Backstage is a *framework*, not a *product*. These three core features are building blocks. You still need to set it up, configure it, add security, make it production-ready, maintain it. Typical setup time is 2-4 weeks, and you need dedicated resources to keep it running."

> "This is where Red Hat Developer Hub comes in - taking this powerful foundation and making it enterprise-ready."

### Key Points:
- Make Backstage credible (Spotify, CNCF, adoption)
- Explain the problem it solves
- Set up the need for RHDH

### Body Language:
- Show scale with hand gestures (2,000 engineers, 4,000 services)
- Look excited when talking about adoption
- Show slight concern when discussing "the challenge"

**Transition:** "So what is Red Hat Developer Hub?"

---

## Slide 5: What is Red Hat Developer Hub? - 3 minutes

### What's On Screen:
- Title, value proposition diagram, what Red Hat adds

### What to Say:

**Part 1: Core Message (30 seconds)**

> "Red Hat Developer Hub, or RHDH, is Backstage - but enterprise-ready. Think of it this way: [point to diagram] Backstage is a powerful framework that requires significant setup. RHDH is a production-ready product that works out of the box."

> "It's Backstage plus Enterprise equals RHDH."

**Part 2: What Red Hat Adds (2 minutes)**

> "So what does Red Hat add? Five major things:"

**Point to each:**

**1. Enterprise-Ready Out of the Box (20s)**

> "First, it's pre-configured for production use. Security hardening, high-availability deployment configs, performance optimizations - all done for you. You're not starting from scratch."

**2. Dynamic Plugin System (20s)**

> "Second, dynamic plugins. This is huge. With regular Backstage, every time you want to add a plugin, you rebuild the entire application. With RHDH, you can load plugins dynamically, update them independently, without any downtime. No need to fork Backstage and maintain your own version."

**3. Red Hat Ecosystem Integration (25s)**

> "Third, deep integration with the Red Hat ecosystem. If you're using OpenShift - our Kubernetes platform - you get native integration. Tekton for cloud-native CI/CD, Quay for container registry, Ansible for automation, Red Hat SSO for identity management. It all just works together."

**4. Enterprise Support (20s)**

> "Fourth, enterprise support. You get the Red Hat support team, SLA guarantees, regular security updates, migration assistance. This isn't community support - this is enterprise-grade support with accountability."

**5. Pre-Built Templates & Plugins and AI (25s)**

> "And fifth, pre-built templates and plugins based on Red Hat's best practices. Plus, and this is new - Red Hat Developer Lightspeed, which is AI-powered assistance built right into the portal. Context-aware help, intelligent troubleshooting, code generation."

**Part 3: Core Philosophy (20s)**

> "The core philosophy is: 'Shift complexity left, but make it invisible.' We want developers to have power and control, but we don't want them to be overwhelmed. Single pane of glass, self-service, golden paths without feeling like guardrails."

### Key Points:
- Clearly differentiate RHDH from Backstage
- Emphasize enterprise readiness
- Make the value proposition crystal clear

### Body Language:
- Count on fingers for the five additions
- Show confidence - this is valuable
- Use "we" when talking about Red Hat (you're part of it)

**Transition:** "Now let me show you what RHDH can actually do. Let's look at the key features."

---

## Slide 6: Key Feature #1: Software Catalog - 1.5 minutes

### What's On Screen:
- Description, YAML example, benefits

### What to Say:

**Part 1: Introduction (20s)**

> "The first killer feature is the Software Catalog. Think of it as Google for your internal services. It's a centralized, searchable directory of all your software assets."

**Part 2: What It Does (30s)**

> "Every component, API, resource, system, domain - everything is catalogued. The catalog automatically discovers services from your Git repositories. You just add a small YAML file to your repo, and RHDH picks it up."

**Part 3: Example (25s)**

> "[Point to YAML] Here's what that looks like. This is a catalog entry for a payment service. It tells you: it's written in Java with Spring Boot, it's critical infrastructure, it's owned by the payments team, it's part of the e-commerce system. All this metadata makes everything discoverable."

**Part 4: Benefits (15s)**

> "Now instead of asking 'Who owns this service?' in Slack and waiting for someone to respond, you just look it up. What APIs are available? Look it up. What depends on this service? Look it up. It's all right there."

### Key Points:
- Make catalog sound simple but powerful
- Emphasize the "no more asking in Slack" benefit
- Set up for templates (next slide)

**Transition:** "But RHDH doesn't just help you find things. It helps you create things."

---

## Slide 7: Key Feature #2: Software Templates - 2 minutes

### What's On Screen:
- Description, example workflow, impact metrics

### What to Say:

**Part 1: Introduction (20s)**

> "The second killer feature is Software Templates. This is self-service project creation with best practices baked in. We call them Golden Path templates."

**Part 2: What's Included (30s)**

> "Each template is pre-configured with everything you need: repository setup on GitHub or GitLab, CI/CD pipelines using Tekton or Jenkins or GitHub Actions, infrastructure as code with Kubernetes manifests or Helm charts, documentation structure, security scanning - everything."

**Part 3: Example Workflow (50s)**

> "Let me walk you through an example. A developer wants to create a new microservice. They go to RHDH, select the 'Spring Boot Microservice' template. They fill in a simple form: service name, their team, where they want the repository. That's it."

> "Then RHDH does the heavy lifting: It creates a Git repository with the complete code structure. It sets up a Tekton pipeline for CI/CD. It generates Kubernetes deployment manifests. It creates monitoring dashboards. It sets up a documentation site. All of this happens automatically."

> "Five minutes later, the developer is writing business logic. Not configuring YAML. Not googling 'how to set up Jenkins pipeline.' Writing actual code."

**Part 4: Impact (20s)**

> "The impact? [Point to metrics] 80% faster project bootstrapping. Consistent practices across all teams - no more 'everyone does it differently.' And security by default - best practices are built in, not added as an afterthought."

### Key Points:
- Emphasize time savings
- Make it sound easy
- Show consistency benefits

### Body Language:
- Show timeline with hands (before: hours, after: minutes)
- Show relief/ease when talking about developer experience

**Transition:** "Now, templates create code. But what about documentation?"

---

## Slide 8: Key Feature #3: TechDocs - 1 minute

### What's On Screen:
- Description, folder structure example, benefits

### What to Say:

**Part 1: Introduction (20s)**

> "Third feature: TechDocs. This is documentation as code. Docs live right in your repository, alongside your source code. They're written in Markdown, auto-generated from MkDocs, version-controlled."

**Part 2: How It Works (25s)**

> "[Point to folder structure] You just create a docs folder in your repo, add Markdown files, add an mkdocs.yml config. RHDH automatically publishes these as beautiful, searchable documentation. When you update your code and documentation together, they stay in sync."

**Part 3: Benefits (15s)**

> "The benefits? No context switching - docs are right there in the catalog. Always up-to-date because they're version-controlled with code. Discoverable via full-text search. Documentation becomes a first-class citizen, not an afterthought."

### Key Points:
- Keep this brief - it's straightforward
- Emphasize "always up-to-date"
- Set up for enterprise features

**Transition:** "Now, those are the foundational features. But what makes RHDH truly enterprise-ready are the production features."

---

## Slide 9: Key Feature #4: Enterprise Production Features - 2.5 minutes

### What's On Screen:
- Six major features: Quick Starts, Lightspeed AI, Localization, RBAC, Scorecards, Dynamic Plugins

### What to Say:

**Part 1: Introduction (15s)**

> "This slide is packed with the enterprise features that make RHDH production-ready for global organizations. These are the differentiators. Let me walk through each one."

**Part 2: Quick Starts (25s)**

> "[Point] First, Quick Starts. These are guided, interactive tutorials right inside the portal. Instead of reading 50-page documentation, developers get step-by-step, hands-on learning. 'Create your first microservice,' 'Deploy to OpenShift,' 'Set up CI/CD' - all interactive. The result? 40% reduction in onboarding time. New developers become productive in days, not weeks."

**Part 3: Lightspeed AI (30s)**

> "[Point] Second, Red Hat Developer Lightspeed - AI-powered assistance. This isn't generic ChatGPT - it's context-aware AI that understands YOUR organization. Ask 'How do I deploy this service?' and it gives you the actual steps based on YOUR infrastructure. It generates documentation, provides intelligent troubleshooting, recommends code improvements - all context-aware."

**Part 4: Localization (20s)**

> "[Point] Third, localization with support for 10+ languages. If you have global development teams in India, Europe, Asia, Latin America - everyone can use RHDH in their preferred language. The UI, content, documentation - all localized. This is crucial for global enterprises."

**Part 5: RBAC (20s)**

> "[Point] Fourth, Role-Based Access Control. Fine-grained permissions, team-based access control. You control who can view what, who can create templates, who can deploy to production. Enterprise security built in."

**Part 6: Scorecards (15s)**

> "[Point] Fifth, Scorecards and Compliance. Track service quality metrics, monitor compliance, technical health scoring. See at a glance which services meet your standards and which need attention."

**Part 7: Dynamic Plugins (15s)**

> "[Point] And sixth, the dynamic plugin system. Load and update plugins without rebuilding RHDH. Zero downtime updates. With regular Backstage, every plugin change requires a full rebuild. With RHDH, just load it dynamically."

### Key Points:
- Cover all six features efficiently
- Emphasize Quick Starts, Lightspeed, and Localization (the requested highlights)
- Show enterprise value
- Don't rush but be concise

### Body Language:
- Point to each section as you discuss
- Show excitement about Quick Starts and AI
- Maintain confidence about enterprise features
- Use counting gestures (six features)

**Transition:** "These enterprise features sound great, but do they actually deliver results? Let me show you real data from real companies."

---

## Slide 10: Real-World Case Study #1: Spotify - 2 minutes

### What's On Screen:
- The study description, results table, ROI impact quote

### What to Say:

**Part 1: Setup (20s)**

> "Remember Spotify, the company that created Backstage? They didn't just build it and hope it worked. They measured it. They analyzed their internal GitHub activity and compared developers who frequently used Backstage versus those who didn't."

**Part 2: The Results (1 minute)**

> "Here's what they found: [Point to table]"

> "**Developer Activity:** Frequent Backstage users had 2.3 times - more than double - more activity in GitHub compared to infrequent users."

> "**Code Changes:** They created twice as many code changes. Not just small tweaks - actual feature development."

> "**Cycle Time:** They completed code changes 17% faster. From commit to merge, the cycle was quicker."

> "**Retention:** And here's one you might not expect - 5% higher retention rate after 12 months. Developers who use Backstage are less likely to leave Spotify."

**Part 3: ROI Impact (30s)**

> "[Read quote] 'This efficiency is equivalent to saving 3 full-time employees for a team of 10 developers.'"

> "Think about that. For a team of 10, you get the productivity of 13. That's a 30% productivity gain. And this isn't projected or estimated - this is measured data from Spotify's internal systems."

**Part 4: Source (10s)**

> "I'm not making this up. The link is right there - Spotify published this on their Backstage blog. You can read the full methodology."

### Key Points:
- This is the most important slide - emphasize real data
- Speak slowly and let numbers sink in
- Make eye contact to gauge reactions

### Body Language:
- Point to each metric as you discuss it
- Show excitement - these are impressive numbers
- Pause after the 3 FTE quote

**Transition:** "And Spotify isn't alone. Let me show you another case study."

---

## Slide 11: Real-World Case Study #2: Infosys Insurance Client - 2 minutes

### What's On Screen:
- Challenge, solution, results table

### What to Say:

**Part 1: Context (30s)**

> "This is a case study published by the CNCF - the Cloud Native Computing Foundation. It's about a large insurance company that worked with Infosys to implement Backstage."

> "Their challenge: multiple development silos, inconsistent tooling, long onboarding times taking weeks, no unified developer experience. Sound familiar?"

**Part 2: The Solution (20s)**

> "They implemented Backstage to provide an aggregated view of all their tool stacks, standardization across teams, and self-service capabilities so developers weren't blocked waiting for other teams."

**Part 3: The Results (1 minute)**

> "Now here's where it gets interesting. [Point to table]"

> "**Onboarding time:** 40% reduction. New developers productive much faster."

> "**Developer productivity:** 25-30% increase. That's huge. For every four developers, you get the output of five."

> "**Time to market:** Products reaching the market 25-30% faster. That's competitive advantage."

> "**Collaboration and automation:** 25% improvement in teams working together and automating toil."

> "**Deployment frequency:** 35% increase. They're shipping more often."

> "**Lead time for changes:** 20% reduction. From idea to production, faster."

**Part 4: Emphasis (10s)**

> "These aren't small improvements. These are transformative. And again, this is real data from a real company, published by CNCF."

### Key Points:
- Make this feel real (large insurance company)
- Each metric is impressive - give them weight
- Connect to business outcomes (competitive advantage)

### Body Language:
- Point to each metric
- Show impact with hand gestures (up = good)
- Maintain strong eye contact

**Transition:** "Let's summarize what we've learned from these real-world examples."

---

## Slide 12: Summary: Proven Impact - 1.5 minutes

### What's On Screen:
- Three sections: Spotify, Infosys, Industry Average

### What to Say:

**Part 1: Introduction (15s)**

> "So let's put it all together. We're not talking about hypothetical improvements. We're talking about real numbers from real companies."

**Part 2: Spotify (20s)**

> "[Point] Spotify with 2,000+ engineers: 2.3 times more developer activity. That efficiency saves 3 full-time employees per 10-person team. Cycle times 17% faster."

**Part 3: Infosys Client (20s)**

> "[Point] Infosys insurance client: 40% faster onboarding, 25-30% productivity increase, 35% more deployments. These are business-changing numbers."

**Part 4: Industry Average (35s)**

> "[Point] And across the industry, we're seeing patterns: Onboarding time dropping from 2 weeks to 2 days. Service creation from 4 hours to 5 minutes - that's a 98% reduction. Tool switching from 10+ tools to 1 portal. And ROI - return on investment - typically in 3 to 6 months."

> "So if you're thinking 'this sounds expensive' - it pays for itself in less than a year, and then keeps delivering value."

### Key Points:
- Reinforce the data
- Make ROI clear
- Build momentum toward demo

### Body Language:
- Point to each section as you discuss
- Show confidence in the numbers
- Build energy for the demo

**Transition:** "Alright, enough slides. Let me show you this in action."

---

## Slide 13: Architecture Overview - 45 seconds

### What's On Screen:
- Comprehensive five-layer architecture diagram with components

### What to Say:

**Quick walkthrough (45s):**

> "Before the demo, let me show you the full RHDH architecture. Remember Backstage's three core features we saw earlier - catalog, templates, TechDocs? This is how RHDH builds on that foundation and makes it enterprise-ready."

> "[Point to Frontend] At the top, you have the React frontend - the catalog browser, TechDocs, API explorer we discussed, plus Quick Starts for onboarding, Lightspeed AI assistant, RBAC controls, scorecards - all in one unified UI."

> "[Point to Backend] The Node.js backend has core engines: catalog engine, template scaffolder, search, authentication with SSO, TechDocs builder, RBAC engine, and the Lightspeed AI engine. Notice the dynamic plugin system - you can hot-reload plugins without restarting."

> "[Point to Data Layer] PostgreSQL for the catalog data, Redis for caching, object storage for TechDocs and artifacts."

> "[Point to Integrations] And here's the power - extensive plugin ecosystem. Source control like GitHub and GitLab, CI/CD with Tekton and ArgoCD, container registries, Kubernetes, monitoring with Grafana, security tools, Ansible, cloud providers - all integrated."

> "It's container-native, runs on Kubernetes or OpenShift, horizontally scalable, and production-ready."

### Key Points:
- Don't get lost in details - keep moving
- Emphasize the plugin ecosystem (extensibility)
- Highlight dynamic plugins and scalability
- Establish technical credibility

### Body Language:
- Point to each layer as you discuss
- Move quickly but confidently
- Show the breadth with hand gestures

**Transition:** "Now let me show you how this works in practice."

---

## Slide 14: Live Demo: Create a Service in 5 Minutes - 4 minutes

### What's On Screen:
- Demo steps listed

### What to Say:

**Part 1: Introduction (15s)**

> "I'm going to create a complete microservice from scratch. Watch the timer - this will take about 5 minutes, including repository creation, CI/CD setup, Kubernetes manifests, documentation, everything."

**Part 2: Execute Demo (3 min 45s)**

**Step 1: Browse Catalog (30s)**

> "Let me start by showing you existing services. [Navigate to catalog] Here's our software catalog. I can filter by owner, by tag, by type. [Click on a service] Here's one of our existing services - you can see the overview, the relations showing what it depends on, CI/CD status from Kubernetes, documentation."

**Step 2: Create Component (20s)**

> "Now let's create something new. [Click Create] Here are our available templates - Spring Boot, Quarkus, Node.js, React, Python. I'll choose Quarkus Microservice."

**Step 3: Fill Form (40s)**

> "[Start filling] Service name: customer-rewards-api. Description: API for managing customer loyalty points. Owner: platform-team. System: loyalty-program. Repository organization: acme-corp. Repository name: customer-rewards-api."

> "Notice I'm not configuring CI/CD, not writing Kubernetes YAML, not setting up monitoring. Just business information."

**Step 4: Review and Create (20s)**

> "[Click Review] Here's a summary of what will be created. Looks good. [Click Create]"

> "And now watch. RHDH is doing all the work."

**Step 5: Watch Progress (1 minute)**

> "[Point to progress indicators as they complete] Creating GitHub repository... done. Scaffolding project structure... done. Creating Tekton pipeline... done. Generating Kubernetes manifests... done. Setting up monitoring... done. Creating documentation site... done. Registering in catalog... done."

> "All of that just happened automatically."

**Step 6: Verify (45s)**

> "[Navigate to catalog] Here's our new service in the catalog. [Show overview] Already registered. [Show relations] Already part of our system architecture. [Click CI/CD tab] Pipeline is already running. [Click Docs tab] Documentation already published."

> "[Switch to GitHub tab] And here's the GitHub repository - complete project structure, all the code, CI/CD configs, everything."

**Part 3: Wrap Up (15s)**

> "Five minutes. From zero to a fully functional service with CI/CD, documentation, monitoring. Our developer can now focus on writing business logic, not infrastructure."

### Key Points:
- Stay calm if demo has issues (use screenshots)
- Keep energy high
- Emphasize time savings

### Demo Failure Plan:
If demo fails:
> "And this is why we have backup plans! Let me show you screenshots of this working. [Switch to screenshots] The demo gods aren't with us today, but the concept is the same..."

Then walk through screenshots with same narrative.

**Transition:** "So that's the demo - 5 minutes from zero to a fully functional service. Now let me show you how to get started."

---

## Slide 14: Getting Started with RHDH - 45 seconds

### What's On Screen:
- Three installation options

### What to Say:

> "Getting started is straightforward. You have three options:"

> "**Option 1:** If you're on OpenShift, which I recommend, you install the RHDH operator, create an instance. Two commands, you're done."

> "**Option 2:** If you're on vanilla Kubernetes, we have a Helm chart. Helm repo add, helm install, done."

> "**Option 3:** If you just want to try it out, there's an online demo at developers.redhat.com/rhdh. No installation required, you can explore immediately."

> "I'd recommend starting with option 3 - try the demo, see if it fits your needs, then do a pilot installation."

### Key Points:
- Make it sound easy
- Give clear next step (try demo)

**Transition:** "Let me wrap up with key takeaways."

---

## Slide 15: Key Takeaways - 1.5 minutes

### What's On Screen:
- Three sections: For Developers, For Platform Teams, For Organizations

### What to Say:

**Introduction (10s):**

> "Let me give you takeaways based on who you are."

**For Developers (25s):**

> "If you're a developer: Single portal for everything - no more context switching. Self-service infrastructure - no waiting on tickets. Onboarding drops from 2 weeks to 2 days - productive immediately. Less time navigating tools, more time writing code."

**For Platform Teams (25s):**

> "If you're on a platform team: Standardized golden paths mean consistent quality. 70% reduction in support tickets - developers self-serve. Better visibility means faster incident response. And it's an extensible platform - build on it, don't start from scratch."

**For Organizations (40s):**

> "If you're in leadership: These are proven numbers. 25-30% increase in productivity - that's not marginal, that's transformative. 40% faster onboarding - new hires productive in days, not weeks. 35% more deployments - faster time to market. ROI typically in 3-6 months - it pays for itself quickly. And 5% improvement in developer retention - developers are happier, they stay."

**Closing (10s):**

> "Developer portals aren't the future - they're the present. The companies winning today are the ones that have already adopted this approach."

### Key Points:
- Speak to different audiences
- Come back to the data
- Make it feel urgent (not future, present)

**Transition:** "Here are resources if you want to learn more."

---

## Slide 16: Resources & Links - 45 seconds

### What's On Screen:
- Official resources, case studies, community links

### What to Say:

> "I've packed a lot into 25 minutes. Here are resources to go deeper:"

> "For official Red Hat resources: [point] the website, full documentation, GitHub repo, and demo videos."

> "For the case studies I mentioned: [point] the Spotify ROI study, the Infosys case study, and the article about Red Hat's AI tools."

> "And for community: [point] the main Backstage community at backstage.io, and Red Hat's learning resources."

> "I'll share these slides with links after the talk, so you don't need to write anything down."

### Key Points:
- Don't dwell on this slide
- Reassure them they'll get the links
- Move quickly to close

**Transition:** "Let's wrap up."

---

## Slide 17: Thank You! - 30 seconds

### What's On Screen:
- Your contact info, call to action

### What to Say:

> "Thank you so much for your time and attention! I'm Mitesh Kumar from Red Hat. If you want to connect, here's my email, LinkedIn, and GitHub."

> "Questions? I have about 1 minute for quick questions, but I'll also be around afterward if you want to chat more. Who has a question?"

### Key Points:
- Be warm and approachable
- Open up for questions
- Invite personal conversations

**For Q&A:**
- Repeat each question so everyone hears it
- Answer concisely
- If you don't know, say so: "Great question, I don't know off the top of my head, but let me find out and I'll email you"
- If running long: "I see we're out of time, but I'll stick around - let's continue this offline"

---

## Slide 18: Call to Action - 30 seconds

### What's On Screen:
- Next steps for attendees and platform teams

### What to Say:

> "Before you leave, three concrete next steps:"

> "**One:** Try the online demo today. No installation, takes 10 minutes, you'll see if this fits your needs."

> "**Two:** Read those case studies - Spotify and Infosys. See how others have done this."

> "**Three:** If you're on a platform team, run a pilot. Pick 1-2 teams, measure before and after, show your leadership the ROI."

> "Developer portals are becoming table stakes in platform engineering. Start your journey today."

### Key Points:
- Give clear, actionable next steps
- Create urgency
- End on a high note

---

## Post-Talk Actions (Immediately After)

### What to Do:

1. **Thank the organizers** - Find event organizers, thank them personally

2. **Be available** - Don't rush away. People want to ask questions.

3. **Exchange contacts** - Have your phone ready for LinkedIn QR code or business cards if you have them

4. **Take notes** - Write down questions you couldn't answer, feedback, interesting conversations

5. **Share resources** - Send slides/links to organizers to distribute

### Common Questions You Might Get:

**Q: "How long does implementation take?"**
A: "POC in 1 day, pilot with a team in 1 week, full rollout 1-3 months depending on organization size."

**Q: "Can we customize templates?"**
A: "Absolutely. Templates are YAML files in Git. Modify existing ones or create new ones."

**Q: "What about GitLab instead of GitHub?"**
A: "RHDH supports GitHub, GitLab, Bitbucket, and self-hosted Git."

**Q: "How much does it cost?"**
A: "Infrastructure costs $500-2K/month, admin time 0.5-1 FTE, Red Hat subscription - contact sales. But ROI is typically 3-6 months."

**Q: "How does this compare to [competitor]?"**
A: "Great question. RHDH is unique because it's open-source-based, so no vendor lock-in, plus enterprise support. Happy to discuss specific comparisons offline."

**Q: "Can we migrate from Backstage?"**
A: "Yes! RHDH is Backstage-compatible. Your existing plugins and catalog work as-is."

**Q: "Is this only for Red Hat customers?"**
A: "No, RHDH works on any Kubernetes. Red Hat ecosystem integration is a bonus, not a requirement."

---

## Self-Evaluation Checklist (After Event)

Reflect on these:

- [ ] Did I stay within 25 minutes?
- [ ] Did the demo work smoothly?
- [ ] Did I emphasize the real data effectively?
- [ ] Was my energy level appropriate?
- [ ] Did I engage the audience?
- [ ] What questions did people ask? (Note for next time)
- [ ] What went better than expected?
- [ ] What could I improve for next time?
- [ ] Did I make meaningful connections?

---

## Follow-Up (Within 1 Week)

- [ ] LinkedIn post about the talk with key takeaways
- [ ] Email answers to questions you couldn't answer
- [ ] Connect with people you met
- [ ] Internal blog post for Red Hat (share learnings)
- [ ] Update slides based on feedback
- [ ] Prepare for Dec 5 Tech Day presentation (if applicable)

---

## Emergency Situations

### If Demo Environment is Down:

> "Looks like our demo environment isn't cooperating today - I should have made a sacrifice to the demo gods! But let me show you screenshots of this exact workflow. The concept is the same..."

Then use backup screenshots. Make a joke, move on confidently.

### If You Forget Something:

> "Let me circle back to that point..." (Don't apologize profusely, just continue)

### If You're Running Long:

> "I see we're running short on time, so let me quickly summarize..." (Skip less critical slides, hit the highlights)

### If You're Running Short:

> "We have a few extra minutes, so let me show you [additional feature / take more questions / go deeper on X]"

### If Someone Asks a Hostile Question:

> "That's an interesting perspective. In my experience... [give your view politely]. But I'd love to hear more about your situation afterward and see if we can find common ground."

Stay professional, don't get defensive.

### If Technology Fails Completely:

> "Well, this gives me a chance to practice my improv! Let me tell you about RHDH..." (Do the talk without slides if needed - you know the content)

---

## Confidence Reminders

**Before Going On:**

- You know this material
- The technology is genuinely useful
- You're helping people solve real problems
- The audience wants you to succeed
- It's okay if things aren't perfect
- Take a deep breath
- Smile
- You've got this! 🚀

**Good luck at the Platform Engineering Meetup!**

---

**Document End**

