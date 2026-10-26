# Youi (youi)

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

Youi is an Australian general insurance carrier headquartered at Sippy Downs on the Queensland Sunshine Coast, authorised by APRA and operating under AFSL 316511 (ABN 79 123 074 733). It is a wholly owned subsidiary of Youi Holdings Pty Ltd, part of OUTsurance International Holdings, with the OUTsurance Group as ultimate holding company. Youi writes personal and small-business property and casualty lines direct to consumers — car, NSW CTP Green Slip, SA CTP, motorcycle, caravan and trailer, watercraft, home building and contents, and small business cover — and is a member of the Insurance Council of Australia and a signatory to the General Insurance Code of Practice.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/youi/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/youi/refs/heads/main/apis.yml)

## Tags

- Insurance
- Australia
- Property and Casualty
- General Insurance
- Motor Insurance
- Home Insurance
- Business Insurance
- Compulsory Third Party
- Carrier
- Direct to Consumer
- No Public API

## Timestamps

- **Created:** 2026-07-25
- **Modified:** 2026-07-25

## APIs

**None.** Youi publishes no public API.

This is the honest, recorded outcome of a full probe on 2026-07-25, not a gap in research:

- **No developer portal.** `developer.youi.com.au`, `developers.youi.com.au`, `docs.youi.com.au` and `api.youi.com.au` do not resolve in DNS. `https://www.youi.com.au/developers`, `/api`, `/developer`, `/partners` and `/integrations` all return HTTP 404. The 618-URL public sitemap contains no developer, API or integration page — the only "partnership" pages are sports sponsorships.
- **The only portal is a customer login wall.** [portal.youi.com.au](https://portal.youi.com.au/) returns HTTP 200 but is a `noindex` Angular single-page app for policyholders, fronting an ASP.NET policy-manager login at `secure.youi.com.au`. Its own HTML declares a private backend at `portalapi.youi.com.au`, which returns HTTP 404 at root and serves no `swagger.json` or `openapi.json`. That is a first-party SPA backend, not a published API, and it is not listed as one.
- **No OpenAPI, Swagger, Postman, GraphQL, gRPC, webhooks or AsyncAPI** were found, so this repo has no `openapi/` directory.
- **ACORD posture: no ACORD reference found.** No ACORD, AL3, ACORD XML, NGDS or IVANS mention anywhere on the public site. Youi distributes direct to consumers rather than through brokers, so it has no agency-management-system download seam.
- **Quote / bind / issue / FNOL: none exposed programmatically.** Quoting and claims are consumer web and phone flows only.
- **Auth model:** none published. No OpenID Connect or OAuth discovery document is served; the only authentication is an end-customer session login.

Market context: Australia has the legal machinery for open insurance and no live obligation. APRA supervises prudentially, and the Consumer Data Right that already opened banking and energy was designated to extend to general insurance and then deferred and de-prioritised. No forcing function reaches a carrier like Youi.

> Not to be confused with **You.i TV / You.i Engine** (`youi.tv`), an unrelated Canadian software company that does publish developer documentation. Nothing from that company is recorded here.

## Artifacts

Enrichment round 2026-07-25 harvested everything Youi genuinely publishes:

- [`well-known/youi-security.txt`](well-known/youi-security.txt) — the live RFC 9116 document, PGP clear-signed, saved verbatim. Its `Expires` field (2024-01-25) has passed, so the only machine-readable artifact Youi serves is stale by its own terms.
- [`well-known/youi-well-known.yml`](well-known/youi-well-known.yml) — every `/.well-known/` probe across all four hosts. **Trap recorded:** `portal.youi.com.au` returns HTTP 200 for *any* path, including `/openapi.json` and every `/.well-known/*`, because the Angular SPA serves a catch-all route. Those 200s are `text/html` shells, not documents.
- [`security/youi-domain-security.yml`](security/youi-domain-security.yml) — TLS 1.3, HSTS (max-age 15552000), SPF and DMARC `p=reject`; no DNSSEC and no CAA records.
- [`security/youi-vulnerability-disclosure.yml`](security/youi-vulnerability-disclosure.yml) — policy URL and `security@youi.com` contact from the signed security.txt.
- [`conformance/youi-conformance.yml`](conformance/youi-conformance.yml) — negative on every API standard (OpenAPI, AsyncAPI, GraphQL, OAuth2, OIDC, RFC 9457, RFC 9727, ACORD, CDR), positive on RFC 9116, the General Insurance Code of Practice, APRA authorisation and Privacy Act 1988 APPs.
- [`packages/youi-packages.yml`](packages/youi-packages.yml) — zero first-party client libraries, with the npm/PyPI/GitHub-org probe log and the You.i TV disambiguation so a future round cannot mis-attribute `youi-cli` and friends.
- [`llms/youi-llms.txt`](llms/youi-llms.txt) — generated agent-facing summary that states plainly there is no API to call.

## Links

- [Website](https://www.youi.com.au/)
- [About Us](https://www.youi.com.au/about-us)
- [Customer Portal](https://portal.youi.com.au/) (login required)
- [security.txt](https://www.youi.com.au/.well-known/security.txt)
- [Security Vulnerability Disclosure Policy](https://www.youi.com.au/about-us/security-vulnerability-disclosure-policy)
- [Contact](https://www.youi.com.au/contact)
- [You Connect (news and stories)](https://www.youi.com.au/you-connect)

## Review

See [review.yml](review.yml) for the full probe log, HTTP statuses, ACORD posture, and transport findings.
