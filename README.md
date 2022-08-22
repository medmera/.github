# Starter Workflows
Starter workflows for the medmera organization.
## CI
### [Maven Simple Verify](.github/workflow-templates/ci/maven-simple-verify.yml)
Verify PRs that are targeted for the develop branch. This workflow is intended for simple testless builds.

### [Maven Simple Release](.github/workflow-templates/ci/maven-simple-release.yml)
Releases artifact automatically when code is pushed to the develop branch. This workflow is intended for simple testless builds.

### [Maven Push to Feature](.github/workflow-templates/ci/maven-push-to-feature.json)
Verifies (quick) and optionally deploys a feature branch SNAPSHOT of the project when code is pushed to a feature branch

### [Maven Verify Develop PR](.github/workflow-templates/ci/maven-verify-develop-pr.yml)
Verifies (full) a PR targeted for development

### [Maven Push to Develop](.github/workflow-templates/ci/maven-push-to-develop.yml)
Verifies (full) and Releases the project when code is pushed to the develop branch

## Deployments
### [Terraform (GCP) Plan](.github/workflow-templates/deployments/terraform-gcp-plan.yml)
Runs Terraform plan for GCP Infrastructure when a PR is created or updated targeting an environment branch

### [Terraform (GCP) Apply](.github/workflow-templates/deployments/terraform-gcp-apply.yml)
Runs Terraform apply for GCP Infrastructure when code is merged to an environment branch

### [Terraform (GCP) Merge PR](.github/workflow-templates/deployments/terraform-gcp-merge-pr.yml)
Comment on PR when if it targets an environment branch and has been closed/merged

## Utilities
### [Post Link to Release Job if PR Merged](.github/workflow-templates/utilities/post-link-to-release-job-if-pr-merged.yml)
Posts PR comment with link to release workflow job when a PR targeted for the branch develop is merged
