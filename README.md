# Bank of Lithuania Exchange Rates API — bank-of-lithuania-exchange-rate

[![npm version](https://img.shields.io/npm/v/bank-of-lithuania-exchange-rate.svg)](https://www.npmjs.com/package/bank-of-lithuania-exchange-rate)
[![license](https://img.shields.io/npm/l/bank-of-lithuania-exchange-rate.svg)](https://github.com/AllRates-Today/bank-of-lithuania-exchange-rate/blob/main/LICENSE)
[![zero dependencies](https://img.shields.io/badge/dependencies-0-brightgreen.svg)](https://www.npmjs.com/package/bank-of-lithuania-exchange-rate)
[![TypeScript](https://img.shields.io/badge/TypeScript-types%20included-3178C6.svg)](https://www.typescriptlang.org/)
[![EUR/AED today](https://img.shields.io/badge/dynamic/json?url=https%3A%2F%2Fallratestoday.com%2Fapi%2Fopen%2Fcentral-bank%2Flb%3Fsource%3DEUR%26target%3DAED&query=%24.rate&label=EUR%2FAED%20published%20by%20Bank%20of%20Lithuania&color=0A7E8C&cacheSeconds=3600)](https://allratestoday.com/central-bank-rates-api/lb/)
[![rate date](https://img.shields.io/badge/dynamic/json?url=https%3A%2F%2Fallratestoday.com%2Fapi%2Fopen%2Fcentral-bank%2Flb%3Fsource%3DEUR%26target%3DAED&query=%24.rate_date&label=rate%20date&color=555&cacheSeconds=3600)](https://allratestoday.com/central-bank-rates-api/lb/)

**Official Bank of Lithuania (Lithuania) daily exchange rates for Node.js and TypeScript. The published central bank rates behind tax filings, customs valuations, audits, and compliant invoicing — not market estimates, but the numbers Bank of Lithuania itself prints, every business day.**

## 🚀 Why this client?

- 🏛️ **Official published rates** — Bank of Lithuania's own table, with the publisher's own `rate_date` on every response
- 📅 **History back to 2015** — point-in-time tables and daily series for any past date
- 🔀 **Published vs derived, always flagged** — computed inverse/cross pairs carry `derived: true`, never mixed with official prints
- ⚡ **Zero dependencies** — pure ESM + CJS over global `fetch`; Node 18+, Bun, Deno, and edge runtimes
- 🔷 **Type-safe** — full TypeScript definitions shipped with the package
- 🧾 **Compliance-grade metadata** — `rate_type`, publication date, and source disclaimer on every response

> **Official rate, not mid-market:** every value here is a number Bank of Lithuania itself published, fixed once printed and carrying the central bank's own `rate_date` — what filings and audits require. Need the live mid-market rate for pricing or display instead? Use the [mid-market API](https://allratestoday.com/docs/) or [`@allratestoday/sdk`](https://www.npmjs.com/package/@allratestoday/sdk). The two can diverge by several percent.

## 🔑 Get your API key

Get a free API key at [allratestoday.com/register](https://allratestoday.com/register) — no credit card required. Latest rates are on every plan, including free.

## 📈 Latest published table

[![Latest Bank of Lithuania table](https://allratestoday.com/api/open/central-bank/lb/table.svg)](https://allratestoday.com/central-bank-rates-api/lb/)

The image is rendered live from the keyless endpoint, so it follows the central bank's publications on npm and on GitHub alike without a new release. The same table as text is folded below for search and copy-paste: on GitHub [a daily Action](.github/workflows/daily-table.yml) refreshes it whenever the central bank publishes a new table; on npm it is as of the package's publish date.

<!-- daily-table:start -->
<details>
<summary>Table as text: published 2026-10-30 by Bank of Lithuania — 86 rates, first 60 shown. Updated 2026-10-30.</summary>

| Base | Quote | Type | Rate |
| --- | --- | --- | ---: |
| EUR | AED | reference | 4.08952 |
| EUR | AFN | reference | 72.4044 |
| EUR | ALL | reference | 90.83674 |
| EUR | AMD | reference | 401.9374 |
| EUR | ARS | reference | 1714.0793 |
| EUR | AUD | reference | 1.5842 |
| EUR | AZN | reference | 1.89194 |
| EUR | BAM | reference | 1.95585 |
| EUR | BDT | reference | 137.9978 |
| EUR | BHD | reference | 0.42003 |
| EUR | BOB | reference | 13.35523 |
| EUR | BRL | reference | 5.9563 |
| EUR | BYN | reference | 3.28353 |
| EUR | CAD | reference | 1.5577 |
| EUR | CHF | reference | 0.9222 |
| EUR | CLP | reference | 1106.04043 |
| EUR | CNY | reference | 7.4144 |
| EUR | COP | reference | 3525.06337 |
| EUR | CZK | reference | 24.336 |
| EUR | DJF | reference | 197.69931 |
| EUR | DKK | reference | 7.4736 |
| EUR | DZD | reference | 150.73966 |
| EUR | EGP | reference | 62.3867 |
| EUR | ETB | reference | 182.72787 |
| EUR | GBP | reference | 0.83578 |
| EUR | GEL | reference | 2.88816 |
| EUR | GHS | reference | 12.95998 |
| EUR | GNF | reference | 9815.34471 |
| EUR | HKD | reference | 8.733 |
| EUR | HUF | reference | 365.95 |
| EUR | IDR | reference | 20193.16 |
| EUR | ILS | reference | 3.468 |
| EUR | INR | reference | 106.0345 |
| EUR | IQD | reference | 1687.9144 |
| EUR | ISK | reference | 135.8 |
| EUR | JOD | reference | 0.78934 |
| EUR | JPY | reference | 175.92 |
| EUR | KES | reference | 144.63066 |
| EUR | KGS | reference | 97.3685 |
| EUR | KRW | reference | 1488.4 |
| EUR | KWD | reference | 0.34688 |
| EUR | KZT | reference | 504.67082 |
| EUR | LBP | reference | 99730.58933 |
| EUR | LKR | reference | 370.1721 |
| EUR | LYD | reference | 7.15938 |
| EUR | MAD | reference | 10.94834 |
| EUR | MDL | reference | 20.03563 |
| EUR | MGA | reference | 5046.35189 |
| EUR | MKD | reference | 61.56211 |
| EUR | MNT | reference | 4003.2297 |
| EUR | MUR | reference | 52.85867 |
| EUR | MXN | reference | 20.8661 |
| EUR | MYR | reference | 4.5182 |
| EUR | MZN | reference | 71.07255 |
| EUR | NGN | reference | 1499.1931 |
| EUR | NOK | reference | 10.3315 |
| EUR | NZD | reference | 1.9817 |
| EUR | PAB | reference | 1.1134 |
| EUR | PEN | reference | 3.84401 |
| EUR | PHP | reference | 71.052 |

</details>

[Full table on the Bank of Lithuania rates page](https://allratestoday.com/central-bank-rates-api/lb/) · Source: [Official rates published by LB, served by AllRatesToday](https://allratestoday.com/central-bank-rates-api/lb/). Rates are as printed by the central bank; AllRatesToday is not affiliated with it.
<!-- daily-table:end -->

## 📦 Installation

```bash
npm install bank-of-lithuania-exchange-rate
```

```bash
yarn add bank-of-lithuania-exchange-rate
```

```bash
pnpm add bank-of-lithuania-exchange-rate
```

Requires Node 18+ (global `fetch`); also runs on Bun, Deno and edge runtimes. Also published under the org scope as [`@allratestoday/bank-of-lithuania-exchange-rate`](https://www.npmjs.com/package/@allratestoday/bank-of-lithuania-exchange-rate) — same code, same versions.

## 🏁 Quick start

```js
import { getRate } from 'bank-of-lithuania-exchange-rate';

const pair = await getRate('EUR', 'AED', { apiKey: 'art_live_...' });
console.log(pair.rate, pair.rate_date); // the official Bank of Lithuania rate, on the central bank's own date
```

## 📚 API reference

- [Latest pair rate](#latest-pair-rate) — one pair from the latest published table
- [Full published table](#full-published-table) — everything the central bank printed, in one call
- [Table for a date](#table-for-a-date) — the official table for an invoice or filing date
- [Daily time series](#daily-time-series) — one pair across a date range

---

### Latest pair rate

Free plan and up. Pairs the central bank does not print directly are resolved from its table and flagged (see *Published vs derived rates* below).

```js
const pair = await getRate('EUR', 'AED', { apiKey: 'art_live_...' });
```

**Response:**

```javascript
{
  bank: 'lb',
  name: 'Bank of Lithuania',
  rate_date: '2026-10-14',   // Bank of Lithuania's own publication date
  source: 'EUR',
  target: 'AED',
  rate: 4.16977,
  rate_type: 'reference',
  derived: false,
  method: 'published',
  disclaimer: 'Official rates as published by the named central bank. On weekends/holidays the most recent published rate_date is returned.'
}
```

### Full published table

Free plan and up. The complete table for the latest publication date.

```js
import { getLatestRates } from 'bank-of-lithuania-exchange-rate';

const table = await getLatestRates({ apiKey: 'art_live_...' });
console.log(table.rate_date, table.rates.length);
```

**Response:**

```javascript
{
  bank: 'lb',
  name: 'Bank of Lithuania',
  rate_date: '2026-10-14',
  rates: [
    { "base": "EUR", "quote": "AED", "type": "reference", "value": 4.16977 },
    // … the rest of the published table (87 currencies vs EUR)
  ],
  disclaimer: '…'
}
```

### Table for a date

Paid plans. The official table for any date since 2015 — weekends and holidays return the most recent published date, flagged via `published_on_requested_date`, which is exactly the in-force rate a filing needs.

```js
import { getRatesForDate } from 'bank-of-lithuania-exchange-rate';

const day = await getRatesForDate('2026-06-30', { apiKey: 'art_live_...' });
// Optionally narrow to one pair:
const one = await getRatesForDate('2026-06-30', { apiKey: 'art_live_...', source: 'EUR', target: 'AED' });
```

**Response:**

```javascript
{
  bank: 'lb',
  requested_date: '2026-06-30',
  rate_date: '2026-06-30',                // the date actually published
  published_on_requested_date: true,      // false when a weekend/holiday fell back
  rates: [ /* the full table for that date */ ],
  disclaimer: '…'
}
```

### Daily time series

Paid plans. One resolved rate per publication date — ready for charting, revaluation runs, or audit workpapers.

```js
import { getHistory } from 'bank-of-lithuania-exchange-rate';

const series = await getHistory(
  { source: 'EUR', target: 'AED', from: '2026-01-01', to: '2026-10-14' },
  { apiKey: 'art_live_...' }
);
```

**Response:**

```javascript
{
  bank: 'lb',
  source: 'EUR',
  target: 'AED',
  from: '2026-01-01',
  to: '2026-10-14',
  count: 152,
  rates: [
    // one entry per publication date
    { date: '2026-10-14', rate: 4.16977, rate_type: 'reference', derived: false, method: 'published' },
    // …
  ],
  disclaimer: '…'
}
```

Pass `{ symbol: 'AED' }` instead of `source`/`target` to get the raw published rows for one currency (all rate types, no pair resolution).

---

## 🗺️ Currencies covered

Bank of Lithuania currently publishes rates covering **87 currencies** against the EUR (as of the latest table):

🇦🇪 `AED` · 🇦🇫 `AFN` · 🇦🇱 `ALL` · 🇦🇲 `AMD` · 🇦🇷 `ARS` · 🇦🇺 `AUD` · 🇦🇿 `AZN` · 🇧🇦 `BAM` · 🇧🇩 `BDT` · 🇧🇭 `BHD` · 🇧🇴 `BOB` · 🇧🇷 `BRL` · 🇧🇾 `BYN` · 🇨🇦 `CAD` · 🇨🇭 `CHF` · 🇨🇱 `CLP` · 🇨🇳 `CNY` · 🇨🇴 `COP` · 🇨🇿 `CZK` · 🇩🇯 `DJF` · 🇩🇰 `DKK` · 🇩🇿 `DZD` · 🇪🇬 `EGP` · 🇪🇹 `ETB` · 🇬🇧 `GBP` · 🇬🇪 `GEL` · 🇬🇭 `GHS` · 🇬🇳 `GNF` · 🇭🇰 `HKD` · 🇭🇺 `HUF` · 🇮🇩 `IDR` · 🇮🇱 `ILS` · 🇮🇳 `INR` · 🇮🇶 `IQD` · 🇮🇷 `IRR` · 🇮🇸 `ISK` · 🇯🇴 `JOD` · 🇯🇵 `JPY` · 🇰🇪 `KES` · 🇰🇬 `KGS` · 🇰🇷 `KRW` · 🇰🇼 `KWD` · 🇰🇿 `KZT` · 🇱🇧 `LBP` · 🇱🇰 `LKR` · 🇱🇾 `LYD` · 🇲🇦 `MAD` · 🇲🇩 `MDL` · 🇲🇬 `MGA` · 🇲🇰 `MKD` · 🇲🇳 `MNT` · 🇲🇺 `MUR` · 🇲🇽 `MXN` · 🇲🇾 `MYR` · 🇲🇿 `MZN` · 🇳🇬 `NGN` · 🇳🇴 `NOK` · 🇳🇿 `NZD` · 🇵🇦 `PAB` · 🇵🇪 `PEN` · 🇵🇭 `PHP` · 🇵🇰 `PKR` · 🇵🇱 `PLN` · 🇶🇦 `QAR` · 🇷🇴 `RON` · 🇷🇸 `RSD` · 🇸🇦 `SAR` · 🇸🇪 `SEK` · 🇸🇬 `SGD` · 🇸🇾 `SYP` · 🇹🇭 `THB` · 🇹🇯 `TJS` · 🇹🇲 `TMT` · 🇹🇳 `TND` · 🇹🇷 `TRY` · 🇹🇼 `TWD` · 🇹🇿 `TZS` · 🇺🇦 `UAH` · 🇺🇸 `USD` · 🇺🇾 `UYU` · 🇺🇿 `UZS` · 🇻🇪 `VES` · 🇻🇳 `VND` · `XAF` · `XOF` · 🇾🇪 `YER` · 🇿🇦 `ZAR`

## 🏛️ Source

The Bank of Lithuania publishes, alongside the ECB reference list it republishes as a euro member, its own daily table of around 87 currencies the ECB does not quote — from the UAE dirham to the Zambian kwacha — expressed as foreign units per euro. Lithuanian accounting and VAT rules cite this list, and the bank posts the next business day's table in advance.

- Publisher's own page: [Exchange rates (LT list)](https://www.lb.lt/en/currency-exchange-rates) · [www.lb.lt](https://www.lb.lt)
- Publication: every business day; the exact schedule, freshness status and any current delay are on the [Bank of Lithuania rates page](https://allratestoday.com/central-bank-rates-api/lb/)
- In the API: usually by **12:25 UTC** (measured over the last 12 publications). Schedule a sync at or after that time and retry hourly until `rate_date` moves; every response carries the same figure as `available_by_utc` — see [when to poll](https://allratestoday.com/docs/#when-to-poll)
- Values are stored unmodified, with the publisher's own `rate_date` on every row — see the [methodology](https://allratestoday.com/official-rates-methodology/)

## 🧭 Reading the numbers

- `value` is always **quote currency per 1 unit of base currency** (`base: "EUR", quote: "USD", value: 1.15` means 1 EUR = 1.15 USD).
- Bank of Lithuania quotes **foreign currency per 1 EUR** (e.g. `base: "EUR", quote: "USD"` means USD per one EUR).
- Need the other way round? Ask `getRate(target, source)` and the API inverts or crosses for you, flagged `derived: true` — never divide a published rate yourself in a compliance workflow.
- `rate_type` tells you which of the central bank's series a row belongs to (`reference` here); some publishers print buy/sell or several fixings for the same pair.

## 🧩 ERP & accounting systems

Loading the official Bank of Lithuania rate into an accounting system is a supported workflow, not a hack. Step-by-step guides with the direction each system expects:

- [Dynamics 365 Business Central](https://allratestoday.com/docs/integrations/business-central/) — built-in Currency Exchange Rate Service, no code
- [Xero](https://allratestoday.com/docs/integrations/xero/) · [QuickBooks Online](https://allratestoday.com/docs/integrations/quickbooks/) · [SAP S/4HANA and ECC](https://allratestoday.com/docs/integrations/sap/) · [Odoo](https://allratestoday.com/docs/integrations/odoo/)

The same keyed endpoints return `?format=csv`, `?format=xml` and `?format=xlsx`, and accept the key as `?api_key=` on the URL for importers that cannot send headers:

```bash
curl "https://allratestoday.com/api/v1/central-bank/lb/latest?format=xml&api_key=art_live_..."
```

## 🤖 AI agents

- MCP server: `npx -y @allratestoday/central-bank-mcp` (stdio) or the hosted endpoint `https://allratestoday.com/api/mcp` — tools for official rates, history, cross-bank comparison and publication calendars
- Already using the general SDK or MCP server? Since 2026-10-01 [`@allratestoday/sdk`](https://www.npmjs.com/package/@allratestoday/sdk) 1.4+ has `officialRates('lb')` and [`@allratestoday/mcp-server`](https://www.npmjs.com/package/@allratestoday/mcp-server) 0.6+ has a `get_official_rates` tool — both return this source's latest table with no key, so you can add it without a second dependency
- Claude Code plugin (no key): `/plugin marketplace add AllRates-Today/claude-code-plugin` then `/plugin install allratestoday@allratestoday` — bundles both MCP servers plus an `/official-rate lb ...` command
- Evaluating? Agents can self-issue a trial key with no signup: `POST https://allratestoday.com/api/agent/keys` (send `Content-Type: application/json`) returns a 100-call key valid 7 days that covers the free-plan methods (latest table, pairs); dated tables and history need a [paid plan](https://allratestoday.com/pricing/). The MCP servers expose it as `request_trial_key`
- Machine-readable site guide: [llms.txt](https://allratestoday.com/llms.txt) · [for-ai-agents](https://allratestoday.com/for-ai-agents/)

## ⚖️ Published vs derived rates

If Bank of Lithuania does not print a pair directly, the API resolves it from the central bank's own table and says so — official and computed values are never confused:

| `method` | `derived` | Meaning |
| --- | --- | --- |
| `published` | `false` | The central bank printed this pair directly |
| `inverse` | `true` | Computed as 1 ÷ the published opposite direction |
| `cross` | `true` | Computed via EUR from two published rates |

## 🛡️ Error handling

Errors are thrown as `Error` with `status` (HTTP code) and `body` (the API's JSON error) attached:

```js
try {
  const pair = await getRate('EUR', 'XXX', { apiKey: 'art_live_...' });
} catch (err) {
  console.log(err.message); // human-readable reason
  console.log(err.status);  // e.g. 404
}
```

| Status | Meaning |
| ------ | ------- |
| — | Missing `apiKey` (thrown before any request) |
| `400` | Malformed date or parameters |
| `401` | Invalid API key |
| `403` | Endpoint needs a [paid plan](https://allratestoday.com/pricing/) (historical dates & series) |
| `404` | Pair or date range not covered by Bank of Lithuania |
| `429` | Monthly quota exceeded |

## 🔷 TypeScript

Full definitions ship with the package — no `@types` install:

```ts
import type { LatestRates, PairRate, DatedRates, RateEntry, HistoryQuery, RequestOptions } from 'bank-of-lithuania-exchange-rate';
```

## 📦 CommonJS

```javascript
const { getRate } = require('bank-of-lithuania-exchange-rate');

getRate('EUR', 'AED', { apiKey: 'art_live_...' }).then((pair) => console.log(pair.rate));
```

## 💡 Quota tips

- Rates change once per business day — cache the published table locally and a small monthly quota goes a long way.
- Every request counts toward your AllRatesToday quota, shared across all AllRatesToday endpoints on your key.

## 📖 Methods reference

| Method | Plan | Description |
| ------ | ---- | ----------- |
| `getRate(source, target, { apiKey })` | Free | Latest rate for one pair, resolved from the published table |
| `getLatestRates({ apiKey })` | Free | The central bank's full latest published table |
| `getRatesForDate(date, { apiKey, source?, target? })` | Paid | The official table (or one pair) for a YYYY-MM-DD date |
| `getHistory({ symbol \| source+target, from?, to? }, { apiKey })` | Paid | Daily series since 2015 |

## 📥 Bulk data (no key)

Need the whole archive rather than an API call? The same published tables are mirrored daily as open data:

- Hugging Face: [AllRatesToday/central-bank-exchange-rates](https://huggingface.co/datasets/AllRatesToday/central-bank-exchange-rates) — one CSV per institution (`rates/lb.csv`)
- Kaggle: [allratestoday/central-bank-exchange-rates](https://www.kaggle.com/datasets/allratestoday/central-bank-exchange-rates)
- Raw JSON on GitHub: `https://raw.githubusercontent.com/AllRates-Today/central-bank-exchange-rates/main/data/lb/latest.json`

## 🔗 Links

- [Bank of Lithuania rates page](https://allratestoday.com/central-bank-rates-api/lb/) — live table, publication cadence, FAQ
- [All central bank sources](https://allratestoday.com/central-bank-rates-api/)
- [Package docs on the site](https://allratestoday.com/docs/sdk/bank-of-lithuania-exchange-rate/) · [ERP integration guides](https://allratestoday.com/docs/integrations/)
- [API documentation](https://allratestoday.com/docs/#central-bank) · [Interactive reference](https://allratestoday.com/api-reference/) · [Methodology](https://allratestoday.com/official-rates-methodology/)
- [Register (Free)](https://allratestoday.com/register) · [Dashboard](https://allratestoday.com/profile) · [Pricing](https://allratestoday.com/pricing/)
- [Status](https://allratestoday.com/status)
- [Postman collection](https://allratestoday.com/postman/)
- [GitHub](https://github.com/AllRates-Today/bank-of-lithuania-exchange-rate)

## 📜 License

MIT
