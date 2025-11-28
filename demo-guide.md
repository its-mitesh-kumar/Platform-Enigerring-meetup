# Demo Script for RHDH Presentation
## Platform Engineering Meetup - Nov 29, 2025

### Pre-Demo Setup Checklist

**Environment:**
- [ ] RHDH instance running and accessible
- [ ] Demo account logged in
- [ ] Browser tabs pre-arranged:
  - Tab 1: RHDH Home
  - Tab 2: Software Catalog
  - Tab 3: Create Component
  - Tab 4: GitHub (for showing created repo)
- [ ] Sample services visible in catalog
- [ ] Network connection stable

**Backup Plan:**
- [ ] Screenshots of each step ready
- [ ] Screen recording of successful demo
- [ ] PDF export of the demo flow

---

## Demo Flow: Creating a Microservice (5 minutes)

### Step 1: Introduce the Portal (30 seconds)

**What to Say:**
> "Let me show you how a developer can go from zero to a fully configured service in under 5 minutes using RHDH. Remember, this is built on Backstage, but enterprise-ready out of the box."

**Actions:**
1. Show RHDH home page
2. Briefly highlight the navigation:
   - Catalog
   - APIs
   - Docs
   - Create

**Key Points to Make:**
- "Single portal, no context switching"
- "This is Backstage's core functionality, enhanced by Red Hat"

---

### Step 2: Browse Existing Catalog (45 seconds)

**What to Say:**
> "First, let's see what services already exist in our organization. This is the Software Catalog - our single source of truth."

**Actions:**
1. Navigate to Catalog
2. Show different filters:
   - By owner
   - By tag
   - By type
3. Click on one service to show:
   - Overview
   - Relations (dependencies)
   - CI/CD status
   - Documentation

**Key Points to Make:**
- "All services in one place"
- "Clear ownership"
- "Live status from Kubernetes"
- "Integrated documentation"

---

### Step 3: Create New Component (45 seconds)

**What to Say:**
> "Now let's create a new service. I'll use our Golden Path template for a Quarkus microservice."

**Actions:**
1. Click "Create" button
2. Show available templates:
   - Spring Boot API
   - Quarkus Service
   - Node.js Express
   - React Frontend
3. Select "Quarkus Microservice"

**Key Point to Make:**
- "Multiple templates, all with best practices built in"

---

### Step 4: Fill Template Form (60 seconds)

**What to Say:**
> "I just need to provide some basic information. Notice how simple this is - no need to know about pipeline configuration or Kubernetes manifests."

**Actions:**
Fill in form with pre-decided values:

```
Service Name: customer-rewards-api
Description: API for managing customer loyalty points
Owner: platform-team
System: loyalty-program
Repository:
  Organization: acme-corp
  Repository: customer-rewards-api
  Host: github.com
```

**Key Points to Make:**
- "Simple form, complex automation behind the scenes"
- "Team ownership defined upfront"
- "Part of larger system architecture"

**Click "Review" then "Create"**

---

### Step 5: Watch RHDH Magic Happen (90 seconds)

**What to Say:**
> "RHDH is now doing all the heavy lifting. Watch what's being created automatically."

**What RHDH Creates (show the progress):**

1. ✅ Creating GitHub repository
2. ✅ Scaffolding Quarkus project structure
3. ✅ Creating Tekton CI/CD pipeline
4. ✅ Generating Kubernetes manifests
5. ✅ Setting up monitoring configs
6. ✅ Creating documentation site
7. ✅ Registering in software catalog

**Key Point to Make:**
- "All of this would normally take hours or days to set up manually"
- "Everything follows our organization's best practices"

---

### Step 6: Verify Created Assets (60 seconds)

**What to Say:**
> "Let's verify what was created. I'll show you the GitHub repo, the pipeline, and the catalog entry."

**Actions:**

1. **Show GitHub Repo:**
   - Switch to GitHub tab
   - Navigate to new repo
   - Show file structure:
     ```
     customer-rewards-api/
     ├── src/
     │   ├── main/java/...
     │   └── test/java/...
     ├── .tekton/
     │   └── pipeline.yaml
     ├── k8s/
     │   ├── deployment.yaml
     │   └── service.yaml
     ├── docs/
     │   └── index.md
     ├── catalog-info.yaml
     └── pom.xml
     ```

2. **Show Tekton Pipeline:**
   - Back to RHDH
   - Navigate to service in catalog
   - Show "CI/CD" tab
   - Point out pipeline is already running

3. **Show Catalog Entry:**
   - Show "Overview" tab
   - Show "Relations" graph
   - Show "Docs" tab

**Key Points to Make:**
- "Complete project structure"
- "CI/CD already running"
- "Documentation already available"
- "Service is now part of our architecture"

---

### Closing Statement (10 seconds)

**What to Say:**
> "And that's it! In less than 5 minutes, our developer has a fully functional service with CI/CD, documentation, and monitoring - all integrated and ready to go. They can now focus on writing business logic instead of infrastructure."

---

## Demo Talking Points

### If Demo is Going Well:
- Show additional features:
  - API documentation
  - Dependencies graph
  - Tech stack visualization
  - Search functionality

### If Running Short on Time:
- Skip showing GitHub repo
- Focus on catalog entry and pipeline
- Mention other features verbally

### If Demo Fails:
- Have screenshots ready
- Say: "Let me show you what this looks like" and walk through screenshots
- Show pre-recorded video if available
- Emphasize the concept over the execution

---

## Audience Engagement During Demo

### Questions to Ask:

1. Before starting:
   > "How long does it typically take in your organization to set up a new service with all the necessary infrastructure?"

2. After showing templates:
   > "How many of you have standardized templates in your organization?"

3. After completion:
   > "Can you imagine how much time this would save your teams?"

---

## Technical Details (If Asked)

### About the Template Engine:

**Template is defined using:**
```yaml
apiVersion: scaffolder.backstage.io/v1beta3
kind: Template
metadata:
  name: quarkus-microservice
spec:
  parameters:
    - title: Service Details
      properties:
        name:
          type: string
        owner:
          type: string
  steps:
    - id: fetch
      name: Fetch Template
      action: fetch:template
    - id: publish
      name: Publish to GitHub
      action: publish:github
    - id: register
      name: Register Component
      action: catalog:register
```

### About Dynamic Plugins:

- Templates are loaded dynamically
- No need to rebuild RHDH
- Custom templates can be added easily
- Version controlled like any other code

### About Security:

- Uses service account for GitHub access
- No developer credentials stored
- Audit log of all actions
- RBAC controls who can create what

---

## Post-Demo Questions to Anticipate

### Q: "Can we customize the templates?"

**A:** "Absolutely! Templates are just YAML files in your Git repository. You can modify existing templates or create new ones. The template uses actions like fetch, publish, and register that you can compose together."

### Q: "What if we use GitLab instead of GitHub?"

**A:** "RHDH supports multiple Git providers - GitHub, GitLab, Bitbucket, and even self-hosted instances. You just need to configure the appropriate integration."

### Q: "How do you handle secrets in the generated code?"

**A:** "Great question! We use placeholders that reference your secret management system - whether that's Vault, OpenShift secrets, or another solution. The pipeline pulls secrets at runtime, never commits them to the repo."

### Q: "Can developers still customize after creation?"

**A:** "Yes! The template creates a starting point. Developers have full control over the repository afterward. They can modify pipelines, add dependencies, change configurations - it's their code."

### Q: "What if we want to update all services created from a template?"

**A:** "That's where the catalog comes in. You can query all services created from a template and update them programmatically. We also version templates so new services get updates automatically."

---

## Success Metrics to Share

After the demo, reinforce with real numbers:

- **Time to first commit:** 2 weeks → 2 days
- **Service creation:** 4 hours → 5 minutes  
- **Pipeline setup:** 2 hours → automatic
- **Documentation setup:** 1 hour → automatic
- **Developer satisfaction:** 6.5/10 → 8.9/10

---

## Demo Environment Details

### URL Structure:
```
RHDH Portal: https://rhdh.apps.ocp.example.com
Demo User: mitesh.kumar@example.com
Demo Org: acme-corp
```

### Pre-existing Services to Reference:
1. `payment-service` - Java Spring Boot
2. `user-management-api` - Node.js
3. `frontend-app` - React
4. `data-pipeline` - Python

### Template Names:
- Quarkus Microservice
- Spring Boot API
- Node.js Express API
- React Frontend Application
- Python Data Pipeline

---

## Backup Commands (If Needed)

### To check RHDH status:
```bash
oc get pods -n rhdh
oc logs -f deployment/rhdh -n rhdh
```

### To verify GitHub integration:
```bash
curl -H "Authorization: token $GITHUB_TOKEN" \
  https://api.github.com/user
```

### To manually trigger catalog refresh:
```bash
curl -X POST https://rhdh.example.com/api/catalog/refresh
```

---

## Final Checklist Before Going Live

- [ ] RHDH accessible
- [ ] Demo user logged in  
- [ ] All tabs open and organized
- [ ] Backup screenshots saved to Desktop
- [ ] GitHub token valid
- [ ] Presentation mode enabled (hide bookmarks, etc.)
- [ ] Zoom level set to 125% for visibility
- [ ] Speaker notes open on second screen
- [ ] Water bottle handy
- [ ] Confident smile ready! 😊

Good luck with the demo! Remember: it's okay if something goes wrong - use it as an opportunity to show troubleshooting or have a good laugh with the audience. The concept is what matters!

