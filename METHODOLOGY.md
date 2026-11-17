# KYB Compass methodology

Edition November 2026 (`2026-11`). The same rules apply to every ranked provider, SONAR (the publisher) included.

## Where the facts come from

- Only each provider’s own product, pricing, documentation and legal pages, opened on the date in `checked_on` and listed in `source_urls`. No review sites, analyst reports, blogs or sales calls, and no paid sign-ups.
- “Not stated” (`unknown`) means the pages opened do not say; it is not a claim that the feature is missing.
- Prices are before VAT. Euro amounts use the ECB euro reference rates of 2026-11-16 (1 EUR = 0.8345 GBP = 1.1014 USD).
- Cost of 5 checks = 5 x the published price per check, or the monthly plan that includes 5 checks; `cost_5_checks_from` marks a starting price.
- Each edition re-opens every source. A fact found wrong after publication is corrected in the same edition and listed in [CHANGELOG.md](CHANGELOG.md).

## Who is ranked

Providers that sell a business check (kinds `kyb`, `kyc-kyb`, `credit-kyb`): 43 in this edition. Company data tools (`data`) and screening-only tools (`screening`) are listed with `ranked: false`, not ranked. Providers looked at and left out, with the reason:

- Entrust Identity Verification (formerly Onfido) (https://www.entrust.com/products/identity-verification): Verifies people; no business verification on its pages.
- Experian Business Express (https://www.experian.co.uk/business-express/small-business-home): Sells company credit reports (£24.99 ex VAT each); no KYB or AML check in the product.
- Fourthline (https://www.fourthline.com/): Home page lists person verification, AML screening and fraud modules; no KYB product page found on its site.
- FullCircl (https://www.fullcircl.com/): Site now redirects to nCino.
- IDnow (https://www.idnow.io/): Home page lists only person identity, AML screening and data checks; no business verification.
- Jumio (https://www.jumio.com/platform/): KYX page has no business verification; person ID and AML screening only.
- Parcha (https://www.parcha.ai/): Its KYB product line was retired; the company now sells AI compliance agents as Grep AI.
- Plaid Identity Verification (https://plaid.com/products/identity-verification/): Verifies people only; no KYB on the product page.
- SEON (https://seon.io/): Home page lists person identity, document, address and AML screening; no KYB.
- Vespia (https://vespia.io/): Being acquired by Veriff (already listed); its pricing page now redirects to Veriff self-serve plans.
- ZignSec (https://www.zignsec.com/): Site now redirects to G2 Risk Solutions identity verification.

## Depth of a check

8 parts: register record, directors and officers, owners and ubos, sanctions, pep, adverse media, company documents, ongoing monitoring. Each counts 1 when the provider says it is included, 0.5 when it is a paid add-on, 0 when not offered or not stated. Depth = the sum divided by 8.

## Scoring

A check part counts 1 when the provider says it is included, 0.5 when it is a paid add-on, 0 when it is not offered or not stated. Yes/no criteria count 0 when the provider pages do not say. Score = sum of weight x value, out of 100. Equal scores share a rank.

## The four rankings

### A few checks a month (`small-business`)

A small business or agency checking suppliers, partners or customers now and then, without a compliance team.

| Weight | Criterion |
| --- | --- |
| 25 | You can buy KYB online without a sales call |
| 25 | Pay per check: no monthly fee or minimum volume |
| 20 | KYB price published |
| 20 | Depth of the check (8 parts: register, officers, owners, sanctions, PEP, adverse media, documents, monitoring) |
| 10 | Free start without sales |

### UK and EU counterparties (`uk-eu`)

A business that deals with companies registered in the UK and the EU.

| Weight | Criterion |
| --- | --- |
| 20 | UK registers named as covered |
| 25 | EU registers named as covered |
| 35 | Depth of the check (8 parts: register, officers, owners, sanctions, PEP, adverse media, documents, monitoring) |
| 10 | KYB price published |
| 10 | You can buy KYB online without a sales call |

### API for developers and AI agents (`api-agents`)

A product team putting company checks into its software or an AI agent.

| Weight | Criterion |
| --- | --- |
| 20 | API |
| 30 | MCP server or AI-agent connection to live data |
| 25 | Self-serve: keys without a sales call |
| 25 | KYB price published |

### Onboarding at volume (`enterprise`)

A regulated firm or platform onboarding many business customers worldwide.

| Weight | Criterion |
| --- | --- |
| 35 | Depth of the check (8 parts: register, officers, owners, sanctions, PEP, adverse media, documents, monitoring) |
| 25 | Coverage claimed in 100+ countries |
| 15 | Ongoing monitoring included |
| 25 | Identity verification of people on the same platform |

## Limits

- This compares published offers, not data quality, accuracy or service.
- A provider with a better offer behind a sales call scores lower than its product may deserve; that is the point of the small-business ranking (a buyer cannot see it either).
- This is not legal advice on whether you need KYB, and SONAR is not a regulated AML or KYC provider.
