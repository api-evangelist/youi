# Youi (youi)

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
