# Université de Montréal (universite-de-montreal)

Université de Montréal (UdeM) is a leading French-language public research university in Montréal, Québec, Canada, ranked #95 in the QS World University Rankings 2025. This repository catalogs UdeM's public, machine-readable developer and API footprint as an APIs.json provider profile. That footprint is modest and research/library oriented — there is no single unified developer portal — and is captured here without fabricating any endpoints.

- APIs.json: https://raw.githubusercontent.com/api-evangelist/universite-de-montreal/refs/heads/main/apis.yml
- Run with Naftiko: https://github.com/naftiko/fleet?utm_source=api-evangelist&utm_medium=readme&utm_campaign=universite-de-montreal-api-evangelist&utm_content=repo

## Type

- Type: Index
- Position: Consumer
- Access: 3rd-Party

## Tags

Education, Higher Education, University, Research, Open Data, Library, Canada, Québec

## APIs

- SADVR REST API (Vitrine-Recherche) — research data redistribution (resource exposure, persistent identifier search, data retrieval, SOLR search). Docs: https://wiki.umontreal.ca/spaces/DOC/pages/294781211/API+REST+%E2%80%93+Description+technique
- Papyrus OAI-PMH Endpoint — OAI-PMH 2.0 metadata harvesting for the UdeM institutional repository. Docs: https://papyrus.bib.umontreal.ca/ — Base: https://umontreal.scholaris.ca/server/oai/openaire4
- UdeM Borealis Dataverse — research data collection in the Canadian Dataverse Repository (native Dataverse REST API). Docs: https://borealisdata.ca/dataverse/montreal

## Plans / Rate Limits / FinOps

- Plans & Pricing: [plans/universite-de-montreal-plans-pricing.yml](plans/universite-de-montreal-plans-pricing.yml)
- Rate Limits: [rate-limits/universite-de-montreal-rate-limits.yml](rate-limits/universite-de-montreal-rate-limits.yml)
- FinOps: [finops/universite-de-montreal-finops.yml](finops/universite-de-montreal-finops.yml)

## Timestamps

- Created: 2026-06-03
- Modified: 2026-06-03

## Common Properties

- Website: https://www.umontreal.ca/en/
- GitHub: https://github.com/bibudem (official UdeM Libraries org)
- LinkedIn: https://www.linkedin.com/school/universite-de-montreal/
- Review: [review.yml](review.yml)

## Notes

- The Papyrus OAI-PMH endpoint was probed live and returns a valid OAI-PMH 2.0 Identify response.
- The SADVR REST API documentation page is live (HTTP 200), but its documented base path (`https://www.recherche.umontreal.ca/vitrine/rest/api/1.8/umontreal/`) returns HTTP 404 and appears to be a testing/legacy endpoint; the `baseURL` is therefore intentionally omitted from apis.yml.
- UdeM participates in Borealis (Canadian Dataverse) rather than hosting its own Dataverse instance.
- The LinkedIn school page returns HTTP 999, which is LinkedIn's standard bot-block and not an indication the page is absent.
- No endpoints, API keys, or base URLs were invented; only confirmed public resources are listed.

## Maintainers

- Kin Lane — kin@apievangelist.com
