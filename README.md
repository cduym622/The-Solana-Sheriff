# HenHacks 2026 Security Category Submission

## [The Solana Sheriff](https://github.com/edwardjones7/TheSolanaSheriff)
The Solana Sheriff was the submission of [Edward Jones](https://github.com/edwardjones7) and I into the HenHacks 2026 hackathon.

Find the devpost here: [devpost](https://devpost.com/software/the-solana-sheriff?ref_content=my-projects-tab&ref_feature=my_projects)

The Solana Sheriff is a full-stack Next.js web app that helps crypto newcomers avoid scams and bad decisions on Solana. It provides:

* AI Safety Assistant: a plain-language chat experience (with optional voice features).
* Wallet Analyzer: a wallet risk assessment based on on-chain patterns, with an optional AI summary.
* Scam Token Detector: a token “rugpull risk” scan (liquidity + distribution + mint authority), plus an optional AI verdict.
* Safety Resource Hub: curated educational content about common scams and best practices

**My contributions included:**

* Built the Wallet Analyzer, including the server-side API route that runs the analysis
* Integrated the Helius API to page through up to 2,000 transactions per wallet, determine its true age, and condense its history into a bounded evidence set
* Wrote the wallet-age and transaction-volume risk factors and integrated the Google Gemini API to return a structured risk verdict that cites specific red flags, falling back to the heuristic score if the call fails

My teammate built the Scam Token Detector, the AI Safety Assistant, and the voice features.

### Technologies

**Next.js · TypeScript · Tailwind CSS · Helius API · Google Gemini API**
