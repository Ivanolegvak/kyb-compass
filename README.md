# KYB Compass: KYB providers compared

**KYB software pricing: what 43 providers charge and include, November 2026 edition.**

What 43 KYB and business verification providers charge and include, taken only from each provider’s own pricing, product and documentation pages, with four rankings by need under published weights. Updated monthly. Current edition: **November 2026** (`2026-11`, published 2026-11-17, corrected 2026-11-25).

- Article: https://getsonar.report/kyb-compass/findings
- Interactive comparison, filters and the cost-versus-depth map: https://getsonar.report/kyb-compass
- Dataset repository: https://github.com/Ivanolegvak/kyb-compass

Published by SONAR (https://getsonar.report), a KYB due-diligence tool that is one of the providers compared and is scored by the same rules. SONAR is not a regulated AML or KYC provider, and this dataset compares published offers, not data quality.

## Key findings (November 2026)

- **The hardest part is finding out what a check costs.** Only 12 of the 43 providers publish a price for a business check. 23 of the 27 identity-verification platforms that also do KYB publish no KYB price; Sumsub, iDenfy and Veriff, for example, publish what checking a person costs, while company checks sit behind a sales contact or an enterprise plan.
- **The monthly minimum matters more than the price per check.** For 5 company checks a month, the 5 pay-per-check providers with no monthly minimum cost €9 to €86 in total before VAT. KYB platforms that require a monthly plan charge from $150 (Baselayer) to €600 (Ondato) a month; UK company-data subscriptions include KYB checks from £19 a month (CompanyStack). If you check a handful of companies, look at the minimum before the unit price: it often decides the bill.
- **"200+ countries" does not tell you much.** 19 of the 43 providers name the UK or EU company registers they search. 14 others claim coverage in 150+ to 300+ countries or jurisdictions without naming a UK or EU register. If you work with companies in specific countries, ask for the list of registers for those countries before you buy.
- **Few can be bought without a sales call.** 12 of the 43 providers let you buy KYB online without talking to sales, and 11 offer a free start without sales. 40 have an API and 16 an MCP server or similar connection that lets AI agents query live data.

### What 5 company checks a month cost, pay per check with no minimum

| Provider | Cost of 5 checks | In euros |
| --- | --- | --- |
| Didit | from $10 | €9.08 |
| Certaby | £34.75 | €41.64 |
| SONAR | €45 | €45.00 |
| KYCAID | €50 | €50.00 |
| Know Your Customer | from $95 | €86.25 |

### Required monthly plans that include KYB

| Provider | Monthly fee | In euros |
| --- | --- | --- |
| CompanyStack | £19 | €22.77 |
| Endole | £39 | €46.73 |
| Baselayer | $150 | €136.19 |
| Ondato | €600 | €600.00 |

The two tables show 9 of the 12 providers that publish a price. Enigma, TheKYB and Global Database fit neither, as they do not sell per check without a minimum and state no required monthly fee. Their minimum terms: Enigma: not stated whether the free plan can buy KYB credits; Pro $20 a month, Max $200 a month. TheKYB: 100 verifications to begin. Global Database: not stated for reports; agreements for API and monitoring.

Prices are before VAT, converted at the ECB euro reference rates of 2026-11-16 (1 EUR = 0.8345 GBP = 1.1014 USD).

## Rankings by need (top 5)

There is no single best KYB provider: a platform built for a bank onboarding thousands of customers is the wrong buy for a firm checking five suppliers a month. Each ranking scores the same facts against criteria for one kind of buyer. The full rankings and weights are in `rankings.json` and [METHODOLOGY.md](METHODOLOGY.md).

### A few checks a month

A small business or agency checking suppliers, partners or customers now and then, without a compliance team.

| Rank | Provider | Score |
| --- | --- | --- |
| 1 | Didit | 97.5 |
| 2 | Certaby | 96.3 |
| 3 | SONAR (publisher) | 95 |
| 4 | KYCAID | 92.5 |
| 5 | Know Your Customer | 82.5 |

### UK and EU counterparties

A business that deals with companies registered in the UK and the EU.

| Rank | Provider | Score |
| --- | --- | --- |
| 1 | Didit | 95.6 |
| 2 | SONAR (publisher) | 91.3 |
| 3 | Know Your Customer | 86.9 |
| 4 | Global Database | 85.6 |
| 5 | Sumsub | 71.3 |
| 5 | Trulioo | 71.3 |

### API for developers and AI agents

A product team putting company checks into its software or an AI agent.

| Rank | Provider | Score |
| --- | --- | --- |
| 1 | Baselayer | 100 |
| 1 | CompanyStack | 100 |
| 1 | Didit | 100 |
| 1 | Enigma | 100 |
| 1 | SONAR (publisher) | 100 |

### Onboarding at volume

A regulated firm or platform onboarding many business customers worldwide.

| Rank | Provider | Score |
| --- | --- | --- |
| 1 | ComplyCube | 100 |
| 1 | Ondato | 100 |
| 1 | Shufti Pro | 100 |
| 4 | Credas | 95.6 |
| 4 | Socure | 95.6 |

## Disclosure

SONAR publishes KYB Compass and is one of the 43 providers, scored by exactly the same rules. In “A few checks a month” it ranks 3rd of 43, behind Didit and Certaby; in “UK and EU counterparties” it ranks 2nd of 43, behind Didit; in “API for developers and AI agents” it shares first place with 4 others (Baselayer, CompanyStack, Didit and Enigma); and in “Onboarding at volume” it ranks 41st of 43. What SONAR does not do: no identity verification of people, no ongoing monitoring. If something about a provider is wrong, email ivan@getsonar.report with the page that shows it and we will correct it.

## Files

| File | What it holds |
| --- | --- |
| vendors.csv | Every provider (50 rows: 43 ranked, 7 data and screening tools listed but not ranked), one row each, the fields below. |
| vendors.json | The same rows as JSON, with the edition and licence. |
| rankings.json | The four segments: who they are for, criteria with weights, and every ranked provider’s rank and score. |
| editions/<YYYY-MM>.json | The frozen data and rankings of each monthly edition. |
| editions/changes.json | What changed in each edition against the previous one. |
| METHODOLOGY.md | How the facts are collected and how the rankings are scored. |
| CHANGELOG.md | Editions and corrections. |
| CITATION.cff | Citation metadata. |
| LICENSE | CC BY 4.0. |

## Fields

| Field | Meaning |
| --- | --- |
| `slug` | Stable identifier of the provider. |
| `name` | Provider name. |
| `url` | Provider home page. |
| `hq` | Country of the head office or contracting entity, as its pages state it. |
| `kind` | kyb, kyc-kyb, credit-kyb, data or screening (see kind_label). |
| `kind_label` | The kind in words. |
| `ranked` | true when the provider sells a business check and is ranked; data and screening tools are listed, not ranked. |
| `publisher` | true for SONAR, the publisher of the dataset (scored by the same rules). |
| `focus` | What the provider says it is for, in one line. |
| `check_registry` | Register record: yes (included), addon (paid add-on), no (not offered) or unknown (not stated on its pages). |
| `check_officers` | Directors and officers: yes (included), addon (paid add-on), no (not offered) or unknown (not stated on its pages). |
| `check_owners` | Owners and UBOs: yes (included), addon (paid add-on), no (not offered) or unknown (not stated on its pages). |
| `check_sanctions` | Sanctions: yes (included), addon (paid add-on), no (not offered) or unknown (not stated on its pages). |
| `check_pep` | PEP: yes (included), addon (paid add-on), no (not offered) or unknown (not stated on its pages). |
| `check_adverse_media` | Adverse media: yes (included), addon (paid add-on), no (not offered) or unknown (not stated on its pages). |
| `check_documents` | Company documents: yes (included), addon (paid add-on), no (not offered) or unknown (not stated on its pages). |
| `check_monitoring` | Ongoing monitoring: yes (included), addon (paid add-on), no (not offered) or unknown (not stated on its pages). |
| `coverage` | Register coverage in the provider’s own words. |
| `names_uk_registers` | Its pages name UK registers as covered. |
| `names_eu_registers` | Its pages name EU registers as covered. |
| `names_us_registers` | Its pages name US registers as covered. |
| `claims_100_plus_countries` | Claims business coverage in 100 or more countries or jurisdictions. |
| `api` | Has an API. |
| `mcp` | Has an MCP server or similar connection for AI agents to live data (documentation-only MCP servers do not count). |
| `self_serve` | KYB can be bought online without talking to sales. |
| `free_start` | Free credit, trial or plan you can start without sales, in its words; empty when none is stated. |
| `kyc_too` | Also verifies people’s identity documents on the same platform. |
| `published_price` | A KYB price (per check, or a plan that includes KYB) is published. |
| `no_minimum` | KYB can be paid per check with no monthly fee and no minimum volume. |
| `price` | Published KYB price in its words, before VAT, or "Not published". |
| `minimum` | Monthly fee, minimum volume or contract, in its words. |
| `monthly_fee_amount` | Lowest monthly fee its pages require before you can buy KYB (monthly billing); empty when none is required or not published. |
| `monthly_fee_currency` | EUR, GBP or USD. |
| `cost_5_checks_amount` | What 5 company checks in a month cost at the published price: 5 x the price per check, or the monthly plan that includes them; empty when no price is published. |
| `cost_5_checks_currency` | EUR, GBP or USD. |
| `cost_5_checks_from` | true when the provider gives only a starting price. |
| `cost_5_checks_eur` | cost_5_checks_amount in euros at the ECB reference rate of the edition, rounded to cents. |
| `note` | Anything else its pages say that changes the picture. |
| `checked_on` | Date the provider’s pages were opened (YYYY-MM-DD). |
| `source_labels` | The provider pages the facts come from (CSV: separated by " \| "). |
| `source_urls` | Their URLs, in the same order (CSV: separated by " \| "). |

## How to cite

SONAR (2026). KYB Compass: KYB providers compared, November 2026 edition [Data set]. https://getsonar.report/kyb-compass. Licensed under CC BY 4.0.

Link the edition you used: `editions/2026-11.json`. When you quote a number, quote the edition month too: prices and features change.

## Corrections

Facts come only from the providers’ own pages, opened on the date in `checked_on`. “Not stated” (`unknown`) means the pages we opened do not say; it is not a claim that the feature is missing. Providers can send corrections, with the page that shows the fact, to ivan@getsonar.report.

## Licence

The data is licensed under the Creative Commons Attribution 4.0 International licence (CC BY 4.0): you may share and adapt it for any purpose, including commercially, if you credit “SONAR, KYB Compass” and link https://getsonar.report/kyb-compass. Provider names and trademarks belong to their owners.

## Try SONAR

Check a company yourself: register record, officers, owners, sanctions, PEP and adverse media in one report. The first report is free, no card: https://getsonar.report/login?mode=signup&ref=compass_dataset
