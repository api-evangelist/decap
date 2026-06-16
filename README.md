# Decap CMS (decap)

Decap CMS (formerly Netlify CMS) is an open-source, Git-based headless content management system for static site generators and modern frontend frameworks. It provides a web-based editorial UI for managing content stored directly in Git repositories, supporting collections of entries and media files, rich-text editing, editorial workflows (draft/review/publish), and i18n. Content operations are proxied to Git hosting backends (GitHub, GitLab, Bitbucket, Azure, Gitea) via their respective REST and GraphQL APIs. Decap Turbo adds a managed cloud layer with a database proxy, centralized authentication, user roles, real-time collaboration presence, and priority support.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/decap/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/decap/refs/heads/main/apis.yml)

## Tags

- CMS
- Headless CMS
- Git-based CMS
- Content Management
- Static Site Generator
- JAMstack
- Open Source
- Editorial Workflow

## Timestamps

- **Created:** 2026-06-13
- **Modified:** 2026-06-13

## APIs

### Decap CMS Git Backend API

Decap CMS communicates with Git hosting providers (GitHub, GitLab, Bitbucket, Azure, Gitea) through their REST and GraphQL APIs to read, create, update, and delete content entries, manage media file uploads, and orchestrate editorial workflows. The Decap client library wraps these provider APIs; there is no standalone Decap REST API server — all operations pass through the configured backend. Decap Turbo augments this with a database proxy that caches content and reduces direct Git API round-trips for improved performance and reduced rate-limit exposure.

- **Human URL:** [https://decapcms.org/docs/intro/](https://decapcms.org/docs/intro/)
- **Base URL:** `https://api.github.com`

#### Tags

- Content Management
- Git Backend
- Editorial Workflow
- Media Management

#### Properties

- [Documentation](https://decapcms.org/docs/intro/)
- [Backends Overview](https://decapcms.org/docs/backends-overview/)
- [Git Hub Backend](https://decapcms.org/docs/github-backend/)
- [Git Lab Backend](https://decapcms.org/docs/gitlab-backend/)
- [Git Gateway Backend](https://decapcms.org/docs/git-gateway-backend/)
- [Collections](https://decapcms.org/docs/collection-types/)
- [Widgets](https://decapcms.org/docs/widgets/)
- [Editorial Workflow](https://decapcms.org/docs/configuration-options/#publish-mode)
- [Media Library](https://decapcms.org/docs/media-library/)
- [Authentication](https://decapcms.org/docs/authentication-backends/)
- [Changelog](https://github.com/decaporg/decap-cms/releases)
- [Graph Q L](graphql/decap-graphql.md)

## Common Properties

- [Website](https://decapcms.org/)
- [Documentation](https://decapcms.org/docs/)
- [Git Hub Org](https://github.com/decaporg)
- [Blog](https://decapcms.org/blog/)
- [Pricing](https://decapcms.org/turbo/)
- [X (Twitter)](https://x.com/Decap_CMS)
- [Plans](plans/decap-plans-pricing.yml)
- [Rate Limits](rate-limits/decap-rate-limits.yml)
- [Fin Ops](finops/decap-finops.yml)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
