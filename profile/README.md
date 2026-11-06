# analytics-os

The studio's own analytics and tracking-data pipelines for [Caldrion Ventures](https://ventures.caldrion.com), the venture studio that identifies opportunities, validates concepts and incubates businesses through launch and growth.

Part of the Caldrion (studio platform) portfolio.

- Website: https://ventures.caldrion.com
- Project board: [Caldrion · Analytics OS](https://github.com/orgs/analytics-os/projects/1) · Portfolio: [Portfolio · Caldrion](https://github.com/orgs/caldrion-com/projects/14)
- Parent organization: [Caldrion](https://www.caldrion.com)

## What we build

Each pipeline pulls a third-party data source into **our own** Cloudflare D1 + R2 every day, so history keeps accumulating beyond the source's own retention window and can be joined across sources.

| Product | What it does | Repository | Live |
| --- | --- | --- | --- |
| Search Console warehouse | All Google Search Console data (Search Analytics, sitemaps, URL Inspection) for the studio's sites, pulled daily (Cloudflare Worker + Workflow) | [search-console](https://github.com/analytics-os/search-console) (private) | https://search-console.caldrion.workers.dev |
| SEO warehouse | Semrush data from rotating 7-day trials, kept in D1 + R2 keyed by trial (Hono + TypeScript Worker, Workflows) | [seo-warehouse](https://github.com/analytics-os/seo-warehouse) (private) | https://seo-warehouse.caldrion.workers.dev |

## How we work

- **Issues first.** Every change starts from an issue opened with one of the org-wide issue forms: Bug, Feature, Task, Epic or Initiative.
- **Hierarchy.** Work is organized with issue types and sub-issues: **Initiative** (a portfolio-level outcome spanning a quarter or more) > **Epic** (a shippable body of work) > **Feature / Task / Bug**.
- **Project boards.** Issues and pull requests are tracked on GitHub Projects with a standard Status flow (Backlog, Ready, In progress, In review, Done), plus Priority (P0–P3), Size (XS–XL) and two-week iterations.
- **Labels.** Triage labels (`needs-triage`, `needs-info`, `blocked`) plus `platform:*` and `area:*` labels per repository. Types are not duplicated as labels.
- **Pull requests.** Use the pull request template and link the issue with `Closes #<n>` so it moves to Done on merge.

## Contact

- General: https://ventures.caldrion.com/contact
- Security: please report vulnerabilities privately through [www.caldrion.com/contact](https://www.caldrion.com/contact) (the contact in [caldrion.com's security.txt](https://www.caldrion.com/.well-known/security.txt)) rather than in a public issue; see our [security policy](https://github.com/analytics-os/.github/blob/main/SECURITY.md).
