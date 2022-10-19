![](https://img.shields.io/badge/Repository-GitHub-5534eb)
![](https://img.shields.io/badge/Language-Yaml-1a3a99)
# Starter Workflows
Starter workflows for the medmera organization.
## CI
### [Maven Simple Verify](workflow-templates/maven-simple-verify.yml)
Verify PRs that are targeted for the develop branch. This workflow is intended for simple testless builds.

### [Maven Simple Release](workflow-templates/maven-simple-release.yml)
Releases artifact automatically when code is pushed to the develop branch. This workflow is intended for simple testless builds.

### [Maven Push to Feature](workflow-templates/maven-push-to-feature.yml)
Verifies (quick) and optionally deploys a feature branch SNAPSHOT of the project when code is pushed to a feature branch

### [Maven Verify Develop PR](workflow-templates/maven-verify-develop-pr.yml)
Verifies (full) a PR targeted for development

### [Maven Push to Develop](workflow-templates/maven-push-to-develop.yml)
Verifies (full) and Releases the project when code is pushed to the develop branch

## Deployments
### [Terraform (GCP) Plan](workflow-templates/terraform-gcp-plan.yml)
Runs Terraform plan for GCP Infrastructure when a PR is created or updated targeting an environment branch

### [Terraform (GCP) Apply](workflow-templates/terraform-gcp-apply.yml)
Runs Terraform apply for GCP Infrastructure when code is merged to an environment branch

### [Terraform (GCP) Merge PR](workflow-templates/terraform-gcp-merge-pr.yml)
Comment on PR when if it targets an environment branch and has been closed/merged

## Code Scan
### [Maven Nightly Vulnarbility Scan](workflow-templates/maven-owasp-nightly-vulnarbility-scan.yml)
Scans dependencies for known vulnarbilities using OWASP maven plugin nightly

## Utilities
### [Post Link to Release Job if PR Merged](workflow-templates/post-link-to-release-job-if-pr-merged.yml)
Posts PR comment with link to release workflow job when a PR targeted for the branch develop is merged
