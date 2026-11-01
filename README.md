# Awesome-Data-Loss-Prevention-DLP

**Top Data Loss Prevention DLP (Opensource) 🌟 Star if you like it! 🌟**

**Curated List of SaaS Products & Open-Source GitHub Projects**

*Focused on Endpoint DLP, Cloud Egress Control, PII Detection & Self-Hosted Data Leak Gates*

**Last updated: November 2026**

This repository tracks notable **SaaS platforms** and **open-source projects** for **Data Loss Prevention (DLP)**. These tools enable organizations to detect and block sensitive data from leaving their perimeter—across endpoints, email, cloud apps, and AI tools—from fully managed enterprise suites with ML-based classification to open-source gates that scrub data before it reaches external services.

**Examples** include CrowdStrike Falcon Data Protection, Symantec DLP, Forcepoint DLP, Microsoft Purview DLP, Netskope DLP, Zscaler DLP, Digital Guardian, Proofpoint Enterprise DLP, Nightfall AI, and Cyberhaven (the category leaders in commercial space).

**Open-source emphasis**: This section is expanded with relevant projects for self-hosted DLP, PII detection, AI egress guardrails, and data leak prevention.

Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites.

## Table of Contents

- [Sector Overview & Market Dynamics](#sector-overview--market-dynamics)
- [SaaS/Hosted Platforms](#saashosted-platforms)
- [Open-Source GitHub Projects](#open-source-github-projects)
- [How to Contribute](#how-to-contribute)
- [Disclaimer](#disclaimer)

## Sector Overview & Market Dynamics

The global Data Loss Prevention (DLP) market is valued at approximately **$3.5B to $4.3B** and is projected to expand at an **18%–24% CAGR** toward **$13B–$24B+** by the early 2030s, fueled by hybrid workforces, cloud migration, stringent data privacy regulations (GDPR, HIPAA), and generative AI egress risks. 

The sector displays a **moderately to heavily concentrated structure** at the top enterprise tier dominated by diversified cybersecurity giants (Microsoft, Broadcom/Symantec, CrowdStrike, Forcepoint, Zscaler), while maintaining a **fragmented periphery** where specialized startups compete in emerging niches like generative AI data security, agentic AI workflows, and cloud-native API/SSPM DLP.

## SaaS/Hosted Platforms

| Product | Company Scale (Revenue / Valuation) | Pricing (Starting Tier) | Free Tier Limits / Free Trial Limits | Channel Coverage & Focus |
| :--- | :--- | :--- | :--- | :--- |
| **[Microsoft Purview DLP](https://www.microsoft.com/purview)** | **~$3.88T Market Cap** (~$245B+ Annual Revenue) | **$12.00/user/month** (M365 E5 Compliance add-on; full suite $60/user/month for M365 E5) | **Included with M365 E3** (basic DLP policy and labels; excludes Insider Risk & Advanced eDiscovery) / 30-day trial of M365 E5 available (up to 25 user licenses) | Native M365, Teams, SharePoint, OneDrive, and Copilot data boundary governance; requires Defender connectors for 3rd-party SaaS. |
| **[Symantec DLP](https://www.broadcom.com/)** | **~$1.6T Market Cap** (~$51B+ Annual Revenue - Broadcom) | **$1.99/user/year** (Starting tier per SelectHub; ~$14.00/user/year on Capterra) | **No permanent free tier**; 30-day proof-of-concept / evaluation license available via Broadcom partner network | Deep multi-channel enterprise coverage across endpoints, network, email, web traffic, and hybrid cloud storage (AWS, Azure, GCP). |
| **[CrowdStrike Falcon Data Protection](https://www.crowdstrike.com/)** | **~$250B Market Cap** (~$5.84B ARR) | **$73.99/endpoint/year** (CDW Tier 3: 300–499 endpoints; or ~$68.86/endpoint/year on 46-month volume agreement) | **No permanent free tier**; 15-day Falcon platform trial available (limited to endpoint detection / lab agents upon approval) | AI-driven endpoint DLP unified on the Falcon single-agent architecture, monitoring endpoint clipboard, browser, and USB transfers. |
| **[Zscaler DLP](https://www.zscaler.com/)** | **~$40B Market Cap** (~$3.35B Annual Revenue) | **$1,000.00/year** (Starting entry package on AppDirect marketplace; ~$2.00–$5.00/user/month at enterprise volume) | **No permanent free tier**; Custom enterprise evaluation / PoC typically scoped for 14 to 30 days upon sales consultation | Inline zero-trust inspection across cloud web proxy (SWG), CASB, email, SSPM, and generative AI prompt exfiltration controls. |
| **[Proofpoint Enterprise DLP](https://www.proofpoint.com/)** | **$12.3B Valuation** (Thoma Bravo acquisition; ~$1B+ ARR) | **$24.00/user/year** ($2.00/user/month modular entry estimate; SMB Essentials DLP starts at $2.75–$3.93/user/month) | **No permanent free tier**; 30-day guided evaluation / Proof of Concept coordinated through enterprise sales | People-centric DLP covering email gateways, cloud SaaS, endpoints, and insider threat management (ITM). |
| **[Netskope DLP](https://www.netskope.com/)** | **~$6.5B Valuation** (~$899M ARR / ~$709M Revenue - NASDAQ: NTSK) | **$50.00/user/year** (~$4.16/user/month base SWG/CASB starting tier; annual contracts typically start at ~$35,000/year) | **No permanent free tier**; Guided 14 to 30-day Proof of Concept (PoC) scoped for corporate cloud and CASB environments | Cloud-native DLP deeply embedded within Netskope's SASE/SSE architecture, inspecting content and metadata across SaaS and web. |
| **[Forcepoint DLP](https://www.forcepoint.com/)** | **$2.45B Valuation** (carve-out basis; ~$650M Annual Revenue) | **$32.00/user/year** (Baseline compliance licensing starting tier; full IP protection ranges $55–$150+/user/year) | **No permanent free tier**; 14 to 30-day evaluation trial available upon request via enterprise sales | Unified policy engine across web, email, cloud, network, and endpoints with 1,800+ predefined regulatory policies and shadow AI controls. |
| **[Cyberhaven](https://www.cyberhaven.com/)** | **$1.0B Valuation** (Unicorn status; ~$50M+ ARR) | **$30,000.00/year** (Minimum enterprise starting tier contract; translates to ~$4.00–$8.00/user/month at scale) | **No permanent free tier**; 14 to 30-day Proof of Value (PoV) sandbox evaluation offered to qualified enterprise prospects | Patented data lineage tracking at the fragment level; protects sensitive data moving into AI tools, coding assistants (Cursor, Claude Code), and cloud apps. |
| **[Digital Guardian](https://www.digitalguardian.com/)** | **~$500M–$1B Scale** (Parent company Fortra / Thoma Bravo portfolio) | **$60,000.00/year** (Baseline deployment package including management console; minimum 1,000 endpoint threshold) | **No permanent free tier**; 14 to 30-day Proof of Concept (PoC) evaluation coordinated through Fortra sales engineering | Deep kernel-level endpoint inspection, full context tracking, user behavior monitoring, and managed DLP service (MSSP). |
| **[Nightfall AI](https://www.nightfall.ai/)** | **~$150M–$250M Valuation** (~$60M raised; ~$20M+ ARR) | **$48.00/user/year** ($4.00/user/month baseline tier; Nightfall for LLMs custom volume packs) | **Free Developer Tier: 3 GB/month** of scanned data via API; 7-day enterprise Proof of Value (POV) for SaaS and endpoint agents | AI/LLM-native detector utilizing neural NLP models (95% precision) across Slack, Google Drive, Jira, GitHub, endpoints, and GenAI prompts. |

## Open-Source GitHub Projects

| Project | Stars | Focus & Architectural Role | License |
| :--- | :--- | :--- | :--- |
| **[OpenMetadata](https://github.com/open-metadata/OpenMetadata)** | [![GitHub stars](https://img.shields.io/github/stars/open-metadata/OpenMetadata?style=social&color=white)](https://github.com/open-metadata/OpenMetadata/stargazers) | **Unified Metadata & Automated PII Classification Platform**: Comprehensive data governance and cataloging engine with integrated sensitive data discovery, automated column profiling, and PII tagging across modern data warehouses. | Apache-2.0 |
| **[Presidio](https://github.com/microsoft/presidio)** | [![GitHub stars](https://img.shields.io/github/stars/microsoft/presidio?style=social&color=white)](https://github.com/microsoft/presidio/stargazers) | **PII Detection and Anonymization Engine**: Microsoft's production-grade framework providing customizable recognizers (regex, NER, checksums) and redactors/maskers for structured and unstructured data. | MIT |
| **[Cybersecurity-Projects (dlp-scanner)](https://github.com/CarterPerez-dev/Cybersecurity-Projects)** | [![GitHub stars](https://img.shields.io/github/stars/CarterPerez-dev/Cybersecurity-Projects?style=social&color=white)](https://github.com/CarterPerez-dev/Cybersecurity-Projects/stargazers) | **Multi-Format Data Loss Prevention Scanner**: Educational reference architecture featuring file extractors, sensitive pattern matching algorithms, redaction pipelines, and compliance scoring reporters. | MIT |
| **[pipelock](https://github.com/pipelab-org/pipelock)** | [![GitHub stars](https://img.shields.io/github/stars/pipelab-org/pipelock?style=social&color=white)](https://github.com/pipelab-org/pipelock/stargazers) | **AI Agent Security Gateway & Egress Firewall**: Mediates HTTP, MCP, A2A, and WebSocket agent traffic to detect prompt injections and sensitive data exfiltration before external egress. | Apache-2.0 |
| **[earlybird](https://github.com/americanexpress/earlybird)** | [![GitHub stars](https://img.shields.io/github/stars/americanexpress/earlybird?style=social&color=white)](https://github.com/americanexpress/earlybird/stargazers) | **Static Source Code Sensitive Data Scanner**: American Express's enterprise scanner for detecting hardcoded secrets, PII, cleartext credentials, and outdated cryptographic implementations in repositories. | Apache-2.0 |
| **[DontFeedTheAI](https://github.com/zeroc00I/DontFeedTheAI)** | [![GitHub stars](https://img.shields.io/github/stars/zeroc00I/DontFeedTheAI?style=social&color=white)](https://github.com/zeroc00I/DontFeedTheAI/stargazers) | **Transparent LLM Anonymization Proxy**: Intercepts requests destined for cloud LLMs (Claude, OpenAI, OpenRouter) and strips IP addresses, credentials, hostnames, and PII using local Ollama and regex engines. | GPL-3.0 |
| **[pii-masker](https://github.com/HydroXai/pii-masker)** | [![GitHub stars](https://img.shields.io/github/stars/HydroXai/pii-masker?style=social&color=white)](https://github.com/HydroXai/pii-masker/stargazers) | **Transformer-Powered PII Masking Tool**: High-precision sensitive entity detection and masking utility utilizing DeBERTa-v3 to guard privacy in enterprise AI pipelines. | MIT |
| **[openredaction](https://github.com/sam247/openredaction)** | [![GitHub stars](https://img.shields.io/github/stars/sam247/openredaction)](https://github.com/sam247/openredaction/stargazers) | **Local-First TypeScript PII Redaction Engine**: Fast, browser- and Node.js-compatible open-source PII detection and redaction library operating 100% on-device. | MIT |
| **[dlp-pdf-redaction](https://github.com/GoogleCloudPlatform/dlp-pdf-redaction)** | [![GitHub stars](https://img.shields.io/github/stars/GoogleCloudPlatform/dlp-pdf-redaction?style=social&color=white)](https://github.com/GoogleCloudPlatform/dlp-pdf-redaction/stargazers) | **Serverless Document Redaction Pipeline**: Cloud Run and Cloud Workflows architecture demonstrating automated visual and text redaction of sensitive PDF data via Google Cloud DLP APIs. | Apache-2.0 |
| **[nightfall_dlp_action](https://github.com/nightfallai/nightfall_dlp_action)** | [![GitHub stars](https://img.shields.io/github/stars/nightfallai/nightfall_dlp_action?style=social&color=white)](https://github.com/nightfallai/nightfall_dlp_action/stargazers) | **CI/CD Pull Request DLP Action**: Automated GitHub Actions security check scanning pull request diffs for sensitive customer data, PII, and API secrets to prevent repository leaks. | MIT |
| **[BSC_DLP_Community](https://github.com/marianabsctba/BSC_DLP_Community)** | [![GitHub stars](https://img.shields.io/github/stars/marianabsctba/BSC_DLP_Community?style=social&color=white)](https://github.com/marianabsctba/BSC_DLP_Community/stargazers) | **Enterprise Endpoint & Network DLP Platform**: Community edition of an open-source data loss prevention system for discovering, classifying, and enforcing protection policies across network nodes. | GPL-3.0 |
| **[onprem-dlp](https://github.com/portable-genai/onprem-dlp)** | [![GitHub stars](https://img.shields.io/github/stars/portable-genai/onprem-dlp?style=social&color=white)](https://github.com/portable-genai/onprem-dlp/stargazers) | **Deterministic On-Prem Cloud Egress Gate**: CPU-only DLP gate scrubbing sensitive structured columns and unstructured documents/images before reaching cloud LLMs and APIs via deterministic checksum validators. | Apache-2.0 |

---

### Additional Open-Source Observations

- **No mature open-source endpoint DLP exists.** Symantec, Forcepoint, CrowdStrike, and Microsoft dominate full endpoint DLP agent coverage. Open-source solutions excel primarily in egress inspection gates (`onprem-dlp`, `DontFeedTheAI`, `pipelock`), static repository scanning (`earlybird`, `nightfall_dlp_action`), data catalog tagging (`OpenMetadata`), and modular PII detection libraries (`Presidio`, `pii-masker`, `openredaction`).
- **Composing an Open-Source Data Security Stack**: Combine **OpenMetadata** for catalog and warehouse classification, **Presidio** or **pii-masker** for PII detection, and **pipelock** or **onprem-dlp** as a gate for AI/LLM egress enforcement.

## How to Contribute

1. Fork the repo.
2. Add/edit entries in `README.md` (follow existing format and table structure).
3. Include: name, link, specific starting tier pricing, free tier/trial limits, company size, and license (for open-source).
4. Submit PR with a short explanation.

Star the repo if you find it useful!

## Disclaimer

- This is a **community-curated** list — not exhaustive and not an endorsement.
- DLP platforms handling sensitive data and policy enforcement must comply with data protection regulations (GDPR, CCPA, HIPAA, etc.) and implement appropriate access controls and audit logging.
- **The "endpoint DLP" vs. "cloud egress gate" vs. "detection library" distinction is critical.** Commercial DLP suites monitor endpoints, email, cloud, and network channels with centralized policy enforcement. Open-source tools focus on specific egress checkpoints or foundational detection libraries.
- All product names, logos, and brands are property of their respective owners.

---

**Made for security engineers, data protection teams, and organizations building transparent DLP solutions.**
