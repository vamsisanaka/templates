# Azure DevOps Pipeline Templates

Central repository for reusable Azure Pipeline templates across multiple technology stacks.

## Supported Technologies

- ✅ .NET (Core/Framework)


## Quick Start

### Using in Your Project

```yaml
resources:
  repositories:
    - repository: templates
      type: git
      name: YourOrg/azure-pipeline-templates
      ref: refs/heads/main

stages:
  - stage: Build
    jobs:
      - template: templates/jobs/jobs-template-dotnet.yml@templates


