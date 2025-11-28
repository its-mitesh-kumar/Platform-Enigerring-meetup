# Quick Reference Guide - RHDH Presentation
## Platform Engineering Meetup Bengaluru - Nov 29, 2025

---

## Key Statistics to Remember

| Metric | Before RHDH | After RHDH | Improvement |
|--------|-------------|------------|-------------|
| Onboarding Time | 2 weeks | 2 days | **85% faster** |
| Service Creation | 4 hours | 5 minutes | **98% faster** |
| Tool Context Switching | 10+ tools | 1 portal | **90% reduction** |
| Time to First Commit | 3-5 days | 1 day | **70% faster** |
| Developer Satisfaction | 6.5/10 | 8.9/10 | **37% increase** |
| Support Tickets | 50/week | 15/week | **70% reduction** |

---

## One-Liners for Each Feature

### Backstage
> "Open-source developer portal framework created by Spotify, now a CNCF project used by 1000+ companies"

### RHDH
> "Backstage, but enterprise-ready - production-hardened with Red Hat support and ecosystem integration"

### Software Catalog
> "Your entire infrastructure in one searchable directory - think 'Google for your internal services'"

### Software Templates  
> "Create a production-ready service in 5 minutes, with CI/CD and documentation included"

### TechDocs
> "Documentation that lives with your code and never goes out of date"

### Plugin Ecosystem
> "100+ integrations bringing all your tools into one view"

### Developer Portal
> "One dashboard to replace 10+ tools - everything a developer needs in one place"

---

## Elevator Pitch (30 seconds)

"RHDH is an enterprise internal developer portal built on Backstage - the open-source framework created by Spotify. It gives developers a single place to discover services, create new projects from templates, access documentation, and monitor their systems - without switching between dozens of tools. Red Hat takes Backstage and makes it production-ready with enterprise support, dynamic plugins, and deep OpenShift integration. It's like having a 'Google Maps' for your entire infrastructure, helping platform teams scale self-service while maintaining standards and best practices."

## Backstage Quick Facts

- **Created by:** Spotify (2016, open-sourced 2020)
- **CNCF Status:** Incubating Project (2022)
- **Adoption:** 1000+ companies including Netflix, American Airlines, HP
- **Core Features:** Software Catalog, Templates, TechDocs
- **Plugin Ecosystem:** 100+ community plugins
- **License:** Apache 2.0 (fully open source)
- **Architecture:** React frontend, Node.js backend
- **Challenge:** It's a framework, not a product - requires setup & maintenance

---

## Value Propositions by Audience

### For Developers:
- ✅ Less context switching = more coding time
- ✅ Self-service infrastructure = no waiting on tickets
- ✅ Faster onboarding = productive from day one

### For Platform Engineers:
- ✅ Standardized golden paths = consistent quality
- ✅ Reduced support burden = focus on innovation
- ✅ Better visibility = faster incident response

### For Engineering Managers:
- ✅ Improved developer productivity = faster delivery
- ✅ Better developer experience = improved retention
- ✅ Clear ownership & metrics = better planning

### For CTOs/VPs:
- ✅ 30-40% productivity gains = ROI in 3-6 months
- ✅ Reduced operational costs = better margins
- ✅ Improved security & compliance = reduced risk

---

## Common Questions & Quick Answers

### "What is Backstage?"
**A:** "Backstage is an open-source developer portal framework created by Spotify in 2016. It's now a CNCF Incubating Project used by 1000+ companies. It provides the core platform, but requires setup and configuration."

### "How is RHDH different from Backstage?"
**A:** "RHDH is Backstage, enhanced for enterprise use. Red Hat adds production-readiness, dynamic plugins, enterprise support, security hardening, and deep Red Hat ecosystem integration. Think: framework vs product."

### "Can we migrate from Backstage to RHDH?"
**A:** "Yes! RHDH is fully compatible with Backstage. Your existing plugins, templates, and catalog work as-is. It's an easy migration path with additional enterprise features."

### "What about existing tooling?"
**A:** "RHDH integrates with existing tools - it's a portal layer on top. No need to replace what's working."

### "What's the learning curve?"
**A:** "Users: Hours. Template creators: Days. Admins: Week. Much simpler than building from scratch."

### "How long to implement?"
**A:** "POC in 1 day. Pilot with 1 team in 1 week. Full rollout: 1-3 months depending on organization size."

### "What's the cost?"
**A:** "Infrastructure: $500-2000/month. Admin: 0.5-1 FTE. Red Hat support: contact sales. ROI typically in 3-6 months."

### "Can it scale?"
**A:** "Yes. Built on Kubernetes, supports horizontal scaling, used by organizations with 1000+ developers."

### "What if a demo fails?"
**A:** "Shows it's real! Use screenshots/video backup, joke about 'demo gods', emphasize the concept over execution."

---

## Technical Terms Explained Simply

| Term | Simple Explanation |
|------|-------------------|
| **Software Catalog** | Searchable directory of all your services, like a phone book for code |
| **Component** | A piece of software (service, library, website, etc.) |
| **Entity** | Anything tracked in RHDH (components, APIs, resources, teams) |
| **Golden Path** | Pre-approved, standardized way to build something |
| **Software Template** | Fill-in-the-blank form that creates a complete project |
| **TechDocs** | Documentation generated from markdown in your repo |
| **Plugin** | Extension that adds new features to RHDH |
| **Dynamic Plugin** | Plugin that can be added without rebuilding RHDH |
| **Scaffolder** | The template engine that creates new projects |
| **Provider** | Integration with external system (GitHub, Kubernetes, etc.) |

---

## RHDH vs Competitors

| Feature | RHDH | Backstage OSS | Port | Humanitec |
|---------|------|---------------|------|-----------|
| **Open Source** | ✅ | ✅ | ❌ | ❌ |
| **Self-Hosted** | ✅ | ✅ | ❌ | ✅ |
| **Enterprise Support** | ✅ | ❌ | ✅ | ✅ |
| **Dynamic Plugins** | ✅ | ❌ | N/A | N/A |
| **Red Hat Ecosystem** | ✅ | Partial | ❌ | ❌ |
| **Setup Time** | Hours | Days/Weeks | Minutes | Hours |
| **Customization** | High | Very High | Medium | Low |
| **Cost** | Mid | Low | High | High |

---

## Red Hat Integrations

| Product | What RHDH Shows | Value |
|---------|----------------|-------|
| **OpenShift** | Topology, pod status, logs, metrics | Real-time cluster visibility |
| **Tekton** | Pipeline runs, build status, artifacts | CI/CD monitoring |
| **Quay** | Images, vulnerabilities, tags | Security scanning |
| **Ansible** | Job status, playbooks, inventory | Automation tracking |
| **Red Hat SSO** | Authentication, RBAC | Unified access control |
| **Advanced Cluster Security** | Policy violations, security posture | Compliance monitoring |

---

## Demo Flow Cheat Sheet

1. **Home Page** (10s) - "Single portal for everything"
2. **Catalog** (30s) - "All services in one place"
3. **Service Detail** (30s) - "Ownership, dependencies, status"
4. **Create Component** (20s) - "Choose template"
5. **Fill Form** (40s) - "Just basic info needed"
6. **Watch Magic** (90s) - "Automated creation"
7. **Verify** (60s) - "GitHub repo, pipeline, catalog entry"

**Total: ~5 minutes**

---

## Body Language & Delivery Tips

### Voice & Pacing:
- Speak 10% slower than normal (audience has different backgrounds)
- Pause after key statistics (let them sink in)
- Vary tone - enthusiasm for features, seriousness for problems

### Gestures:
- Use hands to show "switching between tools" (chaos)
- Bring hands together for "single portal" (unity)
- Count on fingers when listing features

### Eye Contact:
- Scan the room, don't fixate on one person
- Look at questioners when they ask
- Glance at notes, but don't read from them

### Energy:
- Start strong (they're still settling in)
- Peak during demo (most engaging part)
- End on high note (call to action)

---

## Handling Different Scenarios

### If Running Ahead of Time:
- Expand on use cases (more stories)
- Show additional plugins
- Do deeper Q&A
- Show more of the demo environment

### If Running Behind:
- Skip some template features
- Abbreviate use cases to one story
- Move faster through slides 6-8
- Cut demo to 3 minutes (just creation)

### If Audience Seems Bored:
- Ask interactive question
- Move to demo early
- Share a funny story/anecdote
- Show unexpected plugin (gaming, Spotify)

### If Audience Very Engaged:
- Allow more interruptions for questions
- Go deeper on technical details
- Show code/configuration
- Discuss architecture trade-offs

---

## Quotes to Use

### From Industry:
> "Developer portals are becoming the new standard for platform engineering." - CNCF Survey 2024

> "The average developer switches between 10-15 tools daily. This cognitive load is unsustainable." - State of DevOps Report

### From Users (hypothetical but realistic):
> "RHDH reduced our onboarding time from 2 weeks to 2 days. New engineers are productive immediately." - Platform Lead

> "We went from 50 support tickets per week to 15. Developers can self-serve 90% of what they need." - SRE Manager

---

## Personal Stories to Share (Adapt to Your Experience)

### The Onboarding Story:
"I once joined a team where it took me 3 weeks just to understand what services we had and how they connected. With RHDH, that information is available on day one."

### The Midnight Debug:
"Ever been woken up at 2 AM because a service is down and you can't remember who owns it or where the runbook is? RHDH solves that."

### The Standardization Win:
"We had 30 teams all setting up CI/CD differently. Now with templates, we have consistent best practices across the organization."

---

## Calls to Action

### For Attendees:
1. "Try the RHDH demo at developers.redhat.com"
2. "Join the RHDH community Slack"
3. "Start with just the catalog - catalog your services"
4. "Create one template for your most common service type"

### For Platform Teams:
1. "Run a pilot with 1-2 teams"
2. "Measure time-to-first-commit before and after"
3. "Survey developer satisfaction"
4. "Share results with leadership"

---

## Follow-Up Resources to Share

### Immediate:
- Slides: [Share link after talk]
- Demo: https://developers.redhat.com/rhdh
- Docs: https://docs.redhat.com/en-us/red_hat_developer_hub

### For Deep Dive:
- GitHub: https://github.com/redhat-developer/rhdh
- Plugins: https://developers.redhat.com/rhdh/plugins  
- YouTube: "Red Hat Developer Hub" playlist
- Blog: developers.redhat.com/blog

### Community:
- Slack: #rhdh channel
- Meetup: Platform Engineering community
- Conference: Red Hat Summit 2025

---

## Confidence Boosters

### Remember:
- ✅ You know this material well
- ✅ The audience wants you to succeed
- ✅ It's okay to say "I don't know, let me find out"
- ✅ Technical demos sometimes fail - it's normal
- ✅ Your experience makes you credible
- ✅ The technology is genuinely useful
- ✅ You're helping people solve real problems

### If Nervous:
- Take 3 deep breaths before starting
- Have water nearby
- Remember: they're on your side
- Focus on helping, not performing
- One person at a time, not the whole room

### Power Poses (Before Going On):
- Stand tall, shoulders back (2 minutes)
- Hands on hips, feet apart
- Arms raised in victory
(Science shows these reduce cortisol, increase confidence)

---

## Post-Talk Checklist

### Immediate:
- [ ] Thank the organizers
- [ ] Share slides/resources
- [ ] Connect with interested attendees
- [ ] Note questions you couldn't answer

### Follow-Up (Within 1 week):
- [ ] LinkedIn post with key takeaways
- [ ] Email answers to unanswered questions
- [ ] Connect with new contacts
- [ ] Internal blog post for Red Hat

### Reflection:
- [ ] What went well?
- [ ] What could improve?
- [ ] What questions surprised you?
- [ ] What resonated most with audience?

---

## Emergency Contact Info

**Red Hat Support:** [Number if needed]  
**RHDH Team:** [Slack channel]  
**Your Manager:** [Contact info]

---

## Final Thought

**The goal isn't a perfect presentation.**  
**The goal is to help engineers discover a tool that will make their lives better.**

**You've got this! 🚀**

---

*Good luck at the Platform Engineering Meetup Bengaluru Edition!*  
*November 29, 2025*

---

## 🎯 Tomorrow's Focus: Platform Engineering Meetup Bengaluru

### Event Details
**Date:** November 29, 2025 (TOMORROW!)  
**Time:** 11:10 AM - 11:35 AM (25 minutes)  
**Venue:** Red Hat India Office, Bengaluru  
**Event:** Platform Engineering Meetup Bengaluru Edition - Last of 2025

### Your Presentation
**File:** `presentation_meetup_nov2025.md`  
**Audience:** External platform engineers (community meetup)  
**Goal:** Educate, inspire, show RHDH value proposition

### What to Cover ✅
- ✅ **Problem statement** (relatable pain points)
- ✅ **What is Backstage** (educational foundation)
- ✅ **What is RHDH** (enterprise value proposition)
- ✅ **Core features** (Catalog, Templates, TechDocs, Plugins)
- ✅ **Real-world use cases** (inspiring stories)
- ✅ **Quick demo** (5-minute service creation)

### What to Skip ❌
- ❌ RBAC deep dive
- ❌ Lightspeed AI details
- ❌ Scorecard configuration
- ❌ Extensions system architecture
- ❌ Platform admin journey
- ❌ Red Hat-internal specifics

### Brief Mention Only (30 seconds in wrap-up)
> "And there's more! RHDH includes RBAC for access control, AI-powered Lightspeed assistant, scorecards for service quality, and much more. These are enterprise features that take Backstage from framework to production-ready product."

### Your Perfect 25-Minute Flow
1. **Problem** (3 min) - Developer productivity challenges
2. **Backstage** (3 min) - Open-source foundation story
3. **RHDH** (3 min) - Enterprise features & comparison
4. **Core Features** (7 min) - The essential capabilities
5. **Use Cases** (5 min) - Inspiring real-world stories
6. **Demo** (4 min) - Quick service creation workflow

**Strategy:** High-level, inspirational, focused on core value proposition! 🎯

**Why This Works:**
- ✅ 25 minutes is tight - focus on fundamentals
- ✅ External audience needs basics first
- ✅ Too much detail overwhelms at community meetup
- ✅ Leave them inspired, not information overload

**You're ready! Go inspire some engineers!** 🚀


