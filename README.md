# Indian Institute of Technology Bombay (iit-bombay)

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

Indian Institute of Technology Bombay (IIT Bombay), founded in 1958 in Powai, Mumbai, is one of India's premier engineering and research institutions, ranked #97 in the QS World University Rankings 2025. This repository catalogs its public developer/API footprint as an [APIs.json](https://apisjson.org) profile. IIT Bombay has no central institutional developer portal; its public API surface is community- and library-driven.

- APIs.json: https://raw.githubusercontent.com/api-evangelist/iit-bombay/refs/heads/main/apis.yml
- Run with Naftiko: https://github.com/naftiko/fleet?utm_source=api-evangelist&utm_medium=readme&utm_campaign=iit-bombay-api-evangelist&utm_content=repo

## Type

- Index
- Consumer
- 3rd-Party

## Tags

University, Higher Education, Education, India, Institute of Technology, Research, Identity, Single Sign-On, OpenID Connect, Campus Life, Research Repository, Open Source

## APIs

Every surface carries an `x-operator` — who actually runs the thing, which for a university is
rarely the same answer as whose name is on it.

- **InstiApp API** — `x-operator: institution`. IIT Bombay's campus-life API and its largest
  first-party programmable surface: 112 paths / 164 operations over student bodies (154 live),
  events and calendar, news, hostel mess menus (22), 427 named campus-map locations, a public
  grievance register, marketplace, lost-and-found, achievements, and placement/internship blogs.
  A substantial read surface answers with no credential. Autogenerated OpenAPI served live at
  https://gymkhana.iitb.ac.in/instiapp/api/docs/ | Base: https://gymkhana.iitb.ac.in/instiapp/api |
  Source: https://github.com/DevCom-IITB/instiapp-api (AGPL-3.0)
- **IITB Central SSO — OpenID Connect** — `x-operator: institution`. The Computer Centre's central
  identity provider, publishing a live OpenID Connect Discovery 1.0 document and JWKS. Issuer:
  https://sso.iitb.ac.in | Discovery:
  https://sso.iitb.ac.in/.well-known/openid-configuration
- **Gymkhana Profiles OAuth API** — `x-operator: institution`. OAuth 2.0 (RFC 6749) identity and
  profile API run by the Students' Gymkhana, with ten separately-consented scopes. Access is
  restricted by policy to applications running on Gymkhana server infrastructure. Docs:
  https://gymkhana.iitb.ac.in/profiles/doc/
- **DSpace Institutional Repository (Central Library)** — `x-operator: institution`. DSpace over
  theses, articles and conference papers. Its OAI-PMH endpoint is **not currently verifiable**:
  https://dspace.library.iitb.ac.in/oai/request returns 403 at the Apache layer, and
  /xmlui/OAI/request returns a 200 with an empty body. The June 2026 claim that the Identify verb
  returned a valid OAI-PMH 2.0 response has been withdrawn. Repository:
  https://dspace.library.iitb.ac.in/
- **ITC Single Sign-On** — `x-operator: tenant`. Session-based SSO from the Institute Technical
  Council, an IIT Bombay student body — but on tech-iitb.org, registered in 2024 through Hostinger
  and not an institution-owned domain. The relationship is recorded; the engineering is not
  credited to the institution. Docs: https://sso.tech-iitb.org/docs/

## Plans, Rate Limits, and FinOps

- Plans / Pricing: [plans/iit-bombay-plans-pricing.yml](plans/iit-bombay-plans-pricing.yml)
- Rate Limits: [rate-limits/iit-bombay-rate-limits.yml](rate-limits/iit-bombay-rate-limits.yml)
- FinOps: [finops/iit-bombay-finops.yml](finops/iit-bombay-finops.yml)

## Timestamps

- Created: 2026-06-03
- Modified: 2026-08-30

## Common Properties

- Website: https://www.iitb.ac.in/
- API Reference: https://gymkhana.iitb.ac.in/instiapp/api/docs/
- Documentation: https://gymkhana.iitb.ac.in/profiles/doc/
- Identity Federation: https://sso.iitb.ac.in/.well-known/openid-configuration
- Research Repository: https://dspace.library.iitb.ac.in/
- Library: https://www.library.iitb.ac.in/
- Course Catalog (SSO-gated): https://asc.iitb.ac.in/
- GitHub: https://github.com/DevCom-IITB
- Support: https://github.com/DevCom-IITB/instiapp-api/issues
- Terms: https://www.iitb.ac.in/credits-disclaimer
- LinkedIn: https://www.linkedin.com/school/indian-institute-of-technology-bombay/
- Review: [review.yml](review.yml)

## Artifacts

- OpenAPI: [openapi/iit-bombay-instiapp-api-openapi.yml](openapi/iit-bombay-instiapp-api-openapi.yml)
  (pristine as published: [openapi/_original/iit-bombay-instiapp-api-openapi.json](openapi/_original/iit-bombay-instiapp-api-openapi.json))
- JSON Schema: [json-schema/iit-bombay-instiapp-schemas.json](json-schema/iit-bombay-instiapp-schemas.json)
- Examples (probed live): [examples/iit-bombay-instiapp-examples.yml](examples/iit-bombay-instiapp-examples.yml)
- Authentication: [authentication/iit-bombay-authentication.yml](authentication/iit-bombay-authentication.yml)
- Scopes: [scopes/iit-bombay-scopes.yml](scopes/iit-bombay-scopes.yml)
- Errors: [errors/iit-bombay-problem-types.yml](errors/iit-bombay-problem-types.yml)
- Conformance: [conformance/iit-bombay-conformance.yml](conformance/iit-bombay-conformance.yml)
- Vocabulary: [vocabulary/iit-bombay-vocabulary.yml](vocabulary/iit-bombay-vocabulary.yml)
- Rules: [rules/iit-bombay-rules.yml](rules/iit-bombay-rules.yml)
- Lifecycle: [lifecycle/iit-bombay-lifecycle.yml](lifecycle/iit-bombay-lifecycle.yml)

## Notes

Re-profiled 2026-08-30 under the API Evangelist university pipeline, which settles **who operates
each surface** before saving anything. IIT Bombay is one of the few universities in this catalog
with a genuine first-party API: the InstiApp specification is served from the institution's own
host, names an institutional contact (devcom@iitb.ac.in), and its implementation is published
under AGPL-3.0. No vendor contract (Figshare, Pure, Ex Libris, Dataverse, Symplectic) was found
attributed to this institution, and none was added.

What IIT Bombay does **not** publish is stated rather than padded: no central developer portal, no
course-catalog or registrar API (asc.iitb.ac.in is an SSO + hCaptcha gate), no open-data portal
(data.iitb.ac.in does not resolve), no research-computing surface (hpc./spacetime. do not resolve),
no library discovery API (opac.library.iitb.ac.in returns 502), no `llms.txt` or `security.txt`,
and no discoverable AI policy. Nine of the twelve education-regime domain standards produce no
evidence at all.

Two corrections against the June 2026 profile: the DSpace OAI-PMH liveness claim is withdrawn
(403 at the Apache layer; a 200-with-empty-body soft-200 on the /xmlui path would have read as
live on status alone), and the ITC SSO surface is relabelled from institution to tenant.

## Maintainers

- Kin Lane — kin@apievangelist.com
