# Decap CMS GraphQL API

Decap CMS (formerly Netlify CMS) is a Git-based headless CMS that does not expose a native GraphQL API of its own. All content operations are performed by the client-side JavaScript library communicating directly with the configured Git hosting backend (GitHub, GitLab, Bitbucket, Azure DevOps, or Gitea) through those providers' own REST and GraphQL APIs. There is no standalone Decap API server or GraphQL endpoint.

**Endpoint:** REST API only — see `decap-schema.graphql` for the conceptual data model schema

**Documentation:** https://decapcms.org/docs/

## How Decap CMS Works

Decap CMS runs entirely in the browser. When an editor saves content, the library:

1. Serializes the entry to Markdown (or JSON/YAML/TOML front matter, depending on configuration)
2. Commits the file to the Git repository via the backend provider's API
3. Optionally creates a pull/merge request for editorial workflow review

The GitHub backend uses the GitHub GraphQL API (`https://api.github.com/graphql`) for some operations (such as fetching file trees efficiently), but that GraphQL interface belongs to GitHub, not Decap CMS.

## Decap Turbo (Managed Cloud Layer)

Decap Turbo is a commercial add-on that introduces a database proxy cache in front of the Git backend, centralizes authentication, adds user roles, and provides real-time collaboration presence. The proxy communicates with Git backends over their native APIs. No public GraphQL endpoint for the Turbo proxy has been documented.

**References:**
- Documentation: https://decapcms.org/docs/intro/
- Backends Overview: https://decapcms.org/docs/backends-overview/
- GitHub Backend: https://decapcms.org/docs/github-backend/
- GitLab Backend: https://decapcms.org/docs/gitlab-backend/
- Configuration Options: https://decapcms.org/docs/configuration-options/
- Collection Types: https://decapcms.org/docs/collection-types/
- Widgets Reference: https://decapcms.org/docs/widgets/
- GitHub Repository: https://github.com/decaporg/decap-cms
- Decap Turbo: https://decapcms.org/turbo/
