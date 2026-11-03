# SEC Form D Scraper: Startup Funding Leads Feed (EDGAR): examples

Daily feed of new SEC Form D private raises from official EDGAR data, filtered by state, industry, size and exemption. Incremental: pay only for new filings. Optional open-jobs enrichment for companies with a known website.

This repo shows how to call the [SEC Form D Funding Feed](https://apify.com/clearfeedlabs/form-d-funding-feed) Apify Actor from JavaScript or Python, and what the output looks like.

## What's new
- `executives`, `directors`, `promoters` lists and the filing signer (`signerName`, `signerTitle`, `signatureDate`).

## Use cases
- Sales teams reaching companies that just raised money
- Investors and analysts tracking private-market activity
- Recruiters finding newly funded companies likely to hire
- Local economic-development and market research

## Quick start
1. Create a free Apify account and copy your API token from Settings > Integrations.
2. Set it as an environment variable: `export APIFY_TOKEN=...` (never commit it).
3. Edit `input.json`, then run one of:
   - JavaScript: `npm i apify-client && node run.mjs`
   - Python: `pip install apify-client && python run.py`

## Output fields (first of many)
`accessionNumber`, `formType`, `isAmendment`, `previousAccessionNumber`, `filedDate`, `filingUrl`, `cik`, `issuerName`, `entityType`, `jurisdictionOfInc`, `yearOfInc`, `incorporatedWithinFiveYears`, `address`, `companyPhone`, `industryGroup`, `fundType`, `revenueRange`, `federalExemptions`

See `sample-output.json` for one trimmed record.

## Ready-made example tasks
- [Biotech healthcare raises form d](https://apify.com/clearfeedlabs/form-d-funding-feed/examples/biotech-healthcare-raises-form-d)
- [California private raises form d](https://apify.com/clearfeedlabs/form-d-funding-feed/examples/california-private-raises-form-d)
- [Large private raises 10m form d](https://apify.com/clearfeedlabs/form-d-funding-feed/examples/large-private-raises-10m-form-d)
- [New york private raises form d](https://apify.com/clearfeedlabs/form-d-funding-feed/examples/new-york-private-raises-form-d)
- [Tech startup funding form d](https://apify.com/clearfeedlabs/form-d-funding-feed/examples/tech-startup-funding-form-d)

## Pricing
Pay per result: **$2.00 per 1,000 filings**, with no subscription. The [Store page](https://apify.com/clearfeedlabs/form-d-funding-feed) always shows current prices and every optional add-on event.

## FAQ
**Is this data official?** Yes. It comes from the public source named above, and each record links back to it.
**Do I need a login or proxy?** No. It uses documented public endpoints only.
**Can I schedule it?** Yes. Use Apify Schedules, the API or integrations (Zapier, Make, webhooks, MCP-compatible AI agents).

## Links
- Actor on the Apify Store: https://apify.com/clearfeedlabs/form-d-funding-feed
- Details & pricing: https://clearfeedlabs.com/actors/form-d-funding-feed/
- Clearfeed Labs: https://clearfeedlabs.com
- Bugs or questions: open an issue on the Actor's Issues tab on Apify.

Data comes from public sources and is provided as-is. Check the original source before relying on it. Not legal, financial or investment advice.

License: MIT
