# CI/CD Interview Questions (100 Total)

---

# CI/CD Fundamentals

1. What is CI/CD?
2. What does CI stand for?
3. What does CD stand for?
4. What is Continuous Integration?
5. What is Continuous Delivery?
6. What is Continuous Deployment?
7. What is the difference between Continuous Delivery and Continuous Deployment?
8. Why is CI/CD important?
9. What problems does CI/CD solve?
10. What are the benefits of CI/CD?

---

# DevOps Concepts

11. What is DevOps?
12. How is DevOps related to CI/CD?
13. What is the DevOps lifecycle?
14. What are the stages of a CI/CD pipeline?
15. What is automation in DevOps?
16. Why should deployments be automated?
17. What is infrastructure as code?
18. What is configuration management?
19. What is the difference between development, staging, and production environments?
20. What CI/CD best practices do you follow?

---

# CI Pipeline

21. What happens during Continuous Integration?
22. What steps are included in a CI pipeline?
23. What is a build process?
24. What is automated testing in CI?
25. Why should tests run before deployment?
26. What happens when a CI pipeline fails?
27. How do you debug CI failures?
28. What is a build artifact?
29. How do you manage build artifacts?
30. What CI tools have you used?

---

# CD Pipeline

31. What happens during Continuous Delivery?
32. What happens during Continuous Deployment?
33. What are deployment pipelines?
34. What are deployment stages?
35. How do you deploy automatically after a successful build?
36. How do you handle failed deployments?
37. What is deployment approval?
38. What is a release pipeline?
39. How do you rollback deployments?
40. What CD best practices do you follow?

---

# CI/CD Tools

41. What is GitHub Actions?
42. How does GitHub Actions work?
43. What is Jenkins?
44. What is GitLab CI/CD?
45. What is CircleCI?
46. What is Travis CI?
47. What is the difference between Jenkins and GitHub Actions?
48. How do CI/CD tools integrate with Git repositories?
49. How do you choose a CI/CD tool?
50. What CI/CD tools have you used in real projects?

---

# GitHub Actions & Workflow Automation

51. What is a GitHub Actions workflow?
52. What is a workflow file?
53. Where are GitHub Actions workflow files stored?
54. What is YAML in GitHub Actions?
55. What are events in GitHub Actions?
56. What are jobs in GitHub Actions?
57. What are steps in GitHub Actions?
58. What are actions in GitHub Actions?
59. What are runners in GitHub Actions?
60. How do you create a CI pipeline using GitHub Actions?

---

# Environment & Secrets Management

61. What are environment variables in CI/CD?
62. Why should environment variables not be hardcoded?
63. How do you manage secrets in CI/CD pipelines?
64. What are GitHub Actions secrets?
65. How do you protect API keys in CI/CD?
66. How do you manage different environments?
67. What is the difference between development, staging, and production secrets?
68. How do you rotate CI/CD secrets?
69. What security risks exist in CI/CD pipelines?
70. What CI/CD security best practices do you follow?

---

# Docker & CI/CD Integration

71. Why is Docker used in CI/CD?
72. How do you build Docker images in CI pipelines?
73. How do you push Docker images to a registry?
74. How do you deploy Docker containers automatically?
75. How do GitHub Actions and Docker work together?
76. How do you version Docker images?
77. How do you rollback Docker deployments?
78. What is a container registry?
79. What is Docker Hub?
80. What Docker CI/CD practices do you follow?

---

# Deployment Strategies

81. What is a deployment strategy?
82. What is the traditional deployment approach?
83. What is rolling deployment?
84. What is blue-green deployment?
85. What is canary deployment?
86. What is recreate deployment?
87. What are the advantages of blue-green deployment?
88. What are the risks of canary deployment?
89. How do you choose a deployment strategy?
90. What deployment strategies have you used?

---

# Production & Senior CI/CD Questions

91. How do you design a CI/CD pipeline for a production application?
92. How do you deploy a Next.js application using CI/CD?
93. How do you deploy a Node.js API using CI/CD?
94. How do you handle database migrations in CI/CD?
95. How do you prevent broken deployments?
96. How do you monitor deployments?
97. How do you handle production rollback?
98. What CI/CD mistakes do junior developers commonly make?
99. What CI/CD practices do you use in real projects?
100. In your opinion, what separates a junior, mid-level, and senior CI/CD engineer?

---

# ANSWERS

---

# Part 1 (1–10): CI/CD Fundamentals

---

## Question 1: What is CI/CD?

## Answer:
CI/CD stands for Continuous Integration and Continuous Delivery/Deployment. It's a set of practices that automate the process of building, testing, and deploying code changes.

- **CI**: Automatically build and test code on every change.
- **CD**: Automatically deploy validated code to production.

## Key Points:
- Automates build, test, and deployment.
- CI: integrate and test frequently.
- CD: deploy automatically or with approval.
- Reduces manual errors.
- Faster release cycles.

## Interview Tip:
"CI/CD automates the path from code change to production — build, test, deploy."

---

## Question 2: What does CI stand for?

## Answer:
CI stands for **Continuous Integration** — the practice of frequently merging code changes into a shared repository and automatically building and testing them.

## Key Points:
- Continuous Integration.
- Frequent code merges.
- Automated builds and tests.
- Early bug detection.
- Team collaboration.

## Interview Tip:
"CI means integrating code frequently and verifying it automatically."

---

## Question 3: What does CD stand for?

## Answer:
CD stands for **Continuous Delivery** or **Continuous Deployment**:
- **Continuous Delivery**: Code is always ready to deploy (manual approval).
- **Continuous Deployment**: Code is automatically deployed to production.

## Key Points:
- Continuous Delivery: ready to deploy, manual approval.
- Continuous Deployment: automatic deployment.
- Both automate the release process.
- Delivery is safer; Deployment is faster.

## Interview Tip:
"Delivery = ready to deploy; Deployment = auto-deploy. Know the difference."

---

## Question 4: What is Continuous Integration?

## Answer:
Continuous Integration is the practice of frequently merging code changes into a shared repository, where each merge triggers an automated build and test sequence.

```yaml
# GitHub Actions CI
on: [push, pull_request]
jobs:
  test:
    runs-on: ubuntu-latest
    steps:
      - uses: actions/checkout@v4
      - run: npm ci
      - run: npm test
```

## Key Points:
- Frequent code merges.
- Automated build and test.
- Early bug detection.
- Fast feedback loop.
- Shared repository.

## Interview Tip:
"CI catches bugs early — every push is automatically tested."

---

## Question 5: What is Continuous Delivery?

## Answer:
Continuous Delivery extends CI by ensuring code is always in a deployable state. After passing tests, code is ready to be deployed to production with manual approval.

## Key Points:
- Code always ready to deploy.
- Manual approval before production.
- Automated testing and staging.
- Reduces deployment risk.
- Faster release cycles.

## Interview Tip:
"Continuous Delivery means the code is always ready — you just push the button."

---

## Question 6: What is Continuous Deployment?

## Answer:
Continuous Deployment goes further — every change that passes tests is automatically deployed to production without manual intervention.

## Key Points:
- Automatic deployment to production.
- No manual approval.
- Requires comprehensive testing.
- Fastest release cycle.
- Highest confidence in tests.

## Interview Tip:
"Continuous Deployment is the ultimate — every passing change goes straight to production."

---

## Question 7: What is the difference between Continuous Delivery and Continuous Deployment?

## Answer:
| Feature | Continuous Delivery | Continuous Deployment |
|---------|-------------------|----------------------|
| Deployment | Manual approval | Automatic |
| Risk | Lower (human gate) | Higher (fully automated) |
| Speed | Fast | Fastest |
| Testing | Comprehensive | Most comprehensive |

## Key Points:
- Delivery: manual approval.
- Deployment: automatic.
- Delivery is safer.
- Deployment is faster.
- Choose based on confidence in tests.

## Interview Tip:
"Delivery has a manual gate; Deployment doesn't. Choose based on your test confidence."

---

## Question 8: Why is CI/CD important?

## Answer:
- **Faster releases**: Automate manual processes.
- **Fewer errors**: Automated testing catches bugs.
- **Consistency**: Same process every time.
- **Feedback**: Quick feedback on changes.
- **Confidence**: Tests validate changes.
- **Collaboration**: Frequent integration prevents conflicts.

## Key Points:
- Faster release cycles.
- Fewer manual errors.
- Consistent deployments.
- Quick feedback.
- Team collaboration.

## Interview Tip:
"CI/CD is important because it makes releases fast, safe, and consistent."

---

## Question 9: What problems does CI/CD solve?

## Answer:
1. **Manual deployments**: Error-prone and slow.
2. **Integration conflicts**: Infrequent merges cause conflicts.
3. **Slow feedback**: Developers wait days for bugs.
4. **Inconsistent environments**: "Works on my machine."
5. **Deployment fear**: Releases are stressful events.

## Key Points:
- Manual deployment errors.
- Integration conflicts.
- Slow feedback loops.
- Environment inconsistency.
- Deployment anxiety.

## Interview Tip:
"CI/CD turns deployments from stressful events into routine operations."

---

## Question 10: What are the benefits of CI/CD?

## Answer:
- **Speed**: Faster time to market.
- **Quality**: Automated testing improves code quality.
- **Reliability**: Consistent, repeatable deployments.
- **Feedback**: Quick feedback on changes.
- **Collaboration**: Frequent integration reduces conflicts.
- **Confidence**: Tests validate every change.

## Key Points:
- Faster releases.
- Better quality.
- Reliable deployments.
- Quick feedback.
- Team collaboration.
- Deployment confidence.

## Interview Tip:
"CI/CD benefits: speed, quality, reliability, feedback, collaboration, confidence."

---

# Part 2 (11–20): DevOps Concepts

---

## Question 11: What is DevOps?

## Answer:
DevOps is a culture and set of practices that combines software development (Dev) and IT operations (Ops). It aims to shorten the development lifecycle and deliver high-quality software continuously.

## Key Points:
- Culture and practices.
- Dev + Ops collaboration.
- Shorter development lifecycle.
- Continuous delivery.
- Automation focus.

## Interview Tip:
"DevOps is a culture, not a tool — it's about collaboration and automation."

---

## Question 12: How is DevOps related to CI/CD?

## Answer:
CI/CD is a core DevOps practice. DevOps emphasizes automation, and CI/CD automates the build, test, and deployment process.

```
DevOps = Culture + Practices
CI/CD = Automation of build, test, deploy
```

## Key Points:
- CI/CD is a DevOps practice.
- DevOps is the culture.
- CI/CD is the automation.
- Both aim for faster, reliable delivery.
- CI/CD enables DevOps goals.

## Interview Tip:
"CI/CD is the automation backbone of DevOps."

---

## Question 13: What is the DevOps lifecycle?

## Answer:
1. **Plan**: Define requirements.
2. **Code**: Write code.
3. **Build**: Compile and package.
4. **Test**: Automated testing.
5. **Release**: Prepare for deployment.
6. **Deploy**: Deploy to production.
7. **Operate**: Monitor and maintain.
8. **Monitor**: Collect feedback.

## Key Points:
- Plan → Code → Build → Test → Release → Deploy → Operate → Monitor.
- Continuous loop.
- Automation at every stage.
- Feedback drives improvement.

## Interview Tip:
"The DevOps lifecycle is a continuous loop — plan, code, build, test, deploy, monitor."

---

## Question 14: What are the stages of a CI/CD pipeline?

## Answer:
1. **Source**: Code commit triggers pipeline.
2. **Build**: Compile and package code.
3. **Test**: Run automated tests.
4. **Deploy**: Deploy to staging/production.
5. **Monitor**: Verify deployment health.

## Key Points:
- Source → Build → Test → Deploy → Monitor.
- Each stage is automated.
- Failure stops the pipeline.
- Feedback at every stage.

## Interview Tip:
"Source → Build → Test → Deploy → Monitor — the five pipeline stages."

---

## Question 15: What is automation in DevOps?

## Answer:
Automation removes manual steps from the software delivery process. It includes:
- **Build automation**: Compile and package code.
- **Test automation**: Run tests automatically.
- **Deployment automation**: Deploy without manual steps.
- **Infrastructure automation**: Provision servers automatically.

## Key Points:
- Remove manual steps.
- Build, test, deploy automation.
- Infrastructure automation.
- Consistency and speed.
- Fewer human errors.

## Interview Tip:
"Automation is the heart of DevOps — if it can be automated, it should be."

---

## Question 16: Why should deployments be automated?

## Answer:
- **Consistency**: Same process every time.
- **Speed**: Seconds instead of hours.
- **Reliability**: No human errors.
- **Rollback**: Easy to revert.
- **Confidence**: Tested and validated.
- **Frequency**: Deploy more often.

## Key Points:
- Consistent deployments.
- Faster releases.
- Fewer errors.
- Easy rollback.
- Higher deployment frequency.

## Interview Tip:
"Manual deployments are slow, error-prone, and stressful. Automate them."

---

## Question 17: What is infrastructure as code?

## Answer:
Infrastructure as Code (IaC) manages infrastructure through code files instead of manual configuration.

```yaml
# Docker Compose
services:
  app:
    image: my-app:1.0
    ports:
      - "3000:3000"
```

Tools: Terraform, CloudFormation, Docker Compose, Ansible.

## Key Points:
- Infrastructure defined in code.
- Version controlled.
- Reproducible environments.
- Automated provisioning.
- Tools: Terraform, CloudFormation.

## Interview Tip:
"IaC means your infrastructure is version-controlled and reproducible."

---

## Question 18: What is configuration management?

## Answer:
Configuration management automates the setup and maintenance of software and infrastructure configurations.

Tools: Ansible, Chef, Puppet, Terraform.

## Key Points:
- Automate configuration setup.
- Consistent environments.
- Version controlled.
- Tools: Ansible, Chef, Puppet.
- Reduces manual configuration.

## Interview Tip:
"Configuration management ensures every environment is configured identically."

---

## Question 19: What is the difference between development, staging, and production environments?

## Answer:
- **Development**: Local machines, for coding.
- **Staging**: Pre-production, for testing.
- **Production**: Live, for users.

```
Dev → Staging → Production
```

## Key Points:
- Development: coding and testing.
- Staging: pre-production validation.
- Production: live environment.
- Staging mirrors production.
- Progressive promotion.

## Interview Tip:
"Staging is the dress rehearsal — it should mirror production exactly."

---

## Question 20: What CI/CD best practices do you follow?

## Answer:
1. **Automate everything**: Build, test, deploy.
2. **Test early, test often**: Run tests on every push.
3. **Keep pipelines fast**: <10 minutes ideal.
4. **Version control everything**: Code, config, infrastructure.
5. **Monitor deployments**: Verify health after deploy.
6. **Rollback plan**: Always have a rollback strategy.

## Key Points:
- Automate everything.
- Test on every push.
- Fast pipelines.
- Version control.
- Monitor and rollback.

## Interview Tip:
"Automate everything, test on every push, keep pipelines fast."

---

# Part 3 (21–30): CI Pipeline

---

## Question 21: What happens during Continuous Integration?

## Answer:
1. Developer pushes code.
2. CI server detects change.
3. Code is built.
4. Tests are run.
5. Results are reported.
6. If passed, code is merged.

## Key Points:
- Push triggers pipeline.
- Build → Test → Report.
- Failure blocks merge.
- Fast feedback.
- Automated process.

## Interview Tip:
"CI = push → build → test → report → merge."

---

## Question 22: What steps are included in a CI pipeline?

## Answer:
1. **Checkout**: Clone repository.
2. **Install dependencies**: `npm ci`.
3. **Lint**: Check code style.
4. **Build**: Compile code.
5. **Test**: Run tests.
6. **Report**: Notify results.

## Key Points:
- Checkout code.
- Install dependencies.
- Lint and build.
- Run tests.
- Report results.

## Interview Tip:
"Checkout → Install → Lint → Build → Test → Report."

---

## Question 23: What is a build process?

## Answer:
The build process compiles and packages code into a deployable artifact.

```bash
npm run build  # Compile TypeScript, bundle assets
docker build . # Build Docker image
```

## Key Points:
- Compile and package code.
- Create deployable artifact.
- TypeScript compilation.
- Asset bundling.
- Docker image creation.

## Interview Tip:
"The build process turns source code into something deployable."

---

## Question 24: What is automated testing in CI?

## Answer:
Automated tests run automatically during the CI pipeline to verify code correctness.

```yaml
- run: npm test        # Unit tests
- run: npm run test:e2e # E2E tests
```

## Key Points:
- Runs automatically in CI.
- Unit, integration, E2E tests.
- Catches bugs before deployment.
- Fast feedback.
- Gate for deployment.

## Interview Tip:
"Automated tests are the quality gate — they prevent broken code from reaching production."

---

## Question 25: Why should tests run before deployment?

## Answer:
- **Catch bugs**: Before they reach production.
- **Confidence**: Tests validate changes.
- **Safety**: Prevent broken deployments.
- **Quality**: Maintain code quality.
- **Cost**: Cheaper to fix in CI than production.

## Key Points:
- Catch bugs early.
- Deployment confidence.
- Prevent production issues.
- Maintain quality.
- Cheaper to fix early.

## Interview Tip:
"Testing before deployment is the safety net — it catches bugs before users do."

---

## Question 26: What happens when a CI pipeline fails?

## Answer:
1. Pipeline stops at the failed stage.
2. Error details are reported.
3. Developer is notified.
4. Code cannot be merged (if branch protection).
5. Developer fixes the issue and pushes again.

## Key Points:
- Pipeline stops.
- Error reported.
- Developer notified.
- Merge blocked.
- Fix and re-push.

## Interview Tip:
"A failed pipeline blocks the merge — fix the issue before proceeding."

---

## Question 27: How do you debug CI failures?

## Answer:
1. **Read the logs**: Check error messages.
2. **Reproduce locally**: Run the same commands locally.
3. **Check environment**: Differences between local and CI.
4. **Check dependencies**: Version mismatches.
5. **Check secrets**: Missing environment variables.

## Key Points:
- Read CI logs.
- Reproduce locally.
- Check environment differences.
- Verify dependencies.
- Check secrets.

## Interview Tip:
"Read the logs first, then reproduce locally — most CI failures are environment differences."

---

## Question 28: What is a build artifact?

## Answer:
A build artifact is the output of the build process — a deployable package.

Examples:
- Docker image.
- Compiled JavaScript bundle.
- ZIP file.
- JAR file.

## Key Points:
- Output of build process.
- Deployable package.
- Docker image, bundle, ZIP.
- Stored in artifact repository.
- Versioned and traceable.

## Interview Tip:
"Build artifacts are what you deploy — Docker images, bundles, or packages."

---

## Question 29: How do you manage build artifacts?

## Answer:
1. **Store in registry**: Docker Hub, ECR, S3.
2. **Version with tags**: Semantic versioning, Git SHA.
3. **Retain policy**: Keep recent, delete old.
4. **Security**: Scan for vulnerabilities.

## Key Points:
- Store in registries.
- Version with tags.
- Retention policy.
- Security scanning.
- Traceable to source.

## Interview Tip:
"Store artifacts in registries, version them, and scan for vulnerabilities."

---

## Question 30: What CI tools have you used?

## Answer:
- **GitHub Actions**: Built into GitHub.
- **Jenkins**: Self-hosted, highly customizable.
- **GitLab CI/CD**: Built into GitLab.
- **CircleCI**: Cloud-based, fast.
- **Travis CI**: Cloud-based, open source friendly.

## Key Points:
- GitHub Actions: GitHub-native.
- Jenkins: self-hosted, customizable.
- GitLab CI/CD: GitLab-native.
- CircleCI: cloud-based.
- Travis CI: open source.

## Interview Tip:
"GitHub Actions for GitHub projects; Jenkins for complex self-hosted pipelines."

---

# Part 4 (31–40): CD Pipeline

---

## Question 31: What happens during Continuous Delivery?

## Answer:
1. Code passes CI (build + test).
2. Artifact is created.
3. Deployed to staging.
4. Automated tests run on staging.
5. Ready for production (manual approval).

## Key Points:
- CI passes → deploy to staging.
- Test on staging.
- Manual approval for production.
- Always in deployable state.
- Automated up to production.

## Interview Tip:
"Continuous Delivery = automated to staging, manual gate to production."

---

## Question 32: What happens during Continuous Deployment?

## Answer:
1. Code passes CI (build + test).
2. Artifact is created.
3. Deployed to staging.
4. Tests run on staging.
5. Automatically deployed to production.

## Key Points:
- Fully automated.
- No manual approval.
- Deployed to production automatically.
- Requires comprehensive tests.
- Fastest release cycle.

## Interview Tip:
"Continuous Deployment = fully automated, including production."

---

## Question 33: What are deployment pipelines?

## Answer:
Deployment pipelines define the stages code goes through from commit to production.

```
Build → Test → Staging → Production
```

Each stage is automated and gates the next.

## Key Points:
- Stages from commit to production.
- Each stage gates the next.
- Automated progression.
- Failure stops the pipeline.
- Visual representation of flow.

## Interview Tip:
"Deployment pipelines are the automated path from code to production."

---

## Question 34: What are deployment stages?

## Answer:
1. **Build**: Compile and package.
2. **Test**: Run automated tests.
3. **Staging**: Deploy to staging environment.
4. **Approval**: Manual approval (optional).
5. **Production**: Deploy to production.

## Key Points:
- Build → Test → Staging → Approval → Production.
- Each stage validates the previous.
- Approval is optional (Delivery vs Deployment).
- Failure at any stage stops the pipeline.

## Interview Tip:
"Stages are gates — each one must pass before the next begins."

---

## Question 35: How do you deploy automatically after a successful build?

## Answer:
```yaml
# GitHub Actions
deploy:
  needs: build
  if: github.ref == 'refs/heads/main'
  runs-on: ubuntu-latest
  steps:
    - name: Deploy
      run: ./deploy.sh
```

`needs: build` ensures deployment only runs after build succeeds.

## Key Points:
- `needs` for dependency.
- `if` for conditional deployment.
- Only deploy from main branch.
- Automate with scripts.
- Verify deployment health.

## Interview Tip:
"Use `needs` to chain jobs — deployment only runs after build succeeds."

---

## Question 36: How do you handle failed deployments?

## Answer:
1. **Automatic rollback**: Revert to previous version.
2. **Alert team**: Notify immediately.
3. **Investigate**: Check logs and metrics.
4. **Fix forward**: Push fix and redeploy.
5. **Post-mortem**: Analyze what went wrong.

## Key Points:
- Automatic rollback.
- Alert the team.
- Investigate logs.
- Fix forward if possible.
- Post-mortem for learning.

## Interview Tip:
"Automatic rollback is the safety net — always have a rollback plan."

---

## Question 37: What is deployment approval?

## Answer:
Deployment approval requires manual confirmation before deploying to production. It's the gate in Continuous Delivery.

```yaml
environment:
  name: production
  url: https://example.com
```

GitHub Actions can require approvals via environment protection rules.

## Key Points:
- Manual confirmation before production.
- Gate in Continuous Delivery.
- Environment protection rules.
- Review before deploy.
- Extra safety layer.

## Interview Tip:
"Deployment approval is the human gate — it adds safety to Continuous Delivery."

---

## Question 38: What is a release pipeline?

## Answer:
A release pipeline is the complete process from code commit to production release, including build, test, staging, approval, and deployment.

## Key Points:
- Complete process from commit to production.
- Includes all stages.
- Automated where possible.
- Manual gates where needed.
- Documented and repeatable.

## Interview Tip:
"A release pipeline is the full journey from code to production."

---

## Question 39: How do you rollback deployments?

## Answer:
```bash
# Docker: deploy previous version
docker run my-app:v1.0.0

# Kubernetes
kubectl rollout undo deployment/my-app

# GitHub Actions: deploy previous tag
```

## Key Points:
- Deploy previous version.
- Kubernetes rollback commands.
- Keep previous versions available.
- Automate rollback process.
- Test rollback regularly.

## Interview Tip:
"Rollback is just deploying the previous version — keep previous versions available."

---

## Question 40: What CD best practices do you follow?

## Answer:
1. **Automate deployments**: No manual steps.
2. **Environment parity**: Staging mirrors production.
3. **Rollback plan**: Always have a rollback strategy.
4. **Health checks**: Verify deployment health.
5. **Monitoring**: Monitor after deployment.
6. **Small batches**: Deploy small, frequent changes.

## Key Points:
- Automated deployments.
- Environment parity.
- Rollback plan.
- Health checks.
- Monitoring.
- Small, frequent deploys.

## Interview Tip:
"Small, frequent deployments with automated rollback — that's the CD ideal."

---

# Part 5 (41–50): CI/CD Tools

---

## Question 41: What is GitHub Actions?

## Answer:
GitHub Actions is a CI/CD platform built into GitHub. It automates workflows based on Git events (push, PR, etc.).

```yaml
on: [push]
jobs:
  test:
    runs-on: ubuntu-latest
    steps:
      - uses: actions/checkout@v4
      - run: npm test
```

## Key Points:
- Built into GitHub.
- Event-driven workflows.
- YAML configuration.
- Free for public repos.
- Large marketplace.

## Interview Tip:
"GitHub Actions is CI/CD built into GitHub — it's the default for GitHub projects."

---

## Question 42: How does GitHub Actions work?

## Answer:
1. **Event triggers**: Push, PR, schedule.
2. **Workflow runs**: GitHub starts a runner.
3. **Jobs execute**: Steps run in sequence/parallel.
4. **Results reported**: Pass/fail on PR.

## Key Points:
- Event-driven.
- Runner execution.
- Jobs and steps.
- Results reported.
- YAML configuration.

## Interview Tip:
"GitHub Actions is event-driven — trigger on push, PR, or schedule."

---

## Question 43: What is Jenkins?

## Answer:
Jenkins is an open-source automation server for building CI/CD pipelines. It's self-hosted and highly customizable with plugins.

## Key Points:
- Open-source automation server.
- Self-hosted.
- Highly customizable.
- Plugin ecosystem.
- Jenkinsfile for pipeline definition.

## Interview Tip:
"Jenkins is the veteran CI/CD tool — self-hosted and highly customizable."

---

## Question 44: What is GitLab CI/CD?

## Answer:
GitLab CI/CD is built into GitLab. It uses `.gitlab-ci.yml` for pipeline configuration.

```yaml
test:
  script:
    - npm ci
    - npm test
```

## Key Points:
- Built into GitLab.
- `.gitlab-ci.yml` configuration.
- Integrated with GitLab features.
- Runners for execution.
- Auto DevOps feature.

## Interview Tip:
"GitLab CI/CD is the GitLab-native solution — `.gitlab-ci.yml` defines the pipeline."

---

## Question 45: What is CircleCI?

## Answer:
CircleCI is a cloud-based CI/CD platform known for speed and simplicity.

## Key Points:
- Cloud-based CI/CD.
- Fast execution.
- Simple configuration.
- Docker support.
- Free tier available.

## Interview Tip:
"CircleCI is known for speed — it's a good choice for fast CI/CD."

---

## Question 46: What is Travis CI?

## Answer:
Travis CI is a cloud-based CI service, popular in open-source projects.

## Key Points:
- Cloud-based CI.
- Popular for open source.
- `.travis.yml` configuration.
- GitHub integration.
- Free for open source.

## Interview Tip:
"Travis CI was the go-to for open-source projects — GitHub Actions has largely replaced it."

---

## Question 47: What is the difference between Jenkins and GitHub Actions?

## Answer:
| Feature | Jenkins | GitHub Actions |
|---------|---------|----------------|
| Hosting | Self-hosted | GitHub-hosted |
| Configuration | Jenkinsfile | YAML |
| Setup | Complex | Simple |
| Plugins | Extensive | Marketplace |
| Cost | Free (hosting costs) | Free for public |

## Key Points:
- Jenkins: self-hosted, complex, customizable.
- GitHub Actions: hosted, simple, GitHub-native.
- Jenkins for complex enterprise needs.
- GitHub Actions for GitHub projects.

## Interview Tip:
"Jenkins for complex enterprise; GitHub Actions for simplicity and GitHub integration."

---

## Question 48: How do CI/CD tools integrate with Git repositories?

## Answer:
1. **Webhooks**: Git events trigger pipelines.
2. **Branch protection**: Require CI to pass before merge.
3. **Status checks**: Report pass/fail on PRs.
4. **Automatic triggers**: Push, PR, merge events.

## Key Points:
- Webhooks for event triggers.
- Branch protection rules.
- Status checks on PRs.
- Automatic triggers.
- Deep integration.

## Interview Tip:
"CI/CD tools listen for Git events — push triggers the pipeline automatically."

---

## Question 49: How do you choose a CI/CD tool?

## Answer:
Consider:
1. **Hosting**: Self-hosted vs cloud.
2. **Integration**: GitHub, GitLab, Bitbucket.
3. **Complexity**: Simple vs customizable.
4. **Cost**: Free tier, pricing.
5. **Ecosystem**: Plugins, actions, marketplace.

## Key Points:
- Hosting preference.
- Git platform integration.
- Complexity needs.
- Budget.
- Ecosystem.

## Interview Tip:
"Choose based on your Git platform, hosting preference, and complexity needs."

---

## Question 50: What CI/CD tools have you used in real projects?

## Answer:
- **GitHub Actions**: For GitHub projects.
- **Jenkins**: For enterprise self-hosted.
- **GitLab CI/CD**: For GitLab projects.
- **Vercel**: For Next.js deployments.
- **AWS CodePipeline**: For AWS deployments.

## Key Points:
- GitHub Actions for GitHub.
- Jenkins for enterprise.
- GitLab CI/CD for GitLab.
- Vercel for Next.js.
- AWS CodePipeline for AWS.

## Interview Tip:
"Name the tools you've actually used and describe your experience with each."

---

# Part 6 (51–60): GitHub Actions & Workflow Automation

---

## Question 51: What is a GitHub Actions workflow?

## Answer:
A workflow is an automated process defined in a YAML file. It's triggered by events and contains jobs.

```yaml
name: CI
on: [push]
jobs:
  test:
    runs-on: ubuntu-latest
    steps:
      - uses: actions/checkout@v4
      - run: npm test
```

## Key Points:
- Automated process.
- YAML configuration.
- Triggered by events.
- Contains jobs and steps.
- Stored in `.github/workflows/`.

## Interview Tip:
"Workflows are YAML files in `.github/workflows/` — they define your CI/CD pipeline."

---

## Question 52: What is a workflow file?

## Answer:
A workflow file is a YAML file that defines a GitHub Actions workflow.

```yaml
name: CI
on: [push, pull_request]
jobs:
  test:
    runs-on: ubuntu-latest
    steps:
      - uses: actions/checkout@v4
      - run: npm ci
      - run: npm test
```

## Key Points:
- YAML format.
- Defines triggers, jobs, steps.
- Stored in `.github/workflows/`.
- Multiple workflows per repo.
- Version controlled.

## Interview Tip:
"Workflow files are YAML in `.github/workflows/` — version control them."

---

## Question 53: Where are GitHub Actions workflow files stored?

## Answer:
In `.github/workflows/` directory in the repository.

```
.github/
  workflows/
    ci.yml
    deploy.yml
    release.yml
```

## Key Points:
- `.github/workflows/` directory.
- YAML files.
- Version controlled.
- Multiple workflow files.
- Auto-detected by GitHub.

## Interview Tip:
"Workflow files go in `.github/workflows/` — GitHub auto-detects them."

---

## Question 54: What is YAML in GitHub Actions?

## Answer:
YAML is the configuration format for GitHub Actions workflows. It defines triggers, jobs, steps, and options.

```yaml
name: CI
on: [push]
jobs:
  test:
    runs-on: ubuntu-latest
    steps:
      - run: npm test
```

## Key Points:
- Configuration format.
- Defines triggers, jobs, steps.
- Human-readable.
- Indentation-sensitive.
- Standard for CI/CD.

## Interview Tip:
"YAML is the language of CI/CD — learn its syntax."

---

## Question 55: What are events in GitHub Actions?

## Answer:
Events trigger workflows.

```yaml
on:
  push:
    branches: [main]
  pull_request:
    branches: [main]
  schedule:
    - cron: '0 0 * * *'
```

## Key Points:
- Trigger workflows.
- `push`, `pull_request`, `schedule`.
- Branch filtering.
- Cron scheduling.
- Manual triggers (`workflow_dispatch`).

## Interview Tip:
"`push` and `pull_request` are the most common triggers."

---

## Question 56: What are jobs in GitHub Actions?

## Answer:
Jobs are groups of steps that run on a runner.

```yaml
jobs:
  test:
    runs-on: ubuntu-latest
    steps: [...]
  deploy:
    needs: test
    runs-on: ubuntu-latest
    steps: [...]
```

## Key Points:
- Groups of steps.
- Run on runners.
- Can run in parallel.
- `needs` for dependencies.
- Multiple jobs per workflow.

## Interview Tip:
"Jobs are independent units — they can run in parallel or in sequence."

---

## Question 57: What are steps in GitHub Actions?

## Answer:
Steps are individual commands or actions within a job.

```yaml
steps:
  - uses: actions/checkout@v4
  - run: npm ci
  - run: npm test
```

## Key Points:
- Individual commands or actions.
- Run sequentially within a job.
- `run` for shell commands.
- `uses` for actions.
- Can share data between steps.

## Interview Tip:
"Steps are the individual tasks — `run` for commands, `uses` for actions."

---

## Question 58: What are actions in GitHub Actions?

## Answer:
Actions are reusable units of workflow logic.

```yaml
steps:
  - uses: actions/checkout@v4
  - uses: actions/setup-node@v4
```

Available on GitHub Marketplace.

## Key Points:
- Reusable workflow logic.
- `uses` to reference.
- GitHub Marketplace.
- Version tags.
- Custom or third-party.

## Interview Tip:
"Actions are reusable — use them from the Marketplace instead of writing everything from scratch."

---

## Question 59: What are runners in GitHub Actions?

## Answer:
Runners are servers that execute workflow jobs.

- **GitHub-hosted**: Managed by GitHub (ubuntu, windows, macos).
- **Self-hosted**: Managed by you.

```yaml
runs-on: ubuntu-latest  # GitHub-hosted
runs-on: self-hosted    # Self-hosted
```

## Key Points:
- Execute workflow jobs.
- GitHub-hosted or self-hosted.
- Ubuntu, Windows, macOS.
- `runs-on` specifies the runner.
- Self-hosted for custom environments.

## Interview Tip:
"GitHub-hosted for most cases; self-hosted for custom environments or cost savings."

---

## Question 60: How do you create a CI pipeline using GitHub Actions?

## Answer:
```yaml
name: CI
on: [push, pull_request]
jobs:
  test:
    runs-on: ubuntu-latest
    steps:
      - uses: actions/checkout@v4
      - uses: actions/setup-node@v4
        with:
          node-version: 20
      - run: npm ci
      - run: npm run lint
      - run: npm test
```

## Key Points:
- Trigger on push and PR.
- Checkout code.
- Setup environment.
- Install dependencies.
- Lint and test.

## Interview Tip:
"Checkout → Setup → Install → Lint → Test — the basic CI pipeline."

---

# Part 7 (61–70): Environment & Secrets Management

---

## Question 61: What are environment variables in CI/CD?

## Answer:
Environment variables provide configuration to the pipeline without hardcoding values.

```yaml
env:
  NODE_ENV: production
  API_URL: ${{ secrets.API_URL }}
```

## Key Points:
- Configuration without hardcoding.
- Different per environment.
- Secrets for sensitive data.
- `${{ secrets.NAME }}` syntax.
- Set in workflow or repository settings.

## Interview Tip:
"Environment variables configure your pipeline — secrets for sensitive values."

---

## Question 62: Why should environment variables not be hardcoded?

## Answer:
- **Security**: Secrets exposed in code.
- **Flexibility**: Same code, different config.
- **Portability**: Works across environments.
- **Version control**: Don't commit secrets.

## Key Points:
- Security risk.
- Flexibility lost.
- Portability issues.
- Never commit secrets.
- Use environment variables.

## Interview Tip:
"Never hardcode secrets — use environment variables and secrets management."

---

## Question 63: How do you manage secrets in CI/CD pipelines?

## Answer:
1. **Repository secrets**: Stored in CI/CD platform.
2. **Environment variables**: Injected at runtime.
3. **Secret managers**: HashiCorp Vault, AWS Secrets Manager.
4. **Never in code**: Don't commit secrets.

## Key Points:
- Repository secrets.
- Runtime injection.
- Secret managers.
- Never in code.
- Rotate regularly.

## Interview Tip:
"Store secrets in the CI/CD platform, inject at runtime, never commit to code."

---

## Question 64: What are GitHub Actions secrets?

## Answer:
Secrets are encrypted environment variables stored in GitHub repository settings.

```yaml
steps:
  - run: echo ${{ secrets.API_KEY }}
  - env:
      API_KEY: ${{ secrets.API_KEY }}
```

## Key Points:
- Encrypted environment variables.
- Stored in repository settings.
- `${{ secrets.NAME }}` syntax.
- Not visible in logs.
- Per-repository or organization-level.

## Interview Tip:
"GitHub secrets are encrypted — they're never exposed in logs."

---

## Question 65: How do you protect API keys in CI/CD?

## Answer:
1. **Store as secrets**: GitHub Actions secrets.
2. **Never commit**: `.gitignore` `.env` files.
3. **Inject at runtime**: Use secrets in workflow.
4. **Rotate regularly**: Change keys periodically.
5. **Limit access**: Only necessary repos/users.

## Key Points:
- Store as secrets.
- Never commit to code.
- Runtime injection.
- Regular rotation.
- Access control.

## Interview Tip:
"API keys go in secrets, never in code — inject at runtime."

---

## Question 66: How do you manage different environments?

## Answer:
```yaml
jobs:
  deploy-staging:
    environment: staging
    steps: [...]
  deploy-production:
    environment: production
    needs: deploy-staging
    steps: [...]
```

GitHub environments have separate secrets and approval rules.

## Key Points:
- Separate environments.
- Different secrets per environment.
- Approval rules per environment.
- Progressive promotion.
- Environment protection rules.

## Interview Tip:
"Use GitHub environments for staging and production — separate secrets and approvals."

---

## Question 67: What is the difference between development, staging, and production secrets?

## Answer:
- **Development**: Local `.env` files, test credentials.
- **Staging**: Staging API keys, test database.
- **Production**: Production API keys, real database.

Each environment has its own secrets.

## Key Points:
- Different secrets per environment.
- Development: test credentials.
- Staging: staging credentials.
- Production: production credentials.
- Never share across environments.

## Interview Tip:
"Each environment gets its own secrets — never share production secrets with staging."

---

## Question 68: How do you rotate CI/CD secrets?

## Answer:
1. **Generate new secret**: Create new API key/token.
2. **Update in CI/CD**: Update secret in platform.
3. **Verify**: Run pipeline to verify.
4. **Revoke old**: Delete old secret.

## Key Points:
- Generate new secret.
- Update in CI/CD platform.
- Verify pipeline works.
- Revoke old secret.
- Automate if possible.

## Interview Tip:
"Rotate secrets regularly — generate new, update, verify, revoke old."

---

## Question 69: What security risks exist in CI/CD pipelines?

## Answer:
1. **Exposed secrets**: Secrets in logs or code.
2. **Malicious actions**: Third-party actions with vulnerabilities.
3. **Unauthorized access**: Weak access controls.
4. **Supply chain attacks**: Compromised dependencies.
5. **Privilege escalation**: Excessive permissions.

## Key Points:
- Exposed secrets.
- Malicious actions.
- Unauthorized access.
- Supply chain attacks.
- Excessive permissions.

## Interview Tip:
"The biggest risk is exposed secrets — audit your pipeline regularly."

---

## Question 70: What CI/CD security best practices do you follow?

## Answer:
1. **Use secrets management**: Never hardcode.
2. **Pin action versions**: Use specific versions, not `@latest`.
3. **Least privilege**: Minimal permissions.
4. **Audit logs**: Monitor pipeline activity.
5. **Scan dependencies**: Check for vulnerabilities.
6. **Environment protection**: Approval rules.

## Key Points:
- Secrets management.
- Pin action versions.
- Least privilege.
- Audit logs.
- Dependency scanning.
- Environment protection.

## Interview Tip:
"Pin action versions, use secrets, and apply least privilege — the security trifecta."

---

# Part 8 (71–80): Docker & CI/CD Integration

---

## Question 71: Why is Docker used in CI/CD?

## Answer:
- **Consistency**: Same environment in CI and production.
- **Isolation**: Clean environment per build.
- **Portability**: Works anywhere Docker runs.
- **Reproducibility**: Same build every time.

## Key Points:
- Consistent environments.
- Isolated builds.
- Portable across platforms.
- Reproducible builds.
- Industry standard.

## Interview Tip:
"Docker ensures CI/CD environments match production — no more 'works in CI, fails in production.'"

---

## Question 72: How do you build Docker images in CI pipelines?

## Answer:
```yaml
- name: Build
  run: docker build -t my-app:${{ github.sha }} .
```

## Key Points:
- `docker build` in CI.
- Tag with commit SHA.
- Use multi-stage builds.
- Cache layers for speed.
- Push to registry.

## Interview Tip:
"Tag images with commit SHA for traceability."

---

## Question 73: How do you push Docker images to a registry?

## Answer:
```yaml
- name: Login
  run: docker login -u ${{ secrets.DOCKER_USER }} -p ${{ secrets.DOCKER_PASS }}
- name: Push
  run: docker push my-app:${{ github.sha }}
```

## Key Points:
- Login to registry.
- Push with tag.
- Use secrets for credentials.
- Automate in CI/CD.
- Version with tags.

## Interview Tip:
"Login, tag, push — automate the entire process in CI/CD."

---

## Question 74: How do you deploy Docker containers automatically?

## Answer:
1. **Push to registry**: CI builds and pushes.
2. **Webhook triggers**: Registry notifies deployment.
3. **Pull new image**: Deployment system pulls.
4. **Restart containers**: With new image.

## Key Points:
- Push triggers deployment.
- Webhook notifications.
- Pull and restart.
- Health checks.
- Rollback on failure.

## Interview Tip:
"Push → webhook → pull → restart — the automated Docker deployment flow."

---

## Question 75: How do GitHub Actions and Docker work together?

## Answer:
```yaml
jobs:
  build:
    runs-on: ubuntu-latest
    steps:
      - uses: actions/checkout@v4
      - name: Build
        run: docker build -t my-app:${{ github.sha }} .
      - name: Push
        run: docker push my-app:${{ github.sha }}
      - name: Deploy
        run: ./deploy.sh
```

## Key Points:
- Build in GitHub Actions.
- Push to registry.
- Deploy automatically.
- Tag with SHA.
- Secrets for credentials.

## Interview Tip:
"GitHub Actions + Docker = automated build, push, and deploy."

---

## Question 76: How do you version Docker images?

## Answer:
- **Git SHA**: `my-app:abc123` (traceable).
- **Semantic version**: `my-app:v1.0.0` (releases).
- **Branch name**: `my-app:main` (latest).
- **Build number**: `my-app:build-123` (sequential).

## Key Points:
- Git SHA for traceability.
- Semantic version for releases.
- Avoid `latest` in production.
- Consistent tagging strategy.
- Multiple tags per image.

## Interview Tip:
"Use Git SHA for traceability; semantic version for releases."

---

## Question 77: How do you rollback Docker deployments?

## Answer:
```bash
# Pull previous version
docker pull my-app:v1.0.0

# Restart with previous version
docker-compose up -d
```

Or with Kubernetes:
```bash
kubectl rollout undo deployment/my-app
```

## Key Points:
- Pull previous version.
- Restart with old image.
- Kubernetes rollback commands.
- Keep previous versions.
- Automate rollback.

## Interview Tip:
"Rollback is just deploying the previous version — keep previous images available."

---

## Question 78: What is a container registry?

## Answer:
A container registry stores and distributes Docker images.

- **Docker Hub**: Default public registry.
- **AWS ECR**: Amazon's registry.
- **GitHub Container Registry**: GitHub's registry.
- **Azure ACR**: Azure's registry.

## Key Points:
- Stores Docker images.
- Public and private options.
- Push and pull images.
- Version management.
- Security scanning.

## Interview Tip:
"Docker Hub for public; private registries for proprietary images."

---

## Question 79: What is Docker Hub?

## Answer:
Docker Hub is the default public registry for Docker images. It hosts official images and user-published images.

## Key Points:
- Default public registry.
- Official images.
- User-published images.
- Free for public repositories.
- Private repositories available.

## Interview Tip:
"Docker Hub is the GitHub of Docker images — it's the default registry."

---

## Question 80: What Docker CI/CD practices do you follow?

## Answer:
1. **Build in CI**: Automated builds.
2. **Tag with SHA**: Traceability.
3. **Push to registry**: Central storage.
4. **Scan images**: Security scanning.
5. **Deploy automatically**: CD pipeline.
6. **Health checks**: Verify deployment.

## Key Points:
- Automated builds.
- SHA tagging.
- Registry storage.
- Security scanning.
- Automated deployment.
- Health checks.

## Interview Tip:
"Build, tag, push, scan, deploy, verify — the Docker CI/CD pipeline."

---

# Part 9 (81–90): Deployment Strategies

---

## Question 81: What is a deployment strategy?

## Answer:
A deployment strategy defines how new code is released to production. It balances speed, risk, and downtime.

## Key Points:
- How code is released.
- Balances speed and risk.
- Minimizes downtime.
- Enables rollback.
- Choose based on needs.

## Interview Tip:
"Deployment strategy = how you release code. Choose based on risk tolerance."

---

## Question 82: What is the traditional deployment approach?

## Answer:
Traditional deployment replaces the entire application at once. All instances are updated simultaneously.

- **Risk**: High (all-or-nothing).
- **Downtime**: Yes.
- **Rollback**: Manual.

## Key Points:
- Replace everything at once.
- High risk.
- Downtime required.
- Manual rollback.
- Simple but risky.

## Interview Tip:
"Traditional deployment is simple but risky — all-or-nothing."

---

## Question 83: What is rolling deployment?

## Answer:
Rolling deployment gradually replaces instances one by one.

```
[v1] [v1] [v1] [v1]
[v2] [v1] [v1] [v1]
[v2] [v2] [v1] [v1]
[v2] [v2] [v2] [v1]
[v2] [v2] [v2] [v2]
```

## Key Points:
- Gradual replacement.
- Zero downtime.
- Mixed versions during rollout.
- Easy rollback.
- Most common strategy.

## Interview Tip:
"Rolling deployment = gradual replacement, zero downtime."

---

## Question 84: What is blue-green deployment?

## Answer:
Blue-green deployment maintains two identical environments. Traffic switches from blue (current) to green (new).

```
Blue (v1) ← Live traffic
Green (v2) ← Testing

Switch traffic:

Blue (v1) ← Standby
Green (v2) ← Live traffic
```

## Key Points:
- Two identical environments.
- Instant traffic switch.
- Zero downtime.
- Easy rollback (switch back).
- Double resources required.

## Interview Tip:
"Blue-green = instant switch, easy rollback, but double resources."

---

## Question 85: What is canary deployment?

## Answer:
Canary deployment gradually shifts traffic to the new version.

```
[v1] [v1] [v1] [v1] [v1] [v1] [v1] [v1] [v1] [v1]  # 100% v1
[v2] [v1] [v1] [v1] [v1] [v1] [v1] [v1] [v1] [v1]  # 10% v2
[v2] [v2] [v2] [v2] [v2] [v1] [v1] [v1] [v1] [v1]  # 50% v2
[v2] [v2] [v2] [v2] [v2] [v2] [v2] [v2] [v2] [v2]  # 100% v2
```

## Key Points:
- Gradual traffic shift.
- Monitor new version.
- Rollback if issues.
- Lower risk than full deployment.
- Requires traffic splitting.

## Interview Tip:
"Canary deployment = gradual rollout with monitoring. Rollback if issues detected."

---

## Question 86: What is recreate deployment?

## Answer:
Recreate deployment stops all old instances, then starts new ones.

```
[v1] [v1] [v1] → Stop all
                 → Start all
[v2] [v2] [v2]
```

## Key Points:
- Stop old, start new.
- Downtime required.
- Simple but risky.
- No mixed versions.
- Use for non-critical apps.

## Interview Tip:
"Recreate deployment has downtime — use only for non-critical applications."

---

## Question 87: What are the advantages of blue-green deployment?

## Answer:
- **Zero downtime**: Instant traffic switch.
- **Easy rollback**: Switch back to blue.
- **Testing**: Test green before switching.
- **Confidence**: Full testing before going live.

## Key Points:
- Zero downtime.
- Easy rollback.
- Pre-switch testing.
- High confidence.
- Double resources.

## Interview Tip:
"Blue-green's biggest advantage is instant rollback — switch back if issues."

---

## Question 88: What are the risks of canary deployment?

## Answer:
- **Complexity**: Requires traffic splitting.
- **Monitoring**: Must monitor canary closely.
- **State**: Mixed versions may have state issues.
- **Rollback**: Not instant like blue-green.

## Key Points:
- Complex setup.
- Requires monitoring.
- State management issues.
- Slower rollback.
- Trade-off: lower risk, more complexity.

## Interview Tip:
"Canary is lower risk but more complex — you need good monitoring."

---

## Question 89: How do you choose a deployment strategy?

## Answer:
- **Zero downtime required**: Rolling or blue-green.
- **Instant rollback**: Blue-green.
- **Low risk**: Canary.
- **Simple app**: Recreate.
- **Resource constraints**: Rolling.

## Key Points:
- Based on requirements.
- Zero downtime: rolling or blue-green.
- Instant rollback: blue-green.
- Low risk: canary.
- Simple: recreate.

## Interview Tip:
"Choose based on downtime tolerance, rollback needs, and resource constraints."

---

## Question 90: What deployment strategies have you used?

## Answer:
- **Rolling deployment**: Most common for APIs.
- **Blue-green**: For critical applications.
- **Canary**: For high-traffic services.
- **Recreate**: For development/staging.

## Key Points:
- Rolling for APIs.
- Blue-green for critical apps.
- Canary for high traffic.
- Recreate for dev/staging.
- Choose based on needs.

## Interview Tip:
"Describe your experience with each strategy and when you used it."

---

# Part 10 (91–100): Production & Senior CI/CD Questions

---

## Question 91: How do you design a CI/CD pipeline for a production application?

## Answer:
```
Push → Lint → Build → Test → Staging Deploy → Integration Tests → Production Deploy → Health Check
```

## Key Points:
- Lint for code quality.
- Build for compilation.
- Test for correctness.
- Staging for validation.
- Production for release.
- Health check for verification.

## Interview Tip:
"Lint → Build → Test → Staging → Production → Health Check — the full pipeline."

---

## Question 92: How do you deploy a Next.js application using CI/CD?

## Answer:
```yaml
name: Deploy Next.js
on:
  push:
    branches: [main]
jobs:
  deploy:
    runs-on: ubuntu-latest
    steps:
      - uses: actions/checkout@v4
      - uses: actions/setup-node@v4
      - run: npm ci
      - run: npm run build
      - run: npm run deploy  # Or use Vercel/Netlify action
```

## Key Points:
- Trigger on main branch.
- Build the application.
- Deploy to hosting (Vercel, Netlify, AWS).
- Environment variables.
- Health checks.

## Interview Tip:
"Next.js deploys easily to Vercel — GitHub Actions triggers the deployment."

---

## Question 93: How do you deploy a Node.js API using CI/CD?

## Answer:
```yaml
name: Deploy API
on:
  push:
    branches: [main]
jobs:
  deploy:
    runs-on: ubuntu-latest
    steps:
      - uses: actions/checkout@v4
      - run: npm ci
      - run: npm test
      - run: docker build -t api:${{ github.sha }} .
      - run: docker push api:${{ github.sha }}
      - run: ./deploy.sh
```

## Key Points:
- Test before deploy.
- Build Docker image.
- Push to registry.
- Deploy to server.
- Health checks.

## Interview Tip:
"Build → Test → Docker → Push → Deploy — the Node.js API deployment pipeline."

---

## Question 94: How do you handle database migrations in CI/CD?

## Answer:
```yaml
- name: Run migrations
  run: npx prisma migrate deploy
  env:
    DATABASE_URL: ${{ secrets.DATABASE_URL }}
```

Run migrations before deploying the new code.

## Key Points:
- Run before code deployment.
- Use migration tools (Prisma, Flyway).
- Environment-specific migrations.
- Rollback migrations if needed.
- Test migrations in staging.

## Interview Tip:
"Run migrations before deploying new code — test in staging first."

---

## Question 95: How do you prevent broken deployments?

## Answer:
1. **Automated tests**: Run tests before deployment.
2. **Staging environment**: Test in staging first.
3. **Branch protection**: Require CI to pass.
4. **Health checks**: Verify deployment.
5. **Rollback plan**: Automatic rollback on failure.

## Key Points:
- Automated tests.
- Staging environment.
- Branch protection.
- Health checks.
- Automatic rollback.

## Interview Tip:
"Tests + staging + health checks + rollback = safe deployments."

---

## Question 96: How do you monitor deployments?

## Answer:
1. **Health checks**: Verify application is running.
2. **Error tracking**: Sentry for errors.
3. **Performance monitoring**: Response times.
4. **Log monitoring**: Check for errors.
5. **Alerting**: Notify on issues.

## Key Points:
- Health checks.
- Error tracking.
- Performance monitoring.
- Log monitoring.
- Alerting.

## Interview Tip:
"Monitor health, errors, performance, and logs after every deployment."

---

## Question 97: How do you handle production rollback?

## Answer:
1. **Automatic**: Rollback on health check failure.
2. **Manual**: Trigger rollback via CI/CD.
3. **Kubernetes**: `kubectl rollout undo`.
4. **Docker**: Deploy previous image version.
5. **Database**: Rollback migrations if needed.

## Key Points:
- Automatic rollback.
- Manual trigger.
- Kubernetes commands.
- Previous image version.
- Database rollback.

## Interview Tip:
"Automatic rollback is the safety net — always have it configured."

---

## Question 98: What CI/CD mistakes do junior developers commonly make?

## Answer:
1. **No tests**: Deploying without tests.
2. **Hardcoded secrets**: Secrets in code.
3. **No staging**: Deploying directly to production.
4. **No rollback plan**: No way to revert.
5. **Slow pipelines**: Pipelines that take too long.
6. **No monitoring**: Not verifying deployments.

## Key Points:
- No tests.
- Hardcoded secrets.
- No staging.
- No rollback.
- Slow pipelines.
- No monitoring.

## Interview Tip:
"The biggest mistake is deploying without tests — always test before deploying."

---

## Question 99: What CI/CD practices do you use in real projects?

## Answer:
1. **GitHub Actions**: For CI/CD.
2. **Automated tests**: On every push.
3. **Staging environment**: Before production.
4. **Docker**: For consistent builds.
5. **Health checks**: After deployment.
6. **Rollback**: Automatic on failure.

## Key Points:
- GitHub Actions.
- Automated tests.
- Staging environment.
- Docker builds.
- Health checks.
- Automatic rollback.

## Interview Tip:
"GitHub Actions + Docker + staging + health checks + rollback — the production standard."

---

## Question 100: In your opinion, what separates a junior, mid-level, and senior CI/CD engineer?

## Answer:
- **Junior**: Can set up basic CI (run tests on push). Uses GitHub Actions templates.
- **Mid-level**: Designs multi-stage pipelines. Handles staging, secrets, and Docker.
- **Senior**: Designs complete CI/CD architecture. Handles deployment strategies, monitoring, rollback, and security. Mentors others.

The biggest differentiator: a senior thinks about failure scenarios and designs for resilience.

## Key Points:
- Junior: basic CI setup.
- Mid-level: multi-stage pipelines.
- Senior: architecture, strategies, monitoring.
- Senior designs for failure.
- Senior mentors others.

## Interview Tip:
"The best answer shows self-awareness. Pick your level and explain what you're doing to grow."

---
