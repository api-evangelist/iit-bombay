# Indian Institute of Technology Bombay (iit-bombay)

Indian Institute of Technology Bombay (IIT Bombay), founded in 1958 in Powai, Mumbai, is one of India's premier engineering and research institutions, ranked #97 in the QS World University Rankings 2025. This repository catalogs its public developer/API footprint as an [APIs.json](https://apisjson.org) profile. IIT Bombay has no central institutional developer portal; its public API surface is community- and library-driven.

- APIs.json: https://raw.githubusercontent.com/api-evangelist/iit-bombay/refs/heads/main/apis.yml
- Run with Naftiko: https://github.com/naftiko/fleet?utm_source=api-evangelist&utm_medium=readme&utm_campaign=iit-bombay-api-evangelist&utm_content=repo

## Type

- Index
- Consumer
- 3rd-Party

## Tags

Education, Higher Education, University, Research, India, Open Access, Identity

## APIs

- **Gymkhana Profiles OAuth API** — OAuth 2.0 (RFC 6749) identity/profile API run by the Students' Gymkhana; authorize, token, revoke, and user-resource endpoints. Gated to IIT Bombay server infrastructure. Docs: https://gymkhana.iitb.ac.in/profiles/doc/
- **ITC Single Sign-On API** — Session-based SSO from the Institute Technical Council; redirect ssocall flow plus a getuserdata exchange returning user profile fields. Docs: https://sso.tech-iitb.org/docs/
- **DSpace Institutional Repository OAI-PMH** — Live OAI-PMH 2.0 metadata-harvesting interface over the Central Library DSpace repository. Endpoint: https://dspace.library.iitb.ac.in/oai/request?verb=Identify | Repository: https://dspace.library.iitb.ac.in/

## Plans, Rate Limits, and FinOps

- Plans / Pricing: [plans/iit-bombay-plans-pricing.yml](plans/iit-bombay-plans-pricing.yml)
- Rate Limits: [rate-limits/iit-bombay-rate-limits.yml](rate-limits/iit-bombay-rate-limits.yml)
- FinOps: [finops/iit-bombay-finops.yml](finops/iit-bombay-finops.yml)

## Timestamps

- Created: 2026-06-03
- Modified: 2026-06-03

## Common Properties

- Website: https://www.iitb.ac.in/
- GitHub: https://github.com/DevCom-IITB
- LinkedIn: https://www.linkedin.com/school/indian-institute-of-technology-bombay/
- Review: [review.yml](review.yml)

## Notes

All documentation pages and the OAI-PMH Identify endpoint were probed live and returned HTTP 200; the OAI-PMH response was verified as valid OAI-PMH 2.0. No endpoints were fabricated. The Gymkhana Profiles API is explicitly restricted to applications running on IIT Bombay Students' Gymkhana server infrastructure. LinkedIn returned HTTP 999 (its standard automated-request block); the school page exists. No central, institution-wide developer portal or open-data portal was found.

## Maintainers

- Kin Lane — kin@apievangelist.com
