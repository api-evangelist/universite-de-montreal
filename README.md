# Université de Montréal (universite-de-montreal)

<!-- API-EVANGELIST-PROVENANCE:BEGIN -->
> ### About this repository
>
> **This is not our API.** This repository is an independent, third-party profile of a company's
> **publicly available** API surface, maintained by [API Evangelist](https://apievangelist.com).
> API Evangelist does not operate, host, resell, or support this company's APIs, and is not
> affiliated with or endorsed by the company unless stated on the profile.
>
> **Where the information came from.** Everything here is assembled from material a member of the
> public can reach with a browser and no credentials — the company's own website, developer portal
> and documentation, the specifications it publishes for public use (OpenAPI, AsyncAPI, JSON Schema,
> `apis.json`, `llms.txt` and similar), its public repositories, and its public status, pricing and
> changelog pages. **Nothing here is obtained by breaching a system, defeating an access control, or
> using credentials of any kind.**
>
> **The rating is an independent assessment.** The Kin Score and Agent Readiness rating are
> independently calculated scores of a company's *public* API artifacts, produced by API Evangelist
> against a published rubric. They are not certifications, endorsements, security assessments, or
> audits, and they score published artifacts — not the quality, safety, or security of the software.
>
> **Corrections, re-scores, and removal are free.** No partnership, contract, or purchase is
> required, and you do not need to justify the request.
>
> - **Something wrong?** Open an issue on this repository, or email
>   [info@apievangelist.com](mailto:info@apievangelist.com).
> - **Published something new?** Ask for a re-score and we will re-run the rating.
> - **Want the listing taken down?** Say so and we will honor it. The profile is reduced to your
>   company name, a factual description, and a link to your own site, and the company is recorded as
>   **unrated** — never scored zero for having asked.
>
> **Response times.** Acknowledgement within **one business day**; removal or restriction within
> **two business days**; corrections and re-scores within **five business days**.
>
> **Not from the company, and here with a question?** You are welcome here — we would rather be the
> front line and point you the right way than have a good report go nowhere. What this repository
> can answer is narrow, though, so it is worth knowing who you are actually looking for:
>
> - **A question about how the API works, an account, billing, or a bug in the service** — that is
>   the company's own support, not us. We profile this API; we do not operate it and cannot see
>   your account.
> - **A bug in an open-source project we only catalog** — file it on that project's own repository.
>   This has happened with a real and correct bug report that reached us instead of the people who
>   could fix it, which helped nobody.
> - **Anything about this listing itself** — the description, the tags, the rating, a missing or
>   wrong artifact — is ours. Open an issue here.
> - **Not sure, or something general about API Evangelist or APIs.io** — open an issue on the
>   [APIs.io Inbox](https://github.com/api-search/inbox) and we will route it.
>
> **This repository contains no software, and we will never ask you to download anything.** There is
> no build, release, installer, or binary here — only text and machine-readable API descriptions, so
> there is nothing here that can be "corrupt" or need "repairing". Any issue, comment, or email
> claiming otherwise and offering a download link is not from us and is hostile. Do not follow the
> link; it is a lure. Report it to GitHub and, if you like, tell us at
> [info@apievangelist.com](mailto:info@apievangelist.com) so we can take it down.
>
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

Université de Montréal (UdeM) is a leading French-language public research university in Montréal, Québec, Canada, ranked #95 in the QS World University Rankings 2025. This repository catalogs UdeM's public, machine-readable developer and API footprint as an APIs.json provider profile. That footprint is modest and research/library oriented — there is no single unified developer portal — and is captured here without fabricating any endpoints.

- APIs.json: https://raw.githubusercontent.com/api-evangelist/universite-de-montreal/refs/heads/main/apis.yml
- Run with Naftiko: https://github.com/naftiko/fleet?utm_source=api-evangelist&utm_medium=readme&utm_campaign=universite-de-montreal-api-evangelist&utm_content=repo

## Type

- Type: Index
- Position: Consumer
- Access: 3rd-Party

## Tags

University, Higher Education, Education, Canada, Québec, French Language, U15, Public Research University, Research, Research Data, Research Expertise, Identity Federation, Institutional Repository, Library, Open Access, OAI-PMH, Shibboleth, SAML

## APIs

Every surface carries an `x-operator` in `apis.yml`. A university is a federation of buyers, so
who *operates* a surface matters more than whether a spec exists for it.

**Institution-operated (2)**

- **SADVR REST API (Vitrine-Recherche)** — `x-operator: institution`. UdeM's own read-only research
  API, built by its Centre d'expertise numérique pour la recherche. Faculties, departments, job
  titles, programmes, disciplines, research-expertise keywords, and UdeM's own persistent
  identifiers (idsadvr) for 3,516 researchers and 429 research units. No API key. GET only.
  Base: https://www.recherche.umontreal.ca/vitrine/rest/api/1.8/umontreal —
  Docs: https://wiki.umontreal.ca/spaces/DOC/pages/294781211/API+REST+%E2%80%93+Description+technique —
  Contract: [openapi/universite-de-montreal-sadvr-openapi.yml](openapi/universite-de-montreal-sadvr-openapi.yml)
- **UdeM Shibboleth Identity Provider** — `x-operator: institution`. SAML 2.0 entity metadata
  published under the institution's own domain, scope `umontreal.ca`.
  Metadata: https://shibboleth.umontreal.ca/idp/shibboleth

**Tenancies (4)** — UdeM's data, someone else's contract. Recorded as relationships; the vendor's
spec is deliberately *not* saved here.

- **PAPYRUS OAI-PMH** — `x-operator: tenant`. Scholaris (CRKN-hosted DSpace). 18 metadata prefixes.
  Base: https://umontreal.scholaris.ca/server/oai/request
- **PAPYRUS DSpace REST (HAL)** — `x-operator: tenant`. Base: https://umontreal.scholaris.ca/server/api
- **Borealis Dataverse — UdeM collection** — `x-operator: tenant`. Collection 75123, 452 datasets
  with DataCite DOIs under 10.5683, on the shared national instance operated by Scholars Portal.
  Docs: https://borealisdata.ca/dataverse/montreal
- **WorldCat Discovery** — `x-operator: tenant`. OCLC. https://umontreal.on.worldcat.org/discovery

## Plans / Rate Limits / FinOps

- Plans & Pricing: [plans/universite-de-montreal-plans-pricing.yml](plans/universite-de-montreal-plans-pricing.yml)
- Rate Limits: [rate-limits/universite-de-montreal-rate-limits.yml](rate-limits/universite-de-montreal-rate-limits.yml)
- FinOps: [finops/universite-de-montreal-finops.yml](finops/universite-de-montreal-finops.yml)

## Timestamps

- Created: 2026-06-03
- Modified: 2026-08-30

## Common Properties

- Website: https://www.umontreal.ca/en/
- GitHub: https://github.com/bibudem (official UdeM Libraries org)
- LinkedIn: https://www.linkedin.com/school/universite-de-montreal/
- Review: [review.yml](review.yml)

## Notes

**2026-08-30 — re-profiled under the university pipeline. This was a correction, and it lowered the
apparent footprint on purpose.**

- This repo previously held **36 OpenAPI documents and 38 `apis[]` entries**. All 36 were the
  **Dataverse product's own contract** — a title five to eight other institutions in this cohort
  also ship — harvested from the shared Borealis instance and then re-based by our own
  `refine-openapis` step onto `umontreal.scholaris.ca`, a DSpace host that does not serve the
  Dataverse API at all. The 36 specs and the 88 artifacts derived from them were removed file by
  file. The Borealis relationship is retained as a single tenant entry.
- **The SADVR API was recorded as dead. It is not.** UdeM's own documentation gives an example URL
  reading `ressource/langues`; the deployment serves the singular `ressource/langue`. That one
  character, plus an undocumented HTML 404 where the docs promise a JSON error, produced a false
  "testing/legacy endpoint" verdict in June 2026. Fifteen documented routes were re-probed on
  2026-08-30 and returned 200 `application/json`. The `baseURL` is now recorded.
- **New find: UdeM's Shibboleth Identity Provider.** Live SAML 2.0 entity metadata under the
  institution's own domain, plus a 200 `/idp/status` operational report. Institution-operated by
  definition, machine-readable, and absent from the June profile.
- The documented SADVR base *itself* returns 404 — the API exposes no root resource. Every route
  beneath it answers. A pointer grader reading only the base will under-grade this surface.
- `api.umontreal.ca` resolves (132.204.8.11) and answers **HTTP 400 with an empty body** on every
  anonymous path, and is named in no documentation. Recorded as evidence of an internal gateway,
  **not** as an API.
- SADVR serves researcher names, institutional emails, phone numbers and office locations with **no
  credential and no rate limit**. Its `consentement` / `exclusion` flags are the only control, and
  they are advisory to the consumer. Example payloads in this repo are drawn only from the
  non-personal reference endpoints.
- No developer portal, no open-data portal, no OAuth authorization server, no status page, no
  `llms.txt`, no ORCID cross-walk.
- The LinkedIn school page returns HTTP 999 — LinkedIn's bot-block, graded live, not absent.
- No endpoints, API keys, or base URLs were invented; only confirmed public resources are listed.

## Maintainers

- Kin Lane — kin@apievangelist.com
