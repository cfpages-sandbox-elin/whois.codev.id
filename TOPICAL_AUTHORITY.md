# Topical Authority — whois.codev.id

## Role and boundary

`whois.codev.id` is a specialist Indonesian knowledge and utility-support property for understanding domain-registration data through WHOIS, RDAP, registry, registrar, DNS, and lifecycle evidence. It should help domain owners, buyers, developers, security teams, and researchers query records, interpret uncertainty, and choose safe next steps. The existing web interface and API own live single/bulk lookup intent; articles explain concepts and verification workflows without asserting ownership, availability, legality, value, or purchase suitability from one response. Registry/RDAP/WHOIS freshness, domain availability and status, privacy and security claims, dates, prices, legal conclusions, and current registrar/registry/provider policies must be time-stamped, cross-checked against authoritative current sources, and reviewed by a qualified professional where legal or security risk warrants it.

## Context used

- The repository exposes 2 static HTML routes: the lookup interface and API documentation. It contains no sitemap or existing editorial route family.
- Visible homepage headings are “Who Dat?,” “WHOIS Lookup,” “Results,” “Public API,” and “Self-Hosting.”
- The form accepts one domain and can show formatted or raw results.
- Three handler families are tracked: single-domain lookup, bulk lookup via `/multi`, and health checking via `/ping`.
- Every otherwise unmatched root path is treated as a single-domain lookup. Planned articles therefore require a dedicated `/panduan/<slug>/` filesystem namespace; publishing them as `/<slug>/` would collide with API intent.
- Homepage and project evidence describe a free, open-source WHOIS lookup service with a public API and self-hosting option; those provider and availability claims require current verification before publication.

## Ignored template noise

- No sitemap, article, archive, tag, author, pagination, feed, or location-swapped route families exist.
- Eleven tracked style, icon, and image assets plus framework, build, workflow, contributor, sponsor, and deployment boilerplate were not treated as editorial coverage.
- API examples, generated response bodies, and repeated WHOIS field values were not audited as a corpus.
- A lookup result is treated as a time-bound observation, not proof that a domain is available, transferable, legally unencumbered, or owned by a named party.

## Topical map

| Topic ID | Parent topic | Reader outcome | Boundary | Article target |
|---|---|---|---|---:|
| WHO-01 | Dasar nama domain dan registrasi | Understand domain hierarchy, registration actors, identifiers, and the limits of public lookup data. | Owns foundational vocabulary; record protocols belong to WHO-02 and party roles to WHO-06. | 6 |
| WHO-02 | WHOIS, RDAP, dan sumber data | Distinguish protocols, authoritative sources, output formats, coverage, and transition issues. | Owns source/protocol comparison; field interpretation belongs to WHO-03 and freshness disputes to WHO-15. | 6 |
| WHO-03 | Cara lookup dan membaca hasil | Query safely, normalize a domain, and interpret common fields, missing values, and raw output. | Owns lookup literacy; availability decisions belong to WHO-04 and API automation to WHO-14. | 6 |
| WHO-04 | Availability dan status pendaftaran | Evaluate whether a domain may be registered, reserved, premium, blocked, pending, or merely unresolved. | Owns availability verification; EPP operational statuses belong to WHO-07 and acquisition pricing to WHO-13. | 6 |
| WHO-05 | Tanggal dan lifecycle domain | Understand creation, update, expiry, renewal, grace, redemption, deletion, and release uncertainty. | Owns lifecycle timing; transfer processes belong to WHO-11 and monitoring workflows to WHO-16. | 6 |
| WHO-06 | Registry, registrar, reseller, dan registrant | Identify which party operates the TLD, sells the registration, manages the account, and holds rights. | Owns actor responsibilities; provider due diligence belongs to WHO-13 and privacy disclosure to WHO-09. | 6 |
| WHO-07 | Kode status EPP dan domain lock | Interpret transfer, update, delete, hold, pending, and server/client status codes. | Owns status-code meaning; security response belongs to WHO-12 and lifecycle dates to WHO-05. | 6 |
| WHO-08 | Nameserver, DNS, glue, dan DNSSEC | Connect registration records to delegation, resolution, child nameservers, and validation. | Owns registration-to-DNS evidence; ownership/availability belongs to WHO-04 and incident security to WHO-12. | 6 |
| WHO-09 | Privasi, redaksi, dan data kontak | Understand redacted fields, privacy/proxy services, disclosure limits, and safe handling of personal data. | Owns privacy and contact-data boundaries; legal disputes belong to WHO-13 and abuse/security reporting to WHO-12. | 6 |
| WHO-10 | TLD, ccTLD, dan domain internasional | Account for registry-specific policy, local extensions, IDN/Punycode, and unsupported lookup behavior. | Owns namespace differences; provider roles belong to WHO-06 and protocol coverage to WHO-02. | 6 |
| WHO-11 | Transfer dan perubahan pengelolaan domain | Prepare registrar transfers, registrant changes, authorization, locks, timing, and post-transfer checks. | Owns operational transfer workflow; domain acquisition negotiation belongs to WHO-13 and security controls to WHO-12. | 6 |
| WHO-12 | Keamanan domain, abuse, dan hijacking | Detect suspicious changes, harden accounts, preserve evidence, and escalate incidents safely. | Owns security prevention and response; privacy policy belongs to WHO-09 and routine monitoring to WHO-16. | 6 |
| WHO-13 | Akuisisi, harga, merek, dan due diligence | Verify domain identity, seller authority, transaction process, price evidence, trademarks, and contractual risk. | Owns acquisition decision support without valuation or legal conclusions; availability belongs to WHO-04. | 6 |
| WHO-14 | API WHOIS/RDAP dan otomasi bulk | Use single/bulk endpoints responsibly with validation, limits, caching, authentication, and error handling. | Owns programmatic access; manual lookup interpretation belongs to WHO-03 and portfolio monitoring to WHO-16. | 6 |
| WHO-15 | Freshness, konflik, dan kualitas data | Resolve stale, missing, inconsistent, rate-limited, or differently formatted records through source-aware checks. | Owns evidence-quality incidents; protocol basics belong to WHO-02 and API engineering to WHO-14. | 6 |
| WHO-16 | Monitoring portofolio domain | Track expiry, status, registrar, DNS, and security changes with ownership, alerts, and verification. | Owns ongoing portfolio operations; lifecycle mechanics belong to WHO-05 and incident response to WHO-12. | 6 |

## Internal-link rule

Every article publishes under `/panduan/<slug>/` and links upward to its WHO topic hub; root-level `/<slug>/` publication is prohibited because the catch-all owns lookup intent. WHO-01 routes readers to protocol/data sources (WHO-02/WHO-03), lifecycle evidence (WHO-04–WHO-07), DNS/privacy/security (WHO-08–WHO-12), and acquisition or operational workflows (WHO-13–WHO-16). Lookup guides link to freshness and discrepancy checks before stating a conclusion. Availability, acquisition, or transfer content always links to registry/registrar verification, dates/status, privacy/security, and the relevant live lookup route; no article treats an empty response as permission to register or buy.

## First publication wave

Publish a coherent 12-asset evidence foundation: `WHO-01-01`, `WHO-01-02`, `WHO-02-01`, `WHO-02-02`, `WHO-03-01`, `WHO-03-02`, `WHO-04-01`, `WHO-05-01`, `WHO-06-01`, `WHO-07-01`, `WHO-09-01`, and `WHO-15-01`. This wave establishes the domain-registration model, separates WHOIS from RDAP, teaches safe query and field reading, prevents false availability conclusions, and makes freshness, actor, status, and privacy limitations explicit before operational clusters expand.
