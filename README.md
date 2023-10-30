# Auditmation Policy As Code

This template will create a new repository that allows compliance programs to be
built in GitHub using Markdown and YAML, allowing for:
  - Enhanced workflow where different teams can work in parallel
  - Peer reviews, pull requests, and diffs, and attributable changes
  - Intelligent merging of changes from external sources
  - Pipeline processing to kick off testing, update downstream artifcats, notifications, ...

## Getting Started

### Pre-requisities
1. This tool requires a valid [Auditmation](https://auditmation.io) account and system boundary.
1. Policy content license, either acquired in Auditmation platform or directly from author ([ComplianceForge](https://complianceforge.com), etc).


### Create a new repo
Click the green `Use this template` button on this page and then select `Create a new repository`. Complete fields to taste. No need to `Include all branches` so leave that unchecked.

### Secrets Configuration
The Gitub Actions workflows require the following
[secrets](https://docs.github.com/en/actions/security-guides/using-secrets-in-github-actions)
to be specified. They can be set as Environment, Repository, or Organization secrets as appropriate.

| Secret Name | Description | Default Value / Example |
| ----------- | ----------- | ----------------------- |
| api-url     | Auditmation platform API (optional) | `https://api.nf.auditmation.io` |
| api-key     | Auditmation API Key | ex: `1e96b700-7740-11ee-b962-0242ac120002` |
| org-id      | Auditmation Org ID | ex: `1e96b700-7740-11ee-b962-0242ac120005` |
| boundary-id | Boundary ID (optional). Required if more than 1 boundary present. | ex: `1e96b700-7740-11ee-b962-0242ac120009` |


