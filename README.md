# Awesome-Data-Loss-Prevention-DLP

# Awesome-Data-Loss-Prevention-DLP
**Top Data Loss Prevention DLP (Opensource) 🌟 Star if you like it! 🌟**

**Curated List of SaaS Products & Open-Source GitHub Projects**
*Focused on Endpoint DLP, Cloud Egress Control, PII Detection & Self-Hosted Data Leak Gates*
**Last updated: November 2026**

This repository tracks notable **SaaS platforms** and **open-source projects** for **Data Loss Prevention (DLP)**. These tools enable organizations to detect and block sensitive data from leaving their perimeter—across endpoints, email, cloud apps, and AI tools—from fully managed enterprise suites with ML-based classification to open-source gates that scrub data before it reaches external services.

**Examples** include CrowdStrike Falcon Data Protection, Symantec DLP, Forcepoint DLP, Microsoft Purview DLP, Netskope DLP, Zscaler DLP, Digital Guardian, Proofpoint Enterprise DLP, Nightfall AI, and Cyberhaven (the category leaders in commercial space).

**Open-source emphasis**: This section is expanded with every relevant project for self-hosted DLP, PII detection, and open data leak prevention. **Critical note**: The open-source DLP landscape is sparse but functional—**onprem-dlp** is the most purpose-built open-source DLP gate for preventing sensitive data from reaching cloud LLMs and APIs . **Presidio** provides the detection engine that many DLP tools build upon. No open-source project matches Symantec's channel coverage or Cyberhaven's data lineage depth, but for specific egress control use cases, the open-source options are viable.

Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites.

## Table of Contents
- [SaaS/Hosted Platforms](#saas-hosted-platforms)
- [Open-Source GitHub Projects](#open-source-github-projects)
- [How to Contribute](#how-to-contribute)
- [Disclaimer](#disclaimer)

## SaaS/Hosted Platforms

- **[CrowdStrike Falcon Data Protection](https://www.crowdstrike.com/)**
  **AI-powered endpoint DLP** built on Falcon's unified agent. Monitors data at rest and in motion, including artifacts moving from web sources and endpoints to USBs and via browsers to cloud/SaaS apps . **Pricing**: **$73.99/year per endpoint** (Tier 3, 300–499 endpoints) per CDW listing ; 46-month subscription at **$263.97 per endpoint** (~$68.86/year) . **Free tier**: None. **Best for**: CrowdStrike customers wanting DLP integrated with endpoint protection—**trade-off**: requires Falcon agent; best value at volume pricing tiers.

- **[Symantec DLP](https://www.broadcom.com/)**
  **Enterprise DLP with broad channel coverage** across endpoint, network, and storage. Monitors USB, email, and web traffic; ties events to specific users for rapid incident response; works on-premises or cloud with AWS/Azure/GCP integration . **Pricing**: **Starting at $1.99/user/year** per SelectHub ; Capterra lists **$14/user/year** . **Free tier**: None; free trial available. **Best for**: large enterprises wanting predictable per-user pricing with deep cloud support—**trade-off**: frequent complaints about support quality and slow scanning; policy creation takes time .

- **[Forcepoint DLP](https://www.forcepoint.com/)**
  **Unified DLP across email, cloud, web, endpoint, and AI**. Named a **Leader in IDC MarketScape: Worldwide DLP 2025** . **1,800+ predefined policies and classifiers** covering 80+ countries' regulations; **GDPR policies included**; prevents copy/paste into ChatGPT and blocks shadow AI apps; same policy engine across all channels . **Pricing**: **Custom quote**—explicitly positioned as customized . **Free tier**: None. **Best for**: enterprises wanting unified policy across email and cloud without rearchitecting—**trade-off**: quote-only; policy tuning requires 1–2 FTE-months per third-party estimates .

- **[Microsoft Purview DLP](https://www.microsoft.com/purview)**
  **DLP within Microsoft 365** with Copilot integration. **Critical for Copilot deployments**: sensitivity labels tell Copilot which content requires special handling; DLP blocks Copilot from including regulated content in responses even if users can access it . **Pricing**: Requires **M365 E5 Compliance add-on ($12/user/month)** or **E5 ($60/user/month)** for full functionality; E3 gets basic labels and DLP but misses Insider Risk, Advanced eDiscovery, and Records Management . **Free tier**: Basic DLP on E3. **Best for**: Microsoft 365 enterprises needing DLP that prevents Copilot from exposing over-shared content—**trade-off**: content-blind outside M365 ecosystem; non-Microsoft SaaS coverage requires Defender for Cloud Apps connectors and incurs Purview At Rest charges ($0.50/1,000 files/month) .

- **[Netskope DLP](https://www.netskope.com/)**
  **Cloud-native DLP** within Netskope's SASE platform. Basic DLP included in Prime Advantage package; advanced DLP in Max Advantage; inspects file contents and metadata . **Pricing**: **Quote-only**; packaged as part of SASE tiers . **Free tier**: None. **Best for**: organizations adopting SASE wanting DLP integrated with CASB and SWG—**trade-off**: DLP depth varies by package tier.

- **[Zscaler DLP](https://www.zscaler.com/)**
  **Inline and cloud DLP** within Zscaler's Zero Trust Exchange. Covers inline DLP, CASB, endpoint, email, SSPM, DSPM, workloads, and BYOD; AI auto data discovery; Gen AI control with prompt-level visibility . **Pricing**: **Starting from $1,000/year** per AppDirect listing . **Free tier**: None. **Best for**: Zscaler customers wanting inline DLP with Gen AI controls—**trade-off**: entry pricing is for limited scope; full coverage requires additional modules.

- **[Digital Guardian](https://www.digitalguardian.com/)**
  **Data protection platform** with DLP and insider risk. **Pricing**: Quote-only. **Free tier**: None. **Best for**: enterprises wanting deep endpoint DLP with insider threat focus—**trade-off**: no public pricing; implementation complexity.

- **[Proofpoint Enterprise DLP](https://www.proofpoint.com/)**
  **DLP across email, endpoint, and cloud**. Email DLP is easiest to deploy; endpoint DLP adds SOC features; CASB takes most time to set up with limited cloud API options . **Pricing**: Quote-only per Gartner Peer Insights . **Free tier**: None. **Best for**: Proofpoint email security customers wanting DLP continuity—**trade-off**: visual bugs in DLP scanning reported; CASB setup time-consuming .

- **[Nightfall AI](https://www.nightfall.ai/)**
  **AI-native DLP** with ML-based detection across SaaS, endpoint, and AI tools. **95% detection precision** using transformer-based detectors (not regex); covers PII, PHI, PCI, API keys, source code; **endpoint agent** inspects every browser, desktop app, and AI tool—including unsanctioned apps that no vendor has an API for; **MCP server discovery** with shadow-MCP detection . **Pricing**: Per-user pricing bundles SaaS, endpoint, and AI coverage; **7-day or limited-time POV** instead of self-serve trial; customers report **~50x lower TCO** than legacy DLP . **Free tier**: POV only. **Best for**: modern teams wanting AI-native detection without regex tuning—**trade-off**: SaaS API coverage limited to 12 apps; legacy DLP has broader channel breadth.

- **[Cyberhaven](https://www.cyberhaven.com/)**
  **AI-native data security** tracing data lineage at the fragment level. Targets the "agentic enterprise"—where AI agents copy, summarize, and transform data at machine speed, breaking file-based DLP; **covers Cursor and Claude Code** explicitly; **Deep Understanding** layer pairs lineage with context-aware classification; **Linea AI Detection Agents** flag risky handling in real time . **Pricing**: **Custom quote**; enterprise bracket; costs scale with endpoints, connectors, and modules . **Free tier**: None. **Best for**: regulated enterprises with audit obligations wanting lineage evidence for AI-era data flows—**trade-off**: enterprise infrastructure; deployment depends on integration footprint .

## Open-Source GitHub Projects

- **[onprem-dlp](https://github.com/portable-genai/onprem-dlp)**
  **On-prem DLP gate before cloud egress** (Apache-2.0) — **the most purpose-built open-source DLP tool** found in this research, designed to scrub data **before** it reaches any cloud LLM or API . **Features**: **Runs entirely on-prem, CPU-only**—no byte reaches the cloud unless the gate says so. **Two solutions**: **Unstructured** (text + images)—detects PII in free text and images via OCR, then redacts (tag/mask/hash/remove) or black-boxes pixel regions, issuing an **ALLOW / REDACT / BLOCK** egress decision; **Structured** (database columns)—profiles CSV/SQLite/PostgreSQL/MySQL/BigQuery columns (name, value patterns, cardinality, type, null ratio) and classifies each as `PII_DIRECT` / `PII_QUASI` / `SENSITIVE` / `NON_PII` with explainable weighted signals . **Detection core**: pure stdlib regex candidates hardened by **checksum validators** (SG NRIC/FIN, HK HKID, JP MyNumber, AU TFN/ABN/Medicare, credit-card Luhn, IBAN mod-97) with context-word confidence boosting; optional **Google Gemma** (via Ollama or llama.cpp) and **Microsoft Presidio** NER adapters raise recall but **deterministic policy engine always makes the decision** . **Tech stack**: Python (`pip install '.[yaml]'`). **Deploy**: Local, CLI, or FastAPI egress endpoint. **Trade-off**: **Egress gate only**—it prevents data from reaching cloud LLMs/APIs; it does not monitor endpoints, email, or SaaS apps like commercial DLP. **Best for**: teams building AI applications who need to prevent PII from leaking into cloud LLM prompts—especially those with strict data residency requirements or air-gapped environments.

- **[Presidio](https://github.com/microsoft/presidio)**
  **Open-source PII detection and anonymization** (MIT) — **the detection engine that many DLP tools build upon**, maintained by Microsoft. **Features**: **Fast identification** of PII in text, images, and structured data; **modular recognizers** (regex, checksum, NER, custom); **anonymization** with redaction, masking, hashing, and replacement; supports multiple languages . **Tech stack**: Python. **Deploy**: Library, Docker, or API. **Trade-off**: **Detection only**—it identifies and anonymizes PII but does not enforce egress policies or monitor endpoints. **Best for**: developers building custom DLP pipelines who need a proven PII detection foundation.

- **[dlp-scanner](https://github.com/CarterPerez-dev/Cybersecurity-Projects/tree/main/PROJECTS/intermediate/dlp-scanner)**
  **Multi-format data loss prevention scanner** (license per repo) — **a portfolio/learning project** for building DLP scanning logic . **Features**: **Multi-format scanning** (extractors for different file types); **detectors** for sensitive data patterns; **redaction** capabilities; **scoring** and **reporters** for findings; **CLI** interface; compliance-oriented design . **Tech stack**: Python. **Deploy**: CLI. **Trade-off**: **Educational project**—not production-hardened; no egress enforcement or enterprise integrations. **Best for**: developers learning DLP architecture and detection logic—not for production deployment.

### Additional Strong Open-Source Options

- **No mature open-source endpoint DLP exists.** Symantec, Forcepoint, CrowdStrike, and Microsoft dominate endpoint DLP; open-source alternatives focus on egress gates (onprem-dlp) and detection libraries (Presidio), not full endpoint agents.

**Frameworks for building custom systems**: Combine **onprem-dlp** for cloud egress control with **Presidio** for PII detection and **dlp-scanner** as a learning reference—creating a limited open-source DLP stack. **None of these match commercial endpoint DLP's channel coverage or policy enforcement breadth.**

## How to Contribute

1. Fork the repo.
2. Add/edit entries in `README.md` (follow existing format).
3. Include: name, link, 1–2 sentence description, license (for open-source), and whether it's SaaS or open-source.
4. Submit PR with a short explanation.

Star the repo if you find it useful!

## Disclaimer

- This is a **community-curated** list — not exhaustive and not an endorsement.
- DLP platforms handling sensitive data and policy enforcement must comply with data protection regulations (GDPR, CCPA, HIPAA, etc.) and implement appropriate access controls and audit logging.
- **The "endpoint DLP" vs. "cloud egress gate" vs. "detection library" distinction is critical.** **CrowdStrike, Symantec, Forcepoint, Microsoft Purview, Netskope, Zscaler, Digital Guardian, Proofpoint, Nightfall, and Cyberhaven** are **commercial DLP platforms**—they monitor endpoints, email, cloud, and network channels with policy enforcement . **onprem-dlp** is a **cloud egress gate**—it prevents data from reaching cloud LLMs/APIs, not endpoints or email . **Presidio** is a **detection library**—it identifies PII but does not enforce policies . **Choose based on whether you need endpoint coverage, egress control, or detection capabilities.**
- **Microsoft Purview is critical for M365 Copilot deployments.** Without sensitivity labels and DLP, Copilot exposes over-shared content to unauthorized users. **E3 gets basic DLP; E5 Compliance ($12/user) or E5 ($60/user) is required for full functionality** including Insider Risk and Advanced eDiscovery . **Budget for E5 if deploying Copilot.**
- **Nightfall's 95% detection precision is ML-based, not regex.** Customers report **~50x lower TCO** than legacy DLP because analyst time on false positives drops dramatically . **The trade-off**: SaaS API coverage limited to 12 apps; endpoint agent required for full coverage.
- **Cyberhaven targets the "agentic enterprise"**—it traces data fragments, not files, and explicitly covers Cursor and Claude Code . **The trade-off**: enterprise infrastructure; deployment depends on integration footprint. **For regulated companies with AI adoption and audit obligations, it is a serious shortlist entry.**
- **Symantec DLP's per-user pricing is among the lowest entry points** ($1.99–$14/user/year) but support quality and scanning speed are frequent complaints . **Forcepoint is the IDC Leader** but quote-only with 1–2 FTE-months of tuning .
- **onprem-dlp is the only open-source DLP gate for cloud egress.** It runs CPU-only, on-prem, with deterministic checksum-validated detection and optional Gemma/Presidio adapters . **For teams building AI apps that must not leak PII to cloud LLMs, it is the most purpose-built option.**
- **Pricing opacity varies.** CrowdStrike, Symantec, Zscaler, and Microsoft publish per-endpoint or per-user pricing. Forcepoint, Netskope, Digital Guardian, Proofpoint, Nightfall, and Cyberhaven require sales contact or quote requests. **Validate with direct vendor conversations against your channel coverage needs and user count.**
- Self-hosted open-source solutions require proper infrastructure (Python for onprem-dlp and Presidio), security hardening, and ongoing maintenance. **DLP tools inspect sensitive data**—ensure your deployment meets your organization's privacy and compliance requirements before connecting production data flows.

---

**Made for security engineers, data protection teams, and organizations building transparent DLP solutions.**
Let's make Data Loss Prevention more open, data-driven, and egress-aware.
