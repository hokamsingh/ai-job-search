# Job Scraper State

This directory holds the scraper's local state — `seen_jobs.json` is the machine-readable
source of truth (deduplication keys, fit assessments, rank scores once `/rank` runs). This
README is a human-readable mirror of the same data, regenerated whenever the pipeline updates
the JSON, so the current pool of scraped jobs is browsable directly on GitHub.

## `seen_jobs.json` schema

```json
{
  "seen": {
    "<url_or_company_title_key>": {
      "title": "...",
      "company": "...",
      "location": "...",
      "url": "...",
      "first_seen": "YYYY-MM-DD",
      "fit": "high | medium | low",
      "status": "new | ranked | expired | skipped",
      "portal": "<source portal skill, or 'websearch-fallback'>",
      "mass_posting_note": "optional - set when Step 2.5 flags a distribution pattern",
      "rank_score": "optional - set by /rank",
      "rank_verdict": "optional - set by /rank",
      "rank_date": "optional - set by /rank",
      "strengths": ["optional - set by /rank"],
      "gaps": ["optional - set by /rank"]
    }
  }
}
```

## Current postings (27 total)

Last updated: 2026-08-01. All entries below are `status: new` — ranking (`/rank`) has not
run yet because WebFetch access to posting pages was blocked in the environment during
today's scrape; scores will populate once a future run can fetch posting text.

| Fit | Title | Company | Location | First Seen | URL |
|-----|-------|---------|----------|------------|-----|
| high | Senior Backend Engineer (DeFi) - NestJS | Spectrum Search | Not stated | 2026-08-01 | [Link](https://www.linkedin.com/jobs/view/senior-backend-engineer-defi-nestjs-at-spectrum-search-4357581230) |
| high | Back End Software Engineer - Remote | Thriveworks | Atlanta, GA, United States (remote) | 2026-08-01 | [Link](https://www.linkedin.com/jobs/view/back-end-software-engineer-remote-at-thriveworks-3351103908) |
| high | Staff Backend Engineer (Node.js + TypeScript) - Remote Work (posted in 2+ countries) ⚠ Consolidated from 2 near-identical listings (Node.js/TypeScript, Staff level, 'Remote Work') on cl.linkedin.com and hn.linkedin.com; likely posted in additional country domains beyond these two. | BairesDev | Remote (multiple LinkedIn country domains: CL, HN) | 2026-08-01 | [Link](https://hn.linkedin.com/jobs/view/staff-backend-engineer-node-js-%2B-typescript-remote-work-at-bairesdev-4389593102) |
| high | Senior Node.JS Developer - Remote | Emtec Inc. | United States (remote) | 2026-08-01 | [Link](https://www.linkedin.com/jobs/view/senior-node-js-developer-remote-at-emtec-inc-3364398851) |
| high | Backend Engineer at Fintech Startup (ONRAMP) | Onramp | California, United States (Remote) | 2026-08-01 | [Link](https://www.linkedin.com/jobs/view/onramp-–-backend-engineer-at-fintech-startup-full-time-remote-at-onramp-2846803217) |
| high | Senior Lead Backend Engineer (Financial) - Technical Lead, Node | Averity (fintech client) | United States (100% Remote) | 2026-08-01 | [Link](https://www.linkedin.com/jobs/view/technical-lead-node-engineer-financial-100%25-remote-at-averity-3469596225) |
| high | Backend Engineer, Fintech | OnePay | United States | 2026-08-01 | [Link](https://www.linkedin.com/jobs/view/backend-engineer-fintech-at-onepay-4124382466) |
| high | Senior Backend Engineer - Retention/Sports Betting/iGaming | LeoVegas Group | Europe | 2026-08-01 | [Link](https://www.linkedin.com/jobs/view/senior-backend-engineer-retention-sports-betting-igaming-at-leovegas-group-4145078554) |
| high | Senior Back End Software Engineer (Remote) | Routable | Seattle, WA, United States (Remote, US/Canada team) | 2026-08-01 | [Link](https://www.linkedin.com/jobs/view/senior-back-end-software-engineer-remote-at-routable-3736332065) |
| high | Remote Senior Backend Software Developer | BitPay | Remote | 2026-08-01 | [Link](https://remoteok.com/remote-jobs/remote-senior-backend-software-developer-bitpay-1133985) |
| high | Senior Software Engineer, Backend (Onchain Payments) | Coinbase | United States | 2026-08-01 | [Link](https://builtin.com/job/senior-software-engineer-backend-developer-product-group/2660867) |
| medium | React JS + Node JS Developer - Remote (USA) | FullStack Labs | Remote, United States | 2026-08-01 | [Link](https://linkedin.com/jobs/view/react-js-+-node-js-developer-remote-usa-at-fullstack-labs-2968221543) |
| medium | Backend Engineer (Node/Nest.js) | micro1 | Latin America | 2026-08-01 | [Link](https://www.linkedin.com/jobs/view/backend-engineer-node-nest-js-at-micro1-4343526814) |
| medium | Full Stack Developer (Node.js, ReactJS, AWS) - Remote | ConnectTel, Inc. | Austin, TX, United States (remote) | 2026-08-01 | [Link](https://www.linkedin.com/jobs/view/full-stack-developer-node-js-reactjs-aws-remote-at-connecttel-inc-2746684156) |
| medium | Full Stack Engineer (TypeScript, Node.js, Nest.js) | Vonage | India | 2026-08-01 | [Link](https://in.linkedin.com/jobs/view/full-stack-engineer-typescript-node-js-nest-js-at-vonage-4400838757) |
| medium | Full Stack Engineer (React.js / NestJS / TypeScript / Node.js / GCP) | Photon | Not stated | 2026-08-01 | [Link](https://www.linkedin.com/jobs/view/full-stack-engineer-react-js-nestjs-typescript-node-js-gcp-at-photon-4428749355) |
| medium | Senior Software Engineer (TypeScript, NestJS, Node.js, React) | W3Global | Canada | 2026-08-01 | [Link](https://ca.linkedin.com/jobs/view/senior-software-engineer-typescript-nestjs-node-js-react-at-w3global-4437322060) |
| medium | Senior Backend Engineer (Fintech) | Recruiting from Scratch (fintech client) | Germantown, KY, United States | 2026-08-01 | [Link](https://www.linkedin.com/jobs/view/senior-backend-engineer-fintech-at-recruiting-from-scratch-3284314276) |
| medium | FinTech Full Stack Developer (US-Remote) | Token Metrics | United States (Remote) | 2026-08-01 | [Link](https://www.linkedin.com/jobs/view/fintech-full-stack-developer-us-remote-at-token-metrics-3251382677) |
| medium | Backend Engineer - the UK, Europe, remote | Workfully | UK/Europe (Remote) | 2026-08-01 | [Link](https://es.linkedin.com/jobs/view/backend-engineer-the-uk-europe-remote-at-workfully-4034553761) |
| medium | Remote Backend Engineer - Golang - Blockchain/DeFi | CyberCoders (blockchain/DeFi client) | Boston, MA, United States (Remote) | 2026-08-01 | [Link](https://www.linkedin.com/jobs/view/remote-backend-engineer-golang-blockchain-defi-at-cybercoders-2923855247) |
| medium | Blockchain Engineer (Remote) | Polygon Labs | United States (Remote) | 2026-08-01 | [Link](https://www.linkedin.com/jobs/view/blockchain-engineer-remote-at-polygon-labs-3496429679) |
| medium | Backend Engineer (REMOTE) | CoderPad | San Francisco, CA, United States (Remote) | 2026-08-01 | [Link](https://www.linkedin.com/jobs/view/backend-engineer-remote-at-coderpad-2660972215) |
| low | Junior Backend Engineer (Support) | Remote (remote.com) | United States (remote) | 2026-08-01 | [Link](https://www.linkedin.com/jobs/view/junior-backend-engineer-support-at-remote-2942631546) |
| low | Senior Full Stack Engineer (Node + NestJS + AWS) - Remote (Ireland/Portugal only) | Allshore Talent | Remote - restricted to Ireland/Portugal residents | 2026-08-01 | [Link](https://ie.linkedin.com/jobs/view/senior-full-stack-engineer-node-+-nestjs-+-aws-100%-remote-ireland-portugal-only-at-allshore-talent-4361540461) |
| low | Senior Backend Engineer (Remote, USA) | LeoLabs, Inc. | United States (Remote) | 2026-08-01 | [Link](https://www.linkedin.com/jobs/view/senior-backend-engineer-remote-usa-at-leolabs-inc-3318542585) |
| low | Backend Engineer (Remote) | IFTTT | San Francisco, CA, United States (Remote) | 2026-08-01 | [Link](https://www.linkedin.com/jobs/view/backend-engineer-remote-at-ifttt-3043181549) |

---
Regenerated by the `/daily-search` pipeline. Do not hand-edit — edits will be overwritten on the next scrape.
