# .github

Organization-wide defaults and templates for the eurosky-social GitHub organization.

## Purpose

This repository provides default community health files and workflow templates that apply to all repositories in the eurosky-social organization that don't have their own versions of these files.

## What Goes Here

### Community Health Files

Files that GitHub automatically uses across all repositories:

- **CODE_OF_CONDUCT.md** - Code of conduct for contributors
- **CONTRIBUTING.md** - Contribution guidelines
- **SECURITY.md** - Security policy and vulnerability reporting
- **SUPPORT.md** - Support resources and contact information
- **FUNDING.yml** - Sponsorship and funding information
- **ISSUE_TEMPLATE/** - Issue templates for all repos
- **PULL_REQUEST_TEMPLATE.md** - Pull request template

### Workflow Templates

Located in `.github/workflows/`, these appear as starter workflows when setting up GitHub Actions in any repository in the organization.

## How It Works

- Files here serve as organization-wide defaults
- Individual repositories can override by creating their own versions
- Default files are not included in repository clones or downloads
- This repository must be public for community health files to work organization-wide
- Workflow templates can work with internal/private repositories

## References

- [GitHub Docs: Creating default community health files](https://docs.github.com/en/communities/setting-up-your-project-for-healthy-contributions/creating-a-default-community-health-file)
- [GitHub Docs: Sharing actions and workflows](https://docs.github.com/en/actions/sharing-automations/sharing-actions-and-workflows-with-your-organization)
