# Legalcode Skills Catalogue

250 installable skills: the existing 50-skill selection plus 200 Legalcode-authored additions.

The additions comprise 130 general workflows and 70 bespoke workflows across 18 jurisdiction or regional groups.

See [selection criteria and provenance](selection-2026-09.json) and [file integrity manifest](catalog.json).

This is a curated publication inventory, not a certification of current legal accuracy. Verify primary authorities when using a skill.

## Existing collection (50)

### [legalcode-ai-governance-framework-builder](skills/legalcode-ai-governance-framework-builder/SKILL.md)

Builds comprehensive organizational AI governance frameworks aligned with ISO/IEC 42001:2023 (AI Management System) and the NIST AI Risk Management Framework (AI RMF 1.0). Covers governance structure (AI ethics committee, RACI matrix, reporting lines), policy development suite (acceptable use, risk classification, procurement, training data), risk management lifecycle (MAP, MEASURE, MANAGE, GOVERN functions), risk-tiered use case approval workflows, model lifecycle management (development, testing, deployment, monitoring, retirement), vendor and third-party AI assessment criteria, AI incident response procedures, and ongoing monitoring and audit programs.

### [legalcode-ai-provisions-reviewer](skills/legalcode-ai-provisions-reviewer/SKILL.md)

Reviews contracts for AI-specific provisions: IP ownership of AI-generated outputs, AI usage restrictions and acceptable-use policies, training data rights (inputs/outputs as training material), liability allocation for AI errors and hallucinations, transparency and explainability requirements, algorithmic audit rights, bias monitoring and disparate impact obligations, human oversight and human-in-the-loop requirements, AI governance and responsible-AI clauses, and missing AI governance terms. Flags contracts that lack adequate AI safeguards, identifies one-sided AI risk transfers, generates redlines, and produces a confidence-scored, auditable AI governance analysis.

### [legalcode-aml-kyc-compliance](skills/legalcode-aml-kyc-compliance/SKILL.md)

Design, assess, and gap-analyse Anti-Money Laundering and Know Your Customer compliance programs covering: Customer Due Diligence (CDD) and Enhanced Due Diligence (EDD) procedures; beneficial ownership identification (FinCEN CDD Final Rule 31 C.F.R. § 1010.230, Corporate Transparency Act, EU AMLD/AMLR, UK MLR 2017); sanctions screening (OFAC SDN/50% rule, EU Consolidated List, UK OFSI, UN Security Council); Politically Exposed Person (PEP) identification and risk rating; Suspicious Activity Report (SAR) filing procedures (30/60-day deadlines, tipping-off prohibition); Currency Transaction Report (CTR) filing ($10,000 threshold, structuring rules); transaction monitoring rule design (velocity, structuring, behavioral alerts); enterprise risk assessment methodology; BSA/AML five-pillar program governance; employee training requirements; independent audit/testing procedures; and regulatory examination preparation.

### [legalcode-case-timeline-builder](skills/legalcode-case-timeline-builder/SKILL.md)

Build defensible litigation chronologies from document corpora using a dual-path multi-agent pipeline. Process PDFs, Word documents, emails, images, and other evidence formats at scale — converting to markdown, extracting dates, events, entities, and relationships using Claude Haiku workers in parallel, validating sequences with Sonnet, and synthesizing final timelines with Opus. Supports two execution paths: (1) Claude Code CLI scripts (`claude -p --model haiku`) for maximum throughput on large corpora, and (2) in-skill sub-agent fallback via the Task tool when CLI is unavailable. Produces citation-linked master timelines, issue timelines, entity timelines, deadline calendars, and court-ready outputs (FRCP Rule 56 statements, proposed findings of fact) across jurisdictions. Handles 10K+ document corpora with automatic chunking, deduplication, privilege screening, protective order designations, and conflict resolution.

### [legalcode-case-timeline-generator](skills/legalcode-case-timeline-generator/SKILL.md)

Codex orchestration skill for designing or running a case timeline over one or more local folders. Use when the user wants a chronology, event map, or investigative timeline from PDFs, DOCX files, emails, scans, or mixed evidence and wants a canonical JSON plus a portable static HTML report rendered locally.

### [legalcode-cloud-service-agreement-review](skills/legalcode-cloud-service-agreement-review/SKILL.md)

Review cloud and hosted-service agreements (CSA, cloud MSA, SaaS agreement, cloud subscription agreement, cloud order form) — flag deviations, generate confidence-scored redlines, and produce an auditable analysis. Covers service description and scope, SLAs and uptime credits, security commitments, data processing (GDPR Art. 28 / DPA overlay), sub-processors, audit rights, customer data ownership, provider AI training rights, limitation of liability (including data breach super-caps), indemnification, business continuity and DR, exit assistance and data portability (EU Data Act 2023), regulatory compliance allocation (DORA, HIPAA BAA, PCI DSS, FedRAMP), unilateral modification rights, and term and termination. Jurisdiction-agnostic with [JURISDICTION-SPECIFIC] markers. Native Legalcode replacement for imported cloud-service agreement packs.

### [legalcode-contract-comparison](skills/legalcode-contract-comparison/SKILL.md)

Compare two contract versions or compare a contract against an approved template/playbook to detect textual and semantic legal changes, classify risk by clause family, and produce remediation-ready recommendations with fallback language and audit traceability. Use when reviewing counterparty markups, renewal amendments, template drift, procurement paper, M&A diligence batches, or any scenario requiring defensible contract delta analysis.

### [legalcode-contract-playbook-builder](skills/legalcode-contract-playbook-builder/SKILL.md)

Build and continuously improve organization-specific contract negotiation playbooks with approved clause positions, fallback ladders, escalation triggers, approval matrices, and KPI instrumentation. Use when legal, procurement, sales, or commercial teams need a governed system for reviewing and negotiating NDAs, MSAs, SaaS agreements, procurement terms, partner agreements, and other commercial contracts at scale. Supports green/yellow/ red/black positioning, clause-library governance, and auditable decision trails.

### [legalcode-contract-review](skills/legalcode-contract-review/SKILL.md)

Review contracts against your organization's negotiation playbook — flag deviations, generate confidence-scored redlines, and produce an auditable analysis with business impact assessment. Use when reviewing vendor contracts, customer agreements, SaaS agreements, professional services contracts, licenses, partnerships, procurement agreements, or any commercial agreement requiring clause-by-clause analysis against standard positions. Jurisdiction-agnostic with localization markers for any governing law. Supports playbook-based or general-standard review.

### [legalcode-cookie-compliance-audit](skills/legalcode-cookie-compliance-audit/SKILL.md)

Audit cookie and tracking technology implementations for ePrivacy Directive and GDPR compliance. Tests consent banner functionality including pre-consent cookie blocking, granular category controls, reject-all parity with accept-all, consent withdrawal mechanisms, and consent record retention. Identifies tracking technologies beyond cookies (pixels, fingerprinting, local storage, ETags). Evaluates compliance with CNIL, ICO, and EDPB guidance on cookie walls, analytics exceptions, and essential cookie classifications. Covers US state requirements (CCPA opt-out signals, Global Privacy Control, and state universal opt-out mechanisms). Produces remediation checklist with technical implementation guidance and confidence-scored compliance findings. Use when auditing a website, mobile app, or digital platform for cookie consent compliance, preparing for supervisory authority review, or assessing a consent management platform (CMP) implementation.

### [legalcode-cross-border-transfer-assessment](skills/legalcode-cross-border-transfer-assessment/SKILL.md)

Assess the lawfulness of international personal data transfers under GDPR Chapter V, UK GDPR, and Swiss DPA (nDSG). Use when transferring personal data outside the EEA/UK/ Switzerland to a third country; when selecting or validating a transfer mechanism (adequacy decision, SCCs, BCRs, derogations); when building or reviewing a Transfer Impact Assessment (TIA) post-Schrems II; when assessing supplementary technical and organisational measures; when evaluating destination-country surveillance law (FISA 702, EO 12333, CLOUD Act, China PIPL/MPS, India DPDP); when reviewing Binding Corporate Rules for intra-group transfers; or when advising on Art. 49 derogations. Produces a mechanism selection decision, TIA, supplementary measures catalogue, risk classification (LAWFUL/RESTRICTED/UNLAWFUL per transfer), remediation roadmap, and Glass Box audit trail.

### [legalcode-data-processing-agreement-drafter](skills/legalcode-data-processing-agreement-drafter/SKILL.md)

Draft Data Processing Agreements (DPAs) from scratch for controller-to-processor, controller-to-controller (joint), and processor-to-sub-processor relationships. Produces GDPR Article 28-compliant, UK GDPR, CCPA/CPRA service provider, Brazil LGPD, and India DPDP Act-aligned DPA clauses and full agreements with jurisdiction-specific annexes. Covers subject matter and duration, processing instructions and scope limitations, data categories and data subject types, controller/processor obligations, sub-processor management and notification mechanisms, technical and organizational security measures (TOMs), data breach notification SLAs, data subject rights assistance, DPIA and prior consultation support, international data transfer mechanisms (EU SCCs 2021, UK IDTA, adequacy decisions, BCRs), audit and inspection rights, data return and deletion on termination, and liability allocation.

### [legalcode-document-qa](skills/legalcode-document-qa/SKILL.md)

Run a comprehensive quality assurance audit on any legal document — contract, agreement, deed, policy, or court filing — to detect drafting errors before execution or filing.

### [legalcode-dora-compliance-assessment](skills/legalcode-dora-compliance-assessment/SKILL.md)

Assesses EU DORA (Digital Operational Resilience Act, Regulation (EU) 2022/2554) compliance for financial entities covering all five DORA pillars: ICT risk management framework (Chapter II, Articles 5–16); ICT-related incident classification and reporting (Chapter III, Articles 17–23); digital operational resilience testing including Threat-Led Penetration Testing — TLPT (Chapter IV, Articles 24–27); third-party ICT risk management including critical ICT third-party service providers — CTPPs (Chapter V, Articles 28–44); and information sharing arrangements (Chapter VI, Article 45). Maps DORA to NIS2 Directive lex specialis, GDPR Article 32, EBA guidelines, and all 27 finalized regulatory and implementing technical standards (RTS/ITS).

### [legalcode-dpia-generator](skills/legalcode-dpia-generator/SKILL.md)

Build and review Data Protection Impact Assessments (DPIAs) for high-risk processing under GDPR/UK GDPR and aligned privacy regimes. Use when launching new products, AI features, profiling, surveillance, large-scale special-category processing, or new cross-border data uses that may materially impact individuals' rights and freedoms. Produces a defensible trigger decision, risk register, mitigation plan, prior-consultation recommendation, and executive-ready approval package.

### [legalcode-dsar-workflow-builder](skills/legalcode-dsar-workflow-builder/SKILL.md)

Build and execute end-to-end Data Subject Access Request (DSAR) operational workflows covering intake normalization, identity and authority verification, jurisdiction mapping, scope determination, data discovery across all systems, legal basis review, exemption analysis (trade secrets, third-party data, legal privilege, manifestly unfounded/excessive, national security, ongoing investigations), redaction protocols with proportionality review, response assembly, notice drafting, timeline management, and post-dispatch monitoring. Supports GDPR Article 15, CCPA/CPRA, UK GDPR/DPA 2018, LGPD (Brazil), and PIPEDA (Canada). Includes escalation paths, template responses, compliance documentation, and a full Glass Box audit trail. Use when receiving a DSAR or right-to-know request from any individual, managing backlog of open requests, building a DSAR process program, or auditing an existing DSAR response for defensibility.

### [legalcode-due-diligence-report](skills/legalcode-due-diligence-report/SKILL.md)

Structure M&A due diligence findings into executive-ready reports with material risks, deal-breaker identification, negotiation leverage points, closing conditions, and post-closing integration risks. Use when compiling legal due diligence findings into board presentations, legal memoranda, or commercial deal reports for mergers, acquisitions, carve-outs, joint ventures, or corporate investments. Produces audience-differentiated output in three formats — board/executive, legal/counsel, and commercial/deal team — with risk heat maps, remediation recommendations, and a negotiation playbook. Supports US, UK, and EU transactions. Triggers on "due diligence report", "DD report", "findings report", "deal risk summary", "board presentation M&A", "legal DD memo", "red flag report", "deal-breaker analysis", "negotiation leverage DD", "closing conditions", "post-closing integration risk", or "diligence executive summary". Jurisdiction-agnostic with markers for US, UK, and EU variants.

### [legalcode-eu-ai-act-high-risk-compliance](skills/legalcode-eu-ai-act-high-risk-compliance/SKILL.md)

EU AI Act (Regulation 2024/1689) high-risk AI system compliance assessment covering risk classification determination (Annex I and Annex III categories), risk management system requirements (Art. 9), data governance and training data requirements (Art. 10), technical documentation (Art. 11, Annex IV), record-keeping and logging (Art. 12), transparency and provision of information to deployers (Art. 13), human oversight design (Art. 14), accuracy, robustness, and cybersecurity (Art. 15), quality management system (Art. 17), conformity assessment procedures (Art. 43, Annex VI/VII), CE marking and EU declaration of conformity (Art. 49, 71), post-market monitoring (Art. 72), and serious incident reporting (Art. 73).

### [legalcode-eu-directive-analyzer](skills/legalcode-eu-directive-analyzer/SKILL.md)

Extracts a versioned, machine-readable obligation register from any EU directive identified by CELEX or supplied as text. The register is the foundation artefact consumed by every other skill in the seven-skill EU Legislative Compliance suite: the per-Member-State implementation matrix, the Commission-format correlation table, the per-article conformity verdict, the gold-plating detector, the EEA Joint Committee Decision tracker, and the TFEU 258/260 infringement procedure tracker.

### [legalcode-gdpr-legal-basis-assessment](skills/legalcode-gdpr-legal-basis-assessment/SKILL.md)

Systematically assess the appropriate GDPR Article 6 lawful basis for any processing activity — covering consent (Art. 6(1)(a)), contract performance (Art. 6(1)(b)), legal obligation (Art. 6(1)(c)), vital interests (Art. 6(1)(d)), public task (Art. 6(1)(e)), and legitimate interests (Art. 6(1)(f)). Use when selecting a legal basis for new processing, auditing an existing legal basis for GDPR/UK GDPR compliance, refreshing invalidated consent, evaluating basis changes, or building a legal basis register integrated with ROPA requirements. Covers Article 9 special category processing conditions, Article 10 criminal conviction and offence data, and children's data under Article 8.

### [legalcode-indemnification-analysis](skills/legalcode-indemnification-analysis/SKILL.md)

Deep analysis of indemnification provisions across commercial contract types — review indemnification scope (first-party vs. third-party claims), caps and baskets (deductible basket vs. tipping basket, mini-basket thresholds), materiality qualifiers and scrapes, defense and control-of-claim mechanics (duty to defend, right to control defense, right to settle, cooperation obligations, Cumis counsel in US), survival periods by claim type, and interaction with limitation of liability provisions. Evaluates indemnification exposure across IP infringement, confidentiality breach, data protection violations, and regulatory claims. Compares against market standards by contract type (SaaS, M&A, professional services, construction).

### [legalcode-legal-memorandum](skills/legalcode-legal-memorandum/SKILL.md)

Draft objective IRAC/CREAC-structured legal research memoranda with balanced risk assessment, calibrated probability language, and Bluebook/OSCOLA/AGLC citation frameworks. Use when drafting internal predictive research memos, litigation risk assessment memos, deal advisory memos, regulatory compliance memos, or board-ready executive summaries. Produces Glass Box audit-trailed memoranda across US (federal and state), England & Wales, and Australia jurisdictions. Covers issue framing, rule synthesis from statutory and case authority, counterargument steelmanning, probability-weighted conclusions, privilege marking, and mandatory citation verification. Distinguishes settled law from open questions requiring judicial interpretation. Supports multi-issue memos with separate Questions Presented.

### [legalcode-limitation-of-liability-review](skills/legalcode-limitation-of-liability-review/SKILL.md)

Deep analysis of limitation of liability clauses across contract types — review and classify liability caps (aggregate, per-incident, per-claim), excluded damages (consequential, indirect, special, incidental, punitive), carve-outs and super-caps (IP indemnity, confidentiality breach, data breach, willful misconduct, gross negligence, death and personal injury), sole-remedy clauses, and fundamental breach enforceability. Evaluates cap adequacy relative to deal value and risk profile. Compares against market standards for SaaS, professional services, licensing, and procurement agreements. Use when reviewing any commercial agreement with limitation of liability language, when a counterparty proposes aggressive cap levels or broad exclusions, when assessing whether a vendor's LOL clause creates unacceptable risk exposure, or when drafting LOL provisions for any contract type.

### [legalcode-master-services-agreement](skills/legalcode-master-services-agreement/SKILL.md)

Draft and review Master Services Agreements (MSAs) with SOW/Order Form frameworks from both service provider and client perspectives — generate clause-by-clause guidance, flag market deviations, and produce auditable dual-perspective analysis with confidence-scored redlines. Use when drafting or negotiating MSAs, professional services agreements, managed services contracts, IT services agreements, consulting framework agreements, or any engagement model using a master agreement with modular statements of work or order forms.

### [legalcode-mcp-setup](skills/legalcode-mcp-setup/SKILL.md)

Connect the canonical Legalcode MCP endpoint to Claude, ChatGPT, Codex, Cursor, Windsurf, or another MCP-compatible client and verify account-plan access.

### [legalcode-nda-triage](skills/legalcode-nda-triage/SKILL.md)

Screen and triage incoming NDAs — classify as GREEN (standard approval), YELLOW (counsel review), or RED (significant issues) with confidence-scored, auditable analysis. Use when a new NDA arrives from sales, business development, or a counterparty, when assessing NDA risk level before signature, when deciding whether an NDA needs full counsel review, or when routing NDAs through an in-house legal workflow. Jurisdiction-agnostic with localization markers for any governing law. Supports playbook-based or general-standard screening. Produces a structured triage report with Glass Box audit trail.

### [legalcode-nis2-compliance-assessment](skills/legalcode-nis2-compliance-assessment/SKILL.md)

NIS2 Directive (EU 2022/2555) compliance assessment for essential and important entities covering entity classification (essential vs. important), all ten Article 21 risk management measures, Article 23 incident reporting obligations (24-hour early warning, 72-hour notification, one-month final report), Article 32 board accountability and training mandates, supply chain security requirements, cross-border cooperation, and intersection with GDPR, DORA, and sector-specific regulations. Use when an organization needs to determine NIS2 applicability, assess compliance posture against the ten risk management measures, design incident reporting procedures, prepare for supervisory examination, or understand member state transposition variations.

### [legalcode-obligation-tracker](skills/legalcode-obligation-tracker/SKILL.md)

Extract, normalize, prioritize, and monitor post-signature contract obligations across executed agreements, amendments, renewals, and incorporated documents. Use when legal, procurement, finance, sales operations, vendor management, and compliance teams need an auditable obligation register with owners, trigger logic, due-date computation, escalation pathways, and confidence-scored outputs. Supports single-contract and portfolio modes, jurisdiction-agnostic with [JURISDICTION-SPECIFIC] markers.

### [legalcode-policy-gap-analysis](skills/legalcode-policy-gap-analysis/SKILL.md)

Compares organizational policies and procedures against applicable regulatory requirements, industry standards, and best practices to identify gaps, conflicts, and areas requiring update. Builds a complete policy inventory; maps required policies across privacy (GDPR Arts. 5/24/32/33/35, CCPA/CPRA, LGPD, DPDP Act 2023, PIPL), cybersecurity (NIS2 Directive 2022/2555 Art. 21, ISO 27001:2022, NIST CSF 2.0, HIPAA Security Rule 45 C.F.R.

### [legalcode-privacy-policy-drafter](skills/legalcode-privacy-policy-drafter/SKILL.md)

Draft, localize, and QA website/app privacy policies and notice-at-collection content across GDPR/UK GDPR, CCPA/CPRA, LGPD, and expanding state/global privacy regimes. Use when launching products, expanding to new jurisdictions, updating data practices, or remediating policy gaps found during audits, enforcement readiness checks, or incident-driven policy refreshes.

### [legalcode-public-search](skills/legalcode-public-search/SKILL.md)

Use the canonical Legalcode connector for primary-source legal research. Discover coverage, inspect facets, search, fetch, analyze, trace, and report coverage gaps.

### [legalcode-redline-generator](skills/legalcode-redline-generator/SKILL.md)

Generate negotiation-ready contract redlines with primary and fallback language, playbook alignment, risk-tiered priorities, and auditable rationale for each edit. Use when reviewing third-party paper, preparing response markups, or standardizing first-pass legal edits across procurement, sales, and legal teams. Supports Word track-changes workflows and clause-by-clause redline strategy under jurisdiction- agnostic guidance with localization markers.

### [legalcode-regulatory-change-tracker](skills/legalcode-regulatory-change-tracker/SKILL.md)

Monitor regulatory landscape changes and assess their impact on organizational compliance posture across privacy, employment, financial services, environmental, AI, and sector-specific regulations. Use when tracking regulatory amendments or new rules, analyzing applicability to your organization, identifying compliance gaps against current policies and procedures, prioritizing remediation workflows, maintaining a regulatory change log, and generating board-ready impact summaries and compliance project plans.

### [legalcode-ropa-generator](skills/legalcode-ropa-generator/SKILL.md)

Generate Article 30 Records of Processing Activities (RoPA) for controllers and processors under GDPR, UK GDPR, Swiss FADP, and Brazil LGPD. Use when creating or auditing a processing register, onboarding a new business unit into a data inventory, assessing ROPA completeness before a supervisory authority audit, building a department-by-department data inventory, or integrating data mapping outputs into a supervisory-authority-ready ROPA format. Supports controller RoPA (Art. 30(1)) and processor RoPA (Art. 30(2)) with distinct mandatory-field coverage, Art. 30(5) SME exemption screening, multi-regime jurisdictional overlays, and machine-readable export hooks. Produces both summary and detailed ROPA formats with completeness scoring and prioritized remediation.

### [legalcode-saas-agreement-drafter](skills/legalcode-saas-agreement-drafter/SKILL.md)

Draft and review SaaS/cloud service agreements from both vendor and customer perspectives — generate clause-by-clause guidance, flag market deviations, and produce auditable dual-perspective analysis with confidence-scored redlines. Use when negotiating SaaS terms, drafting customer-facing service agreements, building vendor playbooks, managing SaaS compliance obligations (GDPR, CCPA, SOC 2, HIPAA BAA), assessing SaaS-specific risk allocation, reviewing subscription mechanics, SLA uptime commitments, data processing obligations, AI training restrictions, data portability, or exit assistance terms. Covers B2B, B2C, and B2B2C models. Jurisdiction-agnostic with localization markers for US, EU, UK, and AU. Produces structured guidance with Glass Box audit trail.

### [legalcode-safe-review](skills/legalcode-safe-review/SKILL.md)

Review YC post-money SAFEs (Simple Agreements for Future Equity) clause-by-clause for founders, investors, and counsel — covering valuation cap mechanics and Company Capitalization denominator, discount rate analysis, MFN clause triggering and scope, pro rata rights (in-form and side letter), conversion mechanics across all trigger events (equity financing, liquidity event, dissolution), amendment and majority-in-interest provisions, and non-standard modifications. Benchmarks every material term against the current YC post-money templates (v1.1/v1.2, February 2023 update) and market data (Carta Q3 2024). Classifies deviations as STANDARD / FLAG / RED FLAG with dual-perspective framing (founder view and investor view). Models ownership percentage at conversion. Identifies template drift (modifications beyond blank-filling).

### [legalcode-sanctions-export-control-screening](skills/legalcode-sanctions-export-control-screening/SKILL.md)

Screen transactions, counterparties, and exports against major international sanctions and export control regimes: OFAC SDN and Consolidated Sanctions Lists (all programs), EU Consolidated Sanctions List, UK OFSI Consolidated List, UN Security Council consolidated lists, BIS Entity/Denied Persons/Unverified/MEU Lists, and DDTC Debarred Parties. Applies the OFAC 50% Rule (SDN-owned beneficial owners), secondary sanctions analysis under CAATSA Sections 228/231/232/233 and CISADA, and Sectoral Sanctions Identifications (SSI) Directive 1-4 analysis for Russia. Covers EAR export classification (ECCN and EAR99), Commerce Control List (CCL) mapping, license exception analysis (STA, ENC, LVS, TMP, TSU, RPL, GOV, and others), Foreign Direct Product Rule (FDPR), Military End-Use Rule (15 C.F.R. § 744.21), and deemed export analysis.

### [legalcode-services-agreement-drafter](skills/legalcode-services-agreement-drafter/SKILL.md)

Draft and review standalone commercial services agreements for defined-scope engagements — fixed-price projects, time-and-materials assignments, milestone-based delivery, and hybrid fee structures. Covers scope of work and deliverable specification, change control, fees and payment (including acceptance testing, disputed invoices, and audit rights), intellectual property ownership and licensing (background/foreground IP, assignment formalities, license-back, moral rights), professional and fitness-for-purpose warranties, limitation of liability, indemnification (IP, data breach, gross negligence), data protection obligations, subcontracting controls, termination (cause, convenience, insolvency), and transition/wind-down assistance.

### [legalcode-startup-formation](skills/legalcode-startup-formation/SKILL.md)

Generates complete Delaware C-Corporation formation packages for founders and counsel. Produces all eight core formation documents: Certificate of Incorporation, Bylaws, Action by Incorporator, Initial Board of Directors Consent, Founders Restricted Stock Purchase Agreements (with vesting schedule), Confidential Information and Invention Assignment Agreements (CIIA), Section 83(b) Election Letters, and Indemnification Agreements. Use when incorporating a startup, forming a Delaware C-Corp, preparing founder documents, setting up founder equity and vesting, protecting company IP, or preparing for a seed or Series A financing. Covers DGCL §§ 102, 108, 109, 141, 145, 151; IRC § 83(b); IRS Form 15620; California Labor Code § 2870; DTSA immunity notice. Validates the complete formation package against VC due diligence standards and common founder mistake patterns.

### [legalcode-statute-analysis](skills/legalcode-statute-analysis/SKILL.md)

Analyze statutes, acts, and regulations section by section — deconstruct structure, parse definitions, classify operative verbs, map exceptions and conditions, assess penalty tiers, determine authority boundaries, flag interpretive ambiguities, and identify implementation consequences. Use when a lawyer, compliance officer, policy analyst, or legal researcher needs to understand what a statute actually says and requires — as distinct from verifying that a citation is in-force (use legalcode-legislation-verification for that). Covers primary legislation, delegated legislation (statutory instruments, regulations, ordinances, executive orders, decrees), and secondary regulatory frameworks. Jurisdiction-agnostic with [JURISDICTION-SPECIFIC] markers; supports common law and civil law systems.

### [legalcode-tabular-review](skills/legalcode-tabular-review/SKILL.md)

Perform a high-volume, citation-backed tabular review across one or more document folders, VDR exports, DMS exports, or mixed document sets. Turn PDFs, DOCX files, scans, and related legal materials into a spreadsheet-style review where each document is a row and each user question is a column. Use when the user wants to compare agreements side by side, run a due diligence matrix, extract structured terms from a portfolio, build a red-flag table, answer a fixed list of questions across many documents, or generate Excel-ready review outputs with source citations, confidence, and verification states. Supports dual execution paths: Claude Code CLI workers (`claude -p --model haiku`) for scale, or Task sub-agents when CLI is unavailable. Jurisdiction-agnostic with [JURISDICTION-SPECIFIC] markers.

### [legalcode-tabular-review-orchestrator](skills/legalcode-tabular-review-orchestrator/SKILL.md)

Orchestrate citation-backed tabular review over one or more local folders by turning a user-supplied question list into a review matrix with one row per document and one column per question. Use when the user wants Codex to actually run the workflow inside this repository: discover files, convert PDFs and DOCX to reviewable text, fan out cheap extraction workers, normalize answers, assemble CSV / Markdown / JSON / XLSX outputs, and preserve cell-level provenance. Prefer this skill over ad hoc scripting whenever the task involves repeated questions across many documents, portfolio review, diligence matrices, or side-by-side extraction from folders.

### [legalcode-term-sheet-analysis](skills/legalcode-term-sheet-analysis/SKILL.md)

Deep analysis of venture capital term sheets across three dimensions: economics (pre/post-money valuation, option pool dilution, liquidation preference multiples and participation mechanics, pay-to-play provisions, anti-dilution weighted-average vs. full-ratchet), control (board composition, protective provisions and veto rights, drag-along/tag-along, information rights, registration rights), and other terms (founder vesting and acceleration, ESOP allocation, exclusivity, no-shop, conditions precedent). Evaluates each term against market benchmarks by stage (seed, Series A–D) and identifies investor-favorable vs. founder-favorable deviations. Models cap table dilution and founder economics across multiple exit scenarios.

### [legalcode-terms-of-service-drafter](skills/legalcode-terms-of-service-drafter/SKILL.md)

Draft and review Terms of Service agreements for SaaS, web, and mobile platforms — generate jurisdiction-compliant terms covering account eligibility, acceptable use, user-generated content licensing, intellectual property, subscription and billing, auto-renewal disclosure, limitation of liability, dispute resolution, and governing law. Use when drafting consumer-facing or B2B platform terms, auditing existing TOS for regulatory compliance gaps, updating TOS for new regulatory requirements (DSA, DMA, UK DMCCA, AU unfair terms, US auto-renewal laws), creating B2B vs B2C variants, or generating jurisdiction-specific supplements for EU, UK, AU, CA, and US.

### [legalcode-third-party-due-diligence](skills/legalcode-third-party-due-diligence/SKILL.md)

Conduct anti-corruption due diligence on agents, distributors, joint venture partners, consultants, and other third-party intermediaries. Covers risk tiering, red flag analysis, due diligence questionnaire (DDQ) design, sanctions and debarment screening, contractual anti-corruption provisions, and ongoing monitoring. Aligns with DOJ FCPA guidance and DOJ Guidelines for Evaluation of Corporate Compliance Programs, UK Bribery Act 2010 Section 7 "adequate procedures" and Ministry of Justice six principles, OECD Good Practice Guidance on Internal Controls Ethics and Compliance, and World Bank / multilateral development bank debarment framework.

### [legalcode-vendor-privacy-assessment](skills/legalcode-vendor-privacy-assessment/SKILL.md)

Conduct comprehensive privacy risk assessments of third-party vendors and service providers. Use when onboarding new vendors, renewing vendor contracts, responding to procurement due diligence requests, conducting periodic vendor audits, evaluating vendors following a breach incident, reviewing sub-processor chains, assessing vendor acquisitions, or responding to regulatory inquiries about supplier oversight.

### [legalcode-workflow-compound](skills/legalcode-workflow-compound/SKILL.md)

Extract and store learnings from completed legal and knowledge work to make the next task easier. Use after completing any significant piece of legal work — transactions, litigation milestones, regulatory filings, contract negotiations, compliance audits, corporate governance actions — to capture patterns, create templates, update preferences, and compound institutional legal knowledge. Triggers on requests like 'that went well, let's capture what worked', 'what did we learn from that deal/case/negotiation', 'that motion failed — let's analyze why', or after completing high-stakes legal work. Supports 11 insight types including 6 legal-specific types (precedent, clause-library, jurisdiction-note, regulatory-update, opposing-counsel-pattern, judge-pattern) with privilege-safe storage, ethical obligation compliance, and legal knowledge compounding across matters.

### [legalcode-workflow-research](skills/legalcode-workflow-research/SKILL.md)

Research and plan legal and knowledge work tasks thoroughly before execution. Use when starting any significant legal matter — contract review, regulatory compliance analysis, litigation preparation, corporate governance review, IP/patent analysis, M&A due diligence, employment law matters, data privacy assessments (GDPR/CCPA/LGPD), or any high-stakes knowledge work requiring structured research. Triggers on requests like 'help me prepare for', 'I need to draft', 'plan out', 'research this legal question', 'analyze this contract', 'assess regulatory risk', or any compound legal or knowledge work. Jurisdiction-agnostic with localization markers for any governing law. Produces confidence-scored, auditable research plans with Glass Box reasoning trail.

### [legalcode-workflow-review](skills/legalcode-workflow-review/SKILL.md)

Run parallel multi-agent review on completed knowledge work with deep legal domain expertise. Use after the work phase to evaluate output quality from multiple specialized perspectives before finalizing. Triggers on requests like 'review this', 'check this before I send it', 'stress-test this recommendation', 'review this contract', 'check this brief', 'audit this filing', or when quality assurance is needed on a deliverable. Supports general knowledge work review and specialized legal work review including contracts, memoranda, court filings, regulatory submissions, corporate resolutions, and compliance deliverables. Produces a severity-classified, auditable review synthesis with legal-specific quality gates.

### [legalcode-workflow-work](skills/legalcode-workflow-work/SKILL.md)

Execute a knowledge work plan efficiently while maintaining quality, with deep legal domain expertise for contract drafting, legal memoranda, court filings, regulatory submissions, corporate governance, and compliance operations. Use after the research phase to systematically work through a plan using the right agents for each step. Triggers on requests like 'execute the plan', 'draft that contract we planned', 'go ahead and write the memo', 'prepare the filing', or when moving from planning to execution. Supports both general knowledge work and legal-specific work types with precision-of-language standards, defined terms consistency, cross-reference integrity, and privilege preservation.

## General / Banking Finance (3)

### [legalcode-consumer-lending-compliance](skills/legalcode-consumer-lending-compliance/SKILL.md)

Assess consumer lending programs and loan portfolios for regulatory compliance across the US, UK, and EU. Covers Truth in Lending Act (TILA) / Regulation Z (APR disclosure, ATR/QM rule, HOEPA, TRID), Equal Credit Opportunity Act (ECOA) / Regulation B (adverse action notices, anti-discrimination), Fair Lending (Fair Housing Act, disparate treatment, disparate impact, HMDA), Real Estate Settlement Procedures Act (RESPA) (Section 8 kickback prohibitions, mortgage servicing), state usury laws and rate caps (MLA 36% MAPR, SCRA 6%, NBA preemption), CFPB UDAAP, UK FCA Consumer Credit sourcebook (CONC), Consumer Credit Act 1974 (CCA 1974), FCA Consumer Duty (PS22/9), high-cost short-term credit (HCSTC) price cap, EU Consumer Credit Directive (CCD1 / CCD2 — application November 2026), Mortgage Credit Directive (MCD), and GDPR Article 22 automated credit decisions.

### [legalcode-fintech-regulatory-assessment](skills/legalcode-fintech-regulatory-assessment/SKILL.md)

Assess fintech regulatory compliance across four major jurisdictions — US, UK, EU, and Singapore.

### [legalcode-security-collateral-review](skills/legalcode-security-collateral-review/SKILL.md)

Review security interest packages and collateral documentation across US, UK, and EU jurisdictions. Covers UCC Article 9 (attachment, perfection by filing/control/possession, priority rules, PMSI super-priority, fixture filings, continuation statements, 2022 digital asset amendments), deposit account control agreements (DACAs), investment property control, IP security interests (copyright §205 Copyright Office recordation, patent/trademark UCC vs. federal preemption circuit split), UK fixed and floating charges (Companies Act 2006 ss.859A-859Q registration, Re Spectrum Plus [2005] UKHL 41 fixed/floating test, crystallization), UK financial collateral (FCARs 2003), all-asset debentures, real property mortgages and deeds of trust (recording, SNDAs, Garn-St.

## General / Compliance (38)

### [legalcode-accessibility-compliance](skills/legalcode-accessibility-compliance/SKILL.md)

Assesses digital and physical accessibility compliance for websites, mobile apps, software, and built environments under the Americans with Disabilities Act Title III (42 U.S.C. §12181 et seq.), ADA Title II DOJ Final Rule (April 2024 WCAG 2.1 AA mandate), Section 508 of the Rehabilitation Act (29 U.S.C. §794d), WCAG 2.1 and WCAG 2.2 (Level A/AA/AAA), and the EU European Accessibility Act 2025 (Directive 2019/882 / EN 301 549). Covers website and mobile app technical audits, VPAT/ACR documentation, reasonable accommodation analysis, architectural barrier assessment under the ADA 2010 Standards for Accessible Design, and remediation planning with IMMEDIATE/NEAR-TERM/BACKGROUND prioritization.

### [legalcode-ai-acceptable-use-policy](skills/legalcode-ai-acceptable-use-policy/SKILL.md)

Drafts or reviews an organization's AI Acceptable Use Policy (AUP) — governing which AI tools employees may use, under what conditions, and with what safeguards. Covers permitted and prohibited AI uses, data handling restrictions (confidential information, PII/PHI, privileged communications), employee disclosure obligations for AI-generated content, intellectual property considerations for AI-generated work product, ethical walls between AI-assisted and human-only processes, security requirements for AI tool access, training and certification obligations, incident reporting for AI errors and bias, accountability and oversight requirements, and vendor-specific guidance for ChatGPT/OpenAI, Claude/Anthropic, Microsoft Copilot, and Google Gemini.

### [legalcode-ai-fundamental-rights-impact-assessment](skills/legalcode-ai-fundamental-rights-impact-assessment/SKILL.md)

Conduct Fundamental Rights Impact Assessments (FRIA) as required under EU AI Act Art. 27 (Regulation 2024/1689) for deployers of high-risk AI systems. Applies to public authorities deploying any Annex III system (excluding Point 2 critical infrastructure), private entities providing public services (education, healthcare, social services, housing, justice), and financial sector deployers of creditworthiness or insurance-pricing AI. Assesses impact across the full EU Charter of Fundamental Rights: human dignity (Art. 1), privacy and data protection (Arts. 7-8), freedom of expression (Art. 11), equality and non-discrimination (Art. 21), rights of the child (Art. 24), rights of the elderly (Art. 25), persons with disabilities (Art. 26), right to good administration (Art. 41), and right to an effective remedy (Art. 47).

### [legalcode-ai-in-employment-compliance](skills/legalcode-ai-in-employment-compliance/SKILL.md)

Assess and remediate compliance with laws governing AI and automated decision-making in employment and hiring contexts. Use when deploying, auditing, or advising on AI systems used for candidate screening, interviewing, hiring, promotion, compensation, workforce monitoring, or employee evaluation.

### [legalcode-anti-bribery-compliance](skills/legalcode-anti-bribery-compliance/SKILL.md)

Assess, build, or remediate an organization's anti-bribery and anti-corruption (ABAC) compliance program against the major international regimes: US Foreign Corrupt Practices Act (FCPA) anti-bribery provisions, books-and-records, and internal controls requirements; UK Bribery Act 2010 including the Section 7 corporate offence and adequate procedures defense; France Sapin II (Law No. 2016-1691) mandatory compliance program obligations and Agence Française Anticorruption (AFA) guidelines; and Brazil Clean Company Act (Lei 12.846/2013).

### [legalcode-antitrust-merger-review](skills/legalcode-antitrust-merger-review/SKILL.md)

Analyzes pre-merger notification obligations and merger control strategy for transactions subject to antitrust review. Covers US HSR Act notification requirements, EU Merger Regulation (EC 139/2004) jurisdictional thresholds and clearance process, UK CMA review under the Enterprise Act 2002, market definition methodology (SSNIP/hypothetical monopolist test), competitive effects analysis (unilateral, coordinated, vertical, and conglomerate effects), gun-jumping risk management, remedy strategy (structural vs. behavioral), multi-jurisdictional coordination, and deal-timeline planning. Use when advising on M&A antitrust clearance, conducting pre-signing antitrust risk assessments, preparing HSR filings, negotiating merger remedies, managing parallel competition authority reviews, or counseling on standstill obligations and clean-team protocols. Jurisdiction-specific coverage of US (FTC/DOJ), EU (European Commission DG COMP), and UK (CMA).

### [legalcode-biometric-data-compliance](skills/legalcode-biometric-data-compliance/SKILL.md)

Assess biometric data privacy compliance across Illinois BIPA (740 ILCS 14), Texas CUBI (Tex. Bus. & Com. Code § 503.001), Washington My Health MY Data Act (HB 1155, 2024), California CCPA/CPRA sensitive PI framework, Colorado CPA (HB 24-1130, effective July 1, 2025), GDPR Article 9 special category processing, UK GDPR, and emerging US state laws (New York S1422 proposed, Massachusetts, Virginia, Connecticut biometric provisions). Covers: consent and written release requirements, written biometric data policy and retention/destruction schedules, sale and profit prohibitions, third-party disclosure controls, vendor/processor contractual obligations, individual rights response procedures, DPIA requirements for GDPR high-risk processing, FTC risk assessment standards, incident response obligations, and penalty exposure modeling.

### [legalcode-breach-affected-party-communication](skills/legalcode-breach-affected-party-communication/SKILL.md)

Drafts and reviews the complete suite of breach communications directed at affected individuals and the public following a confirmed personal data breach: individual notification letters with jurisdiction-specific mandatory content, timing, and credit monitoring offers; FAQ documents for breach response webpages; call center scripts; media statements; and follow-up / supplementary notifications. Use when you need to draft, review, or improve any communication sent to data breach victims — not regulatory filings (use legalcode-breach-regulatory-notification-drafter for those).

### [legalcode-breach-severity-assessment](skills/legalcode-breach-severity-assessment/SKILL.md)

Run multi-jurisdiction personal-data breach severity assessments for legal/privacy and incident-response teams. Use when triaging a security incident to decide whether it is notifiable, who must be notified, when clocks start, and how to produce a defensible regulator-ready and executive-ready decision package. Covers global incidents, parallel regulator duties, confidence-scored findings, and auditable timeline logic.

### [legalcode-compliance-program-builder](skills/legalcode-compliance-program-builder/SKILL.md)

Build comprehensive corporate compliance programs aligned with DOJ Evaluation of Corporate Compliance Programs (ECCP) September 2024, UK Ministry of Justice Adequate Procedures under the Bribery Act 2010 (MoJ Six Principles), ISO 37301:2021 Compliance Management Systems, US Sentencing Guidelines §8B2.1 seven elements, and Transparency International Business Principles for Countering Bribery. Use when building a new compliance program from scratch, assessing and maturing an existing program, preparing for DOJ/SFO enforcement defense, pursuing ISO 37301 certification, or producing board-level compliance program assessment documentation.

### [legalcode-consent-mechanism-review](skills/legalcode-consent-mechanism-review/SKILL.md)

Reviews consent collection mechanisms for validity under GDPR Article 7, EDPB Guidelines 05/2020 on consent, and EDPB Guidelines 03/2022 on deceptive design patterns. Detects dark patterns including pre-ticked boxes (Planet49), bundled consent, cookie walls, forced consent, asymmetric button design, confirmshaming, withdrawal obstruction, and consent fatigue tactics. Evaluates all four validity conditions — freely given, specific, informed, and unambiguous — plus withdrawal parity (Article 7(3)) and proof burden (Article 7(1)). Covers consent granularity (purpose-by-purpose), children's consent under Article 8 with national age thresholds, explicit consent for Article 9 special categories, power-imbalance contexts (employment, public authorities, large platforms), and consent refresh triggers.

### [legalcode-coppa-compliance-assessment](skills/legalcode-coppa-compliance-assessment/SKILL.md)

COPPA compliance assessment for operators of websites and online services directed to children or with actual knowledge of child users. Covers the Children's Online Privacy Protection Act (15 U.S.C. §§ 6501–6506) and the FTC's COPPA Rule (16 C.F.R. Part 312), including the 2025 amendments (effective June 23, 2025; compliance deadline April 22, 2026). Assesses all five operator obligation domains: (1) privacy notice requirements including new retention disclosure mandate; (2) direct notice to parents; (3) verifiable parental consent (VPC) including all 10 approved methods and new separate consent for third-party sharing, targeted advertising, and AI training; (4) parental access and deletion rights; and (5) children's data security including the new written information security program requirement.

### [legalcode-corporate-governance-audit](skills/legalcode-corporate-governance-audit/SKILL.md)

Audit corporate governance frameworks against US SOX Sections 302 and 404, UK Corporate Governance Code 2024, EU Shareholder Rights Directive II (2017/828/EU), and German Corporate Governance Code (DCGK). Covers board composition and independence, committee structure (audit, compensation, nomination), executive compensation disclosure and clawback, internal controls over financial reporting (ICFR), risk oversight, related-party transaction governance, and shareholder engagement. Use when preparing for SEC examination, shareholder activism, IPO governance readiness, annual proxy season, post-M&A board integration, or routine governance health checks. Applies to listed companies subject to US SEC rules, UK FCA/LSE premium listings, EU-listed entities under SRD II, and German AktG companies. Produces compliance-classified findings with remediation roadmaps, board mandate templates, and a Glass Box audit trail. Jurisdiction-agnostic core with US/UK/EU/DE specific modules.

### [legalcode-data-mapping-workflow](skills/legalcode-data-mapping-workflow/SKILL.md)

Conduct end-to-end data mapping exercises to build Records of Processing Activities (RoPA) compliant with GDPR Article 30, CCPA/CPRA, LGPD, PIPEDA, and APPI. Use when creating or refreshing a privacy data inventory, onboarding a new DPO, preparing for a DPIA, responding to a regulator inquiry, conducting a vendor privacy audit, or building breach-response readiness. Covers data inventory methodology (interviews, automated scanning, questionnaires), system-by-system data flow documentation, classification of personal data categories and special categories (GDPR Art. 9), legal basis mapping per processing activity, retention schedule alignment, third-party sharing and cross-border transfer identification, and completeness scoring. Produces machine-readable data maps (structured tables + YAML/JSON hooks) suitable for OneTrust, TrustArc, Privaci, and other privacy management platforms.

### [legalcode-dpa-review-and-negotiation](skills/legalcode-dpa-review-and-negotiation/SKILL.md)

Review and negotiate Data Processing Agreements (DPAs) clause-by-clause against GDPR Article 28 mandatory requirements, UK GDPR equivalents, CCPA/CPRA service provider contract provisions, and LGPD operator obligations. Covers subject matter and duration, nature and purpose of processing, data categories and data subject types, controller instructions mechanism, confidentiality of personnel, sub-processor controls (specific and general authorization), security obligations (Art. 32 / technical and organizational measures), data subject rights assistance, DPIA and prior-consultation support, breach notification requirements, audit rights, data return and deletion on termination, and international transfer mechanisms (EU SCCs, UK IDTA, adequacy decisions). GREEN/YELLOW/RED classification with confidence scores, redline suggestions, fallback positions, and negotiation priority tiers.

### [legalcode-eea-incorporation-tracker](skills/legalcode-eea-incorporation-tracker/SKILL.md)

Tracks the European Economic Area (EEA) Joint Committee Decision (JCD) process for incorporating EU acts into the EEA Agreement so that they apply in Iceland, Norway, and Liechtenstein on the EFTA pillar. Operates against the EEA Agreement's two-pillar architecture (Art. 7 EEA on incorporation; Art. 102 EEA on the JCD procedure with its six-month timeline and "serious difficulty" clause; Art. 103 EEA on constitutional reservations and the suspension of entry into force pending parliamentary approval), the Surveillance and Court Agreement (Art. 31 SCA mandating ESA monitoring; Art. 32 SCA on referral to the EFTA Court — the EFTA-pillar mirror of TFEU Art. 258), and the homogeneity principle that drives the EFTA Court to track CJEU jurisprudence.

### [legalcode-employee-handbook-review](skills/legalcode-employee-handbook-review/SKILL.md)

Review employee handbooks and policy manuals for legal compliance, policy gaps, and liability-creating language. Use when onboarding as HR counsel, conducting an annual compliance audit, after a merger or acquisition, when entering a new state, or after a significant statutory change. Covers US federal baseline (Title VII, ADA, ADEA, FMLA, NLRA, FLSA, OSHA, GINA, USERRA, PUMP Act, PWFA), multi-state analysis for distributed workforces, UK requirements (ERA 1996, Equality Act 2010, Employment Rights Act 2025), and Australian requirements (Fair Work Act 2009 NES, positive duty, right to disconnect). Classifies each policy area as COMPLIANT, UPDATE REQUIRED, NON-COMPLIANT, or CRITICAL RISK. Produces a prioritized remediation checklist with model policy language, a multi-state compliance matrix, and a Glass Box audit trail. Supports multi-state operations with jurisdiction-specific supplement analysis.

### [legalcode-environmental-compliance-review](skills/legalcode-environmental-compliance-review/SKILL.md)

Reviews environmental compliance obligations across US, EU, and UK regulatory frameworks.

### [legalcode-eu-conformity-assessment](skills/legalcode-eu-conformity-assessment/SKILL.md)

Runs the substantive, per-provision conformity assessment of a Member State's National Implementing Measures (NIM) against the operative obligations of an EU directive. For each obligation extracted by `legalcode-eu-directive-analyzer` and mapped by `legalcode-eu-correlation-table-builder`, this skill applies the Commission's published methodology — the Better Regulation Toolbox 2023 (Chapter 4: Compliance, Implementation and Preparing Proposals) and the conformity-assessment template used in published Commission tenders such as the ECN+ Directive (Directive (EU) 2019/1, CELEX 32019L0001) tender (Belgian publication reference 765714) — to classify each provision as correctly transposed, partially transposed, incorrectly transposed, or not transposed. Anchors the binding-as-to-result test in Article 288(3) TFEU and the duty of sincere cooperation in Article 4(3) TEU.

### [legalcode-eu-correlation-table-builder](skills/legalcode-eu-correlation-table-builder/SKILL.md)

Generates the Commission-required two-column correlation table that every Member State must submit alongside its transposition notification under Art. 288 TFEU and the Joint Political Declarations of 28 September 2011 (OJ C 369, 17.12.2011, p. 14) and 27 October 2011 (OJ C 369, 17.12.2011, p. 15) on explanatory documents. Maps each operative provision of an EU directive — for example, NIS2 Directive (Directive (EU) 2022/2555, CELEX 32022L2555, OJ L 333, 27.12.2022, p. 80), CSRD Directive (EU) 2022/2464 (CELEX 32022L2464), CSDDD Directive (EU) 2024/1760 (CELEX 32024L1760), or the Whistleblower Protection Directive 2019/1937 — to the corresponding provision(s) in a Member State's National Implementing Measure (NIM).

### [legalcode-eu-gold-plating-detector](skills/legalcode-eu-gold-plating-detector/SKILL.md)

Detects "gold-plating" in a Member State's National Implementing Measure (NIM) for an EU directive — that is, situations where the national text imposes additional scope, requirements, sanctions, or deadlines beyond the EU minimum, fails to use available derogations or opt-outs, or omits review and sunset clauses included in the directive. Operates on the published five-category taxonomy from the Commission High Level Group on Administrative Burden (HLG, 2014 conclusions and recommendations on gold-plating) and from the UK BIS Gold-Plating Review (2013). Anchors burden quantification on the German Nationaler Normenkontrollrat (NKR) cost-opinion methodology and the Standard Cost Model (SCM). Cross-references the Austrian Anti-Gold-Plating-Gesetz 2019 (BGBl.

### [legalcode-eu-infringement-procedure-tracker](skills/legalcode-eu-infringement-procedure-tracker/SKILL.md)

Tracks the infringement-procedure timeline for a Member State / directive pair under TFEU Art. 258 (letter of formal notice → reasoned opinion → CJEU referral) and TFEU Art. 260 (judgment compliance, second-stage lump-sum and periodic-penalty proceedings, and the post-Lisbon Art. 260(3) first-referral penalty for non-notification of transposition of a legislative directive). Mirrors the procedure for EFTA-pillar EEA States (IS, NO, LI) under the Surveillance and Court Agreement (SCA) Arts. 31–32 before the EFTA Surveillance Authority (ESA) and the EFTA Court.

### [legalcode-eu-transposition-tracker](skills/legalcode-eu-transposition-tracker/SKILL.md)

Maintains the per-Member-State implementation matrix for any EU directive across the 27 EU Member States and (where the act is EEA-relevant) the 3 EEA EFTA states (Iceland, Norway, Liechtenstein). Tracks for each MS-directive pair: the National Implementing Measure (NIM) citation in national identifier format (BGBl, JORF, SFS, Dz.U., Stjtíð. A, etc.), transposition status (planned / draft / partial / complete / overdue), notification status to the Commission under Art. 260(3) TFEU, the directive transposition deadline, and links to the national authoritative source (parliament bill page, official journal entry, ministry portal).

### [legalcode-immigration-work-authorization](skills/legalcode-immigration-work-authorization/SKILL.md)

Guide employer-side immigration and work authorization compliance across the United States, United Kingdom, European Union, Australia, and Canada. Use when advising on or auditing work visa sponsorship (US H-1B, L-1, O-1, TN, E-3; UK Skilled Worker, Global Business Mobility; EU Blue Card, Posted Workers, ICT; Australia SID 482, ENS 186, SESR 494; Canada LMIA, CUSMA, IMP), employment eligibility verification (US I-9/E-Verify; UK right-to-work checks; Australian visa work conditions), employer sponsorship obligations, compliance audits, site visit preparedness, penalty exposure assessment, and immigration data protection. Also triggers for employee mobility planning, cross-border assignment structuring, immigration program design, and workforce compliance reviews. Jurisdiction-specific with multi-jurisdiction comparative analysis.

### [legalcode-incident-response-plan-builder](skills/legalcode-incident-response-plan-builder/SKILL.md)

Build comprehensive Incident Response Plans (IRP) covering the full incident lifecycle: preparation, detection and analysis, containment, eradication, recovery, and post-incident activities. Use when building an IRP from scratch, reviewing or updating an existing plan, responding to a live security incident, or preparing tabletop exercises.

### [legalcode-internal-investigation](skills/legalcode-internal-investigation/SKILL.md)

Guide corporate internal investigations from initial allegation through remediation. Covers: investigation scoping and mandate design; legal hold implementation and litigation-hold notice drafting; investigator selection and independence analysis (in-house vs. outside counsel, conflict screening); attorney-client privilege protection (Upjohn Co. v.

### [legalcode-legitimate-interest-assessment](skills/legalcode-legitimate-interest-assessment/SKILL.md)

Conduct a three-part Legitimate Interest Assessment (LIA) under GDPR Art. 6(1)(f), UK GDPR, and Swiss FADP (nDSG). Use when evaluating whether a controller's legitimate interest can lawfully ground processing under the Purpose test (is the interest lawful, clearly articulated, real and present?), the Necessity test (is processing strictly necessary and proportionate?), and the Balancing test (do controller interests outweigh data subject rights?). Also use when documenting LIA records for supervisory authority review, assessing direct marketing, fraud prevention, employee monitoring, profiling, intra-group transfers, network security, or any other processing relying on Art. 6(1)(f). Covers UK Recognised Legitimate Interests (DUA Act 2025) and Swiss Art. 31(1)(b) FADP overriding private interest. Produces a structured, auditable LIA documentation package with GREEN/YELLOW/RED per-test classification, APPROVED/CONDITIONAL/REJECTED overall outcome, remediation plan, and Glass Box audit trail.

### [legalcode-multi-jurisdiction-privacy-comparison](skills/legalcode-multi-jurisdiction-privacy-comparison/SKILL.md)

Perform a side-by-side comparison of global privacy law requirements for specific processing activities or business operations across 12+ international regimes. Use when assessing multi-country compliance obligations, determining the highest common denominator compliance baseline, identifying cross-regime conflicts, building a global harmonized compliance strategy, conducting pre-market entry privacy due diligence, or advising on international data transfers affecting multiple jurisdictions. Covers GDPR (EU), UK GDPR, CCPA/CPRA (California), LGPD (Brazil), PIPEDA/Bill C-27 (Canada), PIPL (China), PDPA (Singapore), POPIA (South Africa), APPI (Japan), Privacy Act (Australia), DPDP Act (India), and emerging frameworks (Thailand, Indonesia, Vietnam, New Zealand).

### [legalcode-non-compete-analysis](skills/legalcode-non-compete-analysis/SKILL.md)

Cross-jurisdictional router for non-compete enforceability analysis covering US (all 50 states + state-by-state variation, California ban, Colorado salary thresholds, FTC landscape post-Ryan LLC v. FTC vacatur), UK (common law reasonableness test, garden leave, protectable interests, blue-pencil doctrine, 2023/2024 reform landscape), Germany (HGB §§ 74-75a Nachvertragliches Wettbewerbsverbot, mandatory Karenzentschädigung 50% minimum, 2-year cap, unverbindlich vs. nichtig distinction), France (clause de non-concurrence, five cumulative Cour de cassation criteria including mandatory contrepartie financière, employer waiver mechanics, collective bargaining agreement floors), and China (Labor Contract Law Arts. 23-24, mandatory monthly economic compensation, senior management/senior technical staff scope, Supreme Court Interpretation III, 2-year cap).

### [legalcode-open-source-license-compliance](skills/legalcode-open-source-license-compliance/SKILL.md)

Audit open-source software license compliance for any project or dependency inventory. Use when reviewing a software project for OSS license obligations before distribution, when assessing license compatibility in combined works, when evaluating copyleft obligations triggered by binary distribution or SaaS network use, when reviewing contributor license agreements (CLAs) and Developer Certificate of Origin (DCO) frameworks, when generating SBOM documentation to meet EO 14028 or EU CRA (Reg. 2024/2847) requirements, or when designing an enterprise open-source policy.

### [legalcode-pay-equity-audit](skills/legalcode-pay-equity-audit/SKILL.md)

Conducts a comprehensive pay equity audit — from data scoping and similarly situated employee group (SSEG) construction through statistical regression design, LNDF validation, gap classification, remediation budget modeling, and reporting. Use when analyzing workforce compensation for gender, race, or other protected-class pay disparities; preparing for OFCCP contractor audits; complying with California SB 1162, New York pay transparency requirements, Colorado Equal Pay for Equal Work Act, or Illinois EPRC obligations; implementing the EU Pay Transparency Directive (2023/970/EU) joint pay assessment; managing pre-litigation pay equity risk; or building a proactive annual pay equity program. Supports both US multi-state and EU multinational engagements. Covers statistical regression methodology (OLS, adjusted/unadjusted gaps), attorney-client privilege structuring, and remediation waterfall modeling.

### [legalcode-soc2-readiness-assessment](skills/legalcode-soc2-readiness-assessment/SKILL.md)

Assess SOC 2 Type I and Type II readiness across all five AICPA Trust Service Criteria (Security, Availability, Processing Integrity, Confidentiality, Privacy). Use when a SaaS company, cloud service provider, managed service provider, or other service organization needs to determine readiness for a SOC 2 audit, identify control gaps, build a remediation roadmap, or understand how SOC 2 maps to ISO 27001, NIST CSF, HIPAA, or PCI DSS. Covers all Common Criteria (CC1–CC9), optional TSC criteria (A, PI, C, P series), evidence collection requirements per control, management assertion obligations under AT-C Section 205, subservice organization carve-out vs. inclusive method, and Complementary User Entity Controls (CUECs).

### [legalcode-trademark-clearance-search](skills/legalcode-trademark-clearance-search/SKILL.md)

Conducts comprehensive trademark availability searches including identical mark searches, phonetic equivalents, visual similarity analysis, and conceptual similarity assessment across USPTO TESS, EUIPO TMView, WIPO Global Brand Database, UKIPO, IP Australia, and IP India databases plus common law sources. Applies likelihood of confusion analysis using DuPont factors (sight, sound, meaning, commercial impression, channels of trade, consumer sophistication, mark fame). Evaluates descriptiveness/genericness risks, surname doctrine, geographic marks, and acquired distinctiveness arguments. Covers goods/services classification strategy across Nice Classification 45 classes (NCL 13-2026). Produces clearance opinion with risk rating (CLEAR/CAUTION/BLOCKED) and alternative mark recommendations.

### [legalcode-us-breach-notification-triage](skills/legalcode-us-breach-notification-triage/SKILL.md)

Multi-state US breach notification triage covering all 50 states, DC, Puerto Rico, Guam, US Virgin Islands, and American Samoa. Use when a security incident involves personal information of US residents and you need to determine notification obligations: which states require notice, to whom, by when, with what content, and whether any safe harbor (encryption, good-faith acquisition, HIPAA compliance) applies. Covers the full triage lifecycle — PI definition matching, breach definition analysis, clock-start normalization, notification deadline calculation, AG filing thresholds, notice content requirements, substitute notice triggers, credit monitoring obligations, and federal overlay requirements (HIPAA Breach Notification Rule, GLBA Safeguards Rule, SEC Form 8-K Item 1.05, FCC telecom rules, CIRCIA).

### [legalcode-us-state-privacy-comparison](skills/legalcode-us-state-privacy-comparison/SKILL.md)

Compare all enacted US state comprehensive privacy laws to determine applicability, map consumer rights obligations, and produce a compliance gap analysis for multi-state operations. Use when assessing whether your organization is subject to CCPA/CPRA (California), VCDPA (Virginia), CPA (Colorado), CTDPA (Connecticut), UCPA (Utah), ICDPA (Iowa), INCDPA (Indiana), DPDPA (Delaware), TIPA (Tennessee), MCDPA (Montana), NHPA (New Hampshire), NJDPA (New Jersey), OCPA (Oregon), TDPSA (Texas), NDPA (Nebraska), MODPA (Maryland), MCDPA (Minnesota), KCDPA (Kentucky), RIDTPPA (Rhode Island), or any other enacted US state comprehensive privacy law. Produces a threshold analysis table, consumer rights compliance matrix, sensitive data obligations mapping, opt-out mechanism assessment, enforcement risk profile, cure period status, and a prioritized gap analysis with remediation roadmap. Covers all 19 enacted comprehensive state privacy laws as of 2026, including 2025-2026 amendments, new UOOM mandates, and GPC requirements.

### [legalcode-wage-hour-compliance-audit](skills/legalcode-wage-hour-compliance-audit/SKILL.md)

Audits wage and hour compliance under the Fair Labor Standards Act (FLSA) and state equivalents. Use when assessing exempt vs. non-exempt employee classification under duties tests (executive, administrative, professional, computer employee, outside sales, highly compensated), salary threshold compliance (including the post-2024 Texas-court-vacated DOL rule, current operative $684/week threshold), overtime calculation methodology (regular rate inclusions/exclusions, fluctuating workweek, piece rate, blended rates), meal and rest break requirements by state, timekeeping adequacy and off-the-clock risk, tip credit and tip pooling rules (2018 CAA and 2021 DOL final rule), child labor compliance (29 CFR Part 570), predictive/fair scheduling obligations, and pay stub and record-keeping requirements. Produces classification findings by violation tier, quantified exposure estimates, and prioritized remediation recommendations. US federal + state jurisdictions.

### [legalcode-warn-act-analysis](skills/legalcode-warn-act-analysis/SKILL.md)

Analyzes federal WARN Act (29 U.S.C. §§ 2101–2109) and state mini-WARN compliance for plant closings and mass layoffs. Covers covered-employer determination, plant closing and mass layoff triggering thresholds, employment loss definitions, the 90-day rolling aggregation lookback, the three notice-reduction exceptions (faltering company, unforeseeable business circumstances, natural disaster), notice content and delivery requirements, damages calculation (back pay + ERISA benefits + $500/day civil penalty), the single-employer/affiliated-companies doctrine, sale-of-business allocation, WARN in bankruptcy, and remote-worker site-of-employment questions. Maps state mini-WARN variations for California, New York, New Jersey, Maine, Maryland, Minnesota, and Illinois.

### [legalcode-workplace-investigation](skills/legalcode-workplace-investigation/SKILL.md)

Guide workplace investigations end-to-end — from complaint intake and scope determination through investigator assignment, privilege preservation, document hold, witness interview protocols, credibility assessment, findings documentation, remedial action planning, and regulatory reporting. Applies to harassment, discrimination, retaliation, hostile work environment, OSHA/safety complaints, code-of-conduct violations, whistleblower allegations, time-and-attendance fraud, workplace violence, and misconduct investigations. Extends to compliance-driven, fraud, and false-claims investigations that arise in employment contexts.

## General / Contracts (18)

### [legalcode-clause-library-manager](skills/legalcode-clause-library-manager/SKILL.md)

Build, govern, and continuously improve contract clause libraries and negotiation playbooks for legal teams. Use when standardizing preferred clauses, fallback ladders, approval thresholds, and version control across MSAs, SaaS agreements, DPAs, procurement templates, and other recurring commercial contracts. Supports greenfield library creation, library cleanup, merger harmonization, and ongoing clause governance operations.

### [legalcode-commercial-lease-review](skills/legalcode-commercial-lease-review/SKILL.md)

Review commercial lease agreements clause-by-clause against a Letter of Intent and market benchmarks — flag deviations, generate confidence-scored redlines, and produce an auditable analysis covering base rent and escalation, CAM charges and reconciliation rights, tenant improvement allowances, personal guarantees and good-guy clauses, use restrictions and exclusivity, assignment and subletting rights, default and cure periods, landlord access and relocation rights, insurance requirements, environmental obligations, ADA/accessibility compliance, holdover provisions, and early termination and contraction options. Use when reviewing office, retail, or industrial leases; comparing executed lease terms against LOI commitments; or evaluating landlord-side or tenant-side risk exposure before signing, renewal, or dispute.

### [legalcode-construction-contract-review](skills/legalcode-construction-contract-review/SKILL.md)

Review construction contracts clause-by-clause covering scope of work, payment and retainage, change orders and variations, extension of time and delay, liquidated damages, defects liability, insurance, indemnification, limitation of liability, dispute resolution, termination, force majeure, design liability, subcontracting, health and safety, and bonds. Supports standard forms: JCT (UK), NEC4 (UK/international), AIA A201 (US), FIDIC Red Book (international), and AS 4000 (Australia). Applies UK, US, and Australian jurisdiction frameworks. Use when reviewing employer-side or contractor-side construction and engineering contracts, design-build agreements, EPC contracts, subcontracts, and professional services appointments on construction projects. Flags deviations, classifies risk (GREEN/YELLOW/RED), generates redlines, and produces a confidence-scored, auditable analysis.

### [legalcode-contract-amendment-drafter](skills/legalcode-contract-amendment-drafter/SKILL.md)

Drafts contract amendments, addenda, amended and restated agreements, and waivers with production-quality legal language. Generates proper recitals, precise section-modification operative clauses, supersession and integration-plus clauses, effective date provisions, counterpart execution blocks, and surviving-terms confirmations. Performs amendment procedure compliance checks (no-oral-modification clause, signatory authority, consideration requirements). Use when modifying any executed commercial agreement, extending or adjusting contract terms, adding new obligations, documenting an oral arrangement in writing, or consolidating multiple amendments into a restated agreement. Jurisdiction-agnostic with [JURISDICTION-SPECIFIC] markers for US, UK, EU, Australia, and Canada.

### [legalcode-contract-metadata-extractor](skills/legalcode-contract-metadata-extractor/SKILL.md)

Extract structured metadata from contracts and legal documents into a normalized, machine-readable format suitable for CLM systems, databases, and analytics. Use when ingesting contracts into a contract lifecycle management system, building a contract repository, performing portfolio analysis, enabling contract search and discovery, or automating contract data capture. Extracts parties, dates, financial terms, governing law, key clauses, obligations, and risk indicators with confidence scoring and provenance tracking. Jurisdiction-agnostic with [JURISDICTION-SPECIFIC] markers.

### [legalcode-contract-renewal-analysis](skills/legalcode-contract-renewal-analysis/SKILL.md)

Analyze contracts approaching renewal to detect auto-renewal traps, calculate termination window deadlines, identify evergreen clauses, flag price escalation triggers, and produce renewal decision checklists with timeline visualization and cost-benefit analysis. Use when reviewing a contract nearing expiration, evaluating whether to renew, renegotiate, rebid, or terminate, assessing auto-renewal risk, benchmarking renewal pricing, or preparing renewal negotiation strategy. Jurisdiction-agnostic with [JURISDICTION-SPECIFIC] markers. Supports playbook-based or general-standard analysis. Covers SaaS subscriptions, vendor agreements, services contracts, licenses, MSAs, and any commercial agreement with recurring or evergreen terms. Produces a structured renewal decision report with Glass Box audit trail and confidence scoring.

### [legalcode-distribution-agreement-review](skills/legalcode-distribution-agreement-review/SKILL.md)

Review distribution and reseller agreements covering territory exclusivity, minimum purchase commitments (MPC/MAP), pricing and discount structures (including RPM and MFN clauses), marketing obligations and brand standards, IP licenses for trademarks and trade dress (naked licensing risk), termination and post-termination obligations, competition law compliance (EU VBER 2022 / Regulation 2022/720, US Sherman Act Section 1 / Leegin / Sylvania / Colgate doctrine / Robinson-Patman), and channel conflict management (dual distribution, online/offline separation, marketplace bans). Produces clause-by-clause review with EU/US market-standard benchmarks, severity-classified findings, and competition-law compliance screening.

### [legalcode-employment-agreement-review](skills/legalcode-employment-agreement-review/SKILL.md)

Review employment agreements clause-by-clause against market standards or an organizational playbook. Use when evaluating new hire offer packages, executive employment agreements, promotion agreements, or renegotiated employment terms.

### [legalcode-esg-clause-reviewer](skills/legalcode-esg-clause-reviewer/SKILL.md)

Review contracts for ESG (Environmental, Social, Governance) provisions — environmental commitments, carbon targets, net-zero clauses, Scope 1/2/3 emissions obligations, science-based targets, social and labor standards, human rights and modern slavery obligations, governance and anti-corruption requirements, supply chain sustainability due diligence (CSDDD, LkSG, France Devoir de Vigilance, UK Modern Slavery Act), ESG reporting obligations, framework compliance (GRI, SASB, TCFD, CSRD/ESRS, ISSB/IFRS S1/S2, SBTi), ESG representations and warranties, greenwashing and green claims risk, ESG-linked commercial terms and sustainability-linked pricing, ESG material adverse change definitions, biodiversity and circular economy provisions.

### [legalcode-franchise-agreement-review](skills/legalcode-franchise-agreement-review/SKILL.md)

Review franchise agreements and Franchise Disclosure Documents (FDD/disclosure documents) clause-by-clause against regulatory requirements and market standards — flag deviations, generate confidence-scored redlines, and produce an auditable analysis covering initial franchise fees and ongoing royalties, territory rights and exclusivity, intellectual property and trademark licenses, quality control and operations manual compliance, advertising fund contributions, training and support obligations, term and renewal rights, transfer and assignment restrictions, termination and post-termination obligations, non-compete and restrictive covenants, financial performance representations (Item 19), and dispute resolution. Use when reviewing franchise agreements as a prospective franchisee, existing franchisee renegotiating terms, or franchisor ensuring compliance.

### [legalcode-guaranty-agreement-review](skills/legalcode-guaranty-agreement-review/SKILL.md)

Review guaranty and surety agreements for scope, suretyship defenses, subrogation, contribution, and enforceability risks. Use when reviewing personal guaranties, parent company guaranties, corporate guaranties, bank guaranties, bad boy carve-out guaranties, keepwell agreements, or comfort letters in connection with commercial lending, real estate finance, lease transactions, construction finance, or supply chain credit support. Covers continuing vs. specific guaranty analysis, waiver of suretyship defenses (RSG §§ 37-49 / UCC § 3-605), anti-deficiency statute exposure (California CCP §§ 580a-580d, one-action rule CCP § 726), subrogation deferral mechanics, contribution rights among co-guarantors, financial covenants and keepwell provisions, notice requirements, dollar cap and burn-off structures, and reinstatement clause risk.

### [legalcode-ip-assignment-agreement](skills/legalcode-ip-assignment-agreement/SKILL.md)

Review and draft intellectual property assignment agreements transferring ownership of patents, copyrights, trademarks, trade secrets, and know-how. Use when reviewing or drafting IP assignments in employment contexts (invention assignment clauses, employee IP provisions), contractor engagements (consultant IP transfer, freelancer work product), M&A transactions (IP due diligence, founder IP transfer, pre-incorporation assignment remediation), technology transfers (source code assignment, software IP, algorithm transfer), and corporate reorganizations (intra-group IP transfer, spin-off IP allocation). Covers assignment vs. license distinction, present vs. future rights assignment language ("hereby assign" vs. "agree to assign"), work-for-hire doctrine (17 USC 101 nine categories, Community for Creative Non-Violence v.

### [legalcode-lease-abstractor](skills/legalcode-lease-abstractor/SKILL.md)

Extract and summarize key commercial lease terms into a structured abstract for portfolio management, date tracking, financial modeling, and quick reference. Use when building a lease database, onboarding a new lease into a portfolio system, tracking renewal and termination option deadlines, abstracting lease terms for due diligence, or creating a machine-readable lease record for import into Yardi, MRI, CoStar, VTS, Tango, or similar platforms. Produces a 14-category structured abstract covering rent and escalations, CAM and operating expenses, TI allowances, renewal/expansion/termination options, assignment and subletting, co-tenancy, exclusivity, use restrictions, insurance, maintenance, guarantees, SNDA, default and cure periods, and holdover provisions — with extraction confidence scoring, critical date computation, amendment reconciliation, and structured JSON/CSV export.

### [legalcode-loan-agreement-review](skills/legalcode-loan-agreement-review/SKILL.md)

Review loan and credit agreements clause-by-clause from the borrower or lender perspective.

### [legalcode-nda-mutual](skills/legalcode-nda-mutual/SKILL.md)

Draft, review, and negotiate mutual non-disclosure agreements (NDAs) for bilateral business discussions across jurisdictions. Use when users ask for two-way confidentiality agreements, MNDA templates, pre-contract information sharing terms, startup and investor confidentiality clauses, or risk review of definition scope, exclusions, term, compelled disclosure, and remedies. Supports playbook-based or general-standard review with confidence-scored analysis and auditable output. Jurisdiction-agnostic with localization markers for any governing law.

### [legalcode-partnership-agreement-review](skills/legalcode-partnership-agreement-review/SKILL.md)

Review partnership agreements — general partnerships (GP), limited partnerships (LP), and limited liability partnerships (LLP) — covering capital contributions, profit/loss allocation and distribution waterfalls, management authority and reserved matters, partner fiduciary duties, non-compete and non-solicitation obligations, admission and withdrawal of partners, dissolution triggers and winding-up procedures, and tax allocation mechanics. Applies RUPA 1997/2013, ULPA 2001, and Delaware DRULPA for US analysis; Partnership Act 1890, Limited Partnership Act 1907, and LLP Act 2000 for UK analysis; and state-based Partnership Acts plus ITAA 1936 Division 5/5A for Australian analysis.

### [legalcode-supply-chain-contract-review](skills/legalcode-supply-chain-contract-review/SKILL.md)

Review supply and procurement agreements covering pricing mechanisms (fixed, index-linked, MFC/MFN), tariff and customs risk allocation, delivery terms (Incoterms 2020), quality specifications and inspection rights, warranty provisions (UCC Article 2, CISG Art. 35, UK Sale of Goods Act 1979), EU Product Liability Directive 2024/2853 (in force Nov 2024), force majeure and commercial impracticability, supply continuity and business continuity obligations, sustainability and ESG supply chain due diligence (EU CSDDD, UK Modern Slavery Act, US UFLPA, France Devoir de Vigilance, Norway Åpenhetsloven), critical minerals and rare earth traceability (EU CRMA, EU Battery Regulation, Dodd-Frank), supply chain finance integration, and indemnification. Covers UCC Article 2, CISG Arts 25/35/71–79, and UK Sale of Goods Act.

### [legalcode-technology-license-agreement](skills/legalcode-technology-license-agreement/SKILL.md)

Structure, draft, review, and negotiate technology and IP license agreements covering the full commercial deal lifecycle across US, EU, and UK frameworks. Use when drafting a technology license from scratch, reviewing a proposed agreement for deal-term acceptability, or advising on the commercial structure of a patent license, software license, know-how license, technology transfer, or mixed-IP bundle license.

## General / Corporate Transactions (16)

### [legalcode-board-resolution-drafter](skills/legalcode-board-resolution-drafter/SKILL.md)

Drafts board resolutions and unanimous written consents (UWCs) for common corporate actions: officer appointments and removals, equity issuances, stock option and warrant grants (ISO/NSO), equity incentive plan adoptions, financing approvals (debt facilities, convertible notes, SAFEs, preferred rounds), contract authorizations, dividend declarations, bank account authorizations, annual compliance resolutions, IP assignments, subsidiary formations, M&A preliminary approvals, and indemnification agreements. Covers recital/WHEREAS and RESOLVED structure, quorum, unanimous consent mechanics, Secretary certification, and corporate formality requirements under Delaware DGCL §141, UK Companies Act 2006, and MBCA. Deep coverage of IRC §409A FMV requirements for equity grants, Rule 701 securities law compliance, and §280G golden parachute analysis triggers.

### [legalcode-cap-table-review](skills/legalcode-cap-table-review/SKILL.md)

Review, audit, and model cap tables for US startups at any stage — covering SAFE mechanics (post-money vs. pre-money conversion, MFN, pro-rata), convertible note conversion (discount, valuation cap, shadow preferred, interest accrual), option pool sizing and the option pool shuffle, anti-dilution adjustments (broad-based weighted average, full ratchet, narrow-based, pay-to-play, NVCA carve-outs), liquidation waterfall modeling (non-participating, participating, participation cap, liquidation multiples), and dilution scenario modeling across rounds. Identifies cap table errors, missing shadow preferred mechanics, incorrect fully diluted counts, and structural red flags. Benchmarks against NVCA October 2025 model documents and current market standards.

### [legalcode-closing-checklist](skills/legalcode-closing-checklist/SKILL.md)

Generate comprehensive transaction closing checklists covering pre-closing deliverables, conditions precedent tracking, signature page logistics, funds flow and escrow mechanics, post-closing obligations, regulatory filings calendars, and closing binder indexes. Use when managing or preparing for M&A closings (stock purchases, asset purchases, mergers), secured financing closings (credit facilities, bonds, mezzanine), or commercial real estate closings. Triggers on "closing checklist", "pre-closing conditions", "conditions precedent tracking", "closing deliverables", "post-closing obligations", "regulatory filings after closing", "closing binder", "funds flow memo", "bring-down certificate", "officer certificate", "good standing certificate", "UCC filing", "transaction closing", "sign and close", or "deferred closing". Jurisdiction-agnostic with [JURISDICTION-SPECIFIC] markers for US, UK, EU, and international variants.

### [legalcode-convertible-note-review](skills/legalcode-convertible-note-review/SKILL.md)

Review convertible notes and convertible loan notes (CLNs) for founders, investors, and counsel — covering interest accrual and compounding mechanics, maturity and redemption risk, qualified financing definition and threshold, conversion mechanics (discount rate, valuation cap, shadow preferred stock, post-money formula), MFN clause analysis, pro-rata rights, prepayment and subordination provisions, events of default, and amendment consent thresholds. Benchmarks every material term against current market standards (NVCA 2025, Carta Q1 2025, Fenwick/Cooley market data) with dual-perspective framing (founder view and investor view for every economic term). Models cap table dilution from interest accrual and conversion across multiple scenarios.

### [legalcode-corporate-minutes-drafter](skills/legalcode-corporate-minutes-drafter/SKILL.md)

Draft formal meeting minutes for board of directors, shareholder/stockholder, and committee meetings. Use when preparing minutes for any corporate meeting — annual, special, organizational, or written consent — covering attendance and quorum certification, agenda items, motions and voting outcomes, conflict of interest disclosures, committee reports, officer elections, equity and financing approvals, M&A and major transactions, action item assignments, and next-meeting scheduling. Supports US (Delaware, MBCA) and UK (Companies Act 2006) corporations with [JURISDICTION-SPECIFIC] markers for other jurisdictions. Also use when reviewing draft minutes for completeness, documenting written consents in lieu of meeting, or producing the secretary's certification block.

### [legalcode-corporate-restructuring](skills/legalcode-corporate-restructuring/SKILL.md)

Comprehensive corporate restructuring analysis covering US Chapter 11 reorganization (automatic stay §362, DIP financing §364, Section 363 asset sales, cramdown §1129(b), executory contracts §365, avoidance actions §547-548, absolute priority rule, SBRA/Subchapter V small business track), UK administration and CVA (Insolvency Act 1986, Part 26A restructuring plans, cross-class cramdown, pre-pack administration SIP 16, schemes of arrangement), German Insolvenzverfahren and StaRUG (InsO, Eigenverwaltung, Schutzschirmverfahren, ESUG 2012, StaRUG 2021 preventive framework), out-of-court workouts (forbearance, standstill, intercreditor agreements, LSTA/LMA distressed trading), debt-for-equity swaps (COD income, IRC §382 NOL limitations, UK/DE tax rules), Section 363 sales (stalking horse, free and clear, bidding procedures), DIP financing (priming liens, roll-ups, milestones, loan-to-own), Assignment for Benefit of Creditors (ABC), receivership, and liability management exercises (uptier, exchange offers, co-ops).

### [legalcode-data-room-organizer](skills/legalcode-data-room-organizer/SKILL.md)

Organizes and audits Virtual Data Rooms (VDRs) for M&A transactions, debt financing, IPO/capital markets, and venture/growth equity. Generates standard folder taxonomy tailored to transaction type, classifies and tags documents, identifies gaps against comprehensive diligence checklists, produces a numbered VDR index, and recommends granular access permission tiers. Use when setting up a sell-side or buy-side data room, auditing an existing data room for completeness, preparing an information request list, generating a VDR index for transaction documentation, or configuring access controls for multi-bidder auction, competitive financing, or IPO processes.

### [legalcode-equity-incentive-plan-review](skills/legalcode-equity-incentive-plan-review/SKILL.md)

Review equity incentive plans — stock option plans (ISO/NSO), RSU plans, RSA plans, phantom equity, SARs, and performance share plans — clause-by-clause to flag deviations from market standards, generate confidence-scored redlines, and produce an auditable analysis of plan design, 409A compliance, vesting mechanics, acceleration triggers, tax treatment, and SEC registration status. Use when reviewing a company's stock incentive plan, equity compensation plan, LTIP, management incentive plan, option agreement, RSU award agreement, or any equity compensation document.

### [legalcode-founders-agreement-drafter](skills/legalcode-founders-agreement-drafter/SKILL.md)

Draft comprehensive founders agreements covering equity allocation and split methodology, vesting schedules (cliff, acceleration on single/double-trigger change of control), intellectual property assignment with pre-existing IP carve-outs, role definitions and decision-making authority, capital contribution requirements, expense policies, non-compete and non-solicitation obligations, departure mechanics (voluntary, involuntary, for-cause), buyback provisions with valuation methodology, deadlock resolution, and dissolution/wind-down procedures. Use when founding a new company, restructuring founder relationships, preparing for Series A investment, or documenting founding team equity arrangements. Supports multi-jurisdiction formation decisions (Delaware C-Corp, UK Ltd, Singapore Pte Ltd, India Private Limited). Includes explanatory notes for non-lawyer founders. Jurisdiction-aware with [JURISDICTION-SPECIFIC] markers. Produces playbook-integrated, investor-ready draft sections with Glass Box audit trail.

### [legalcode-joint-venture-agreement](skills/legalcode-joint-venture-agreement/SKILL.md)

Drafts and reviews joint venture agreements covering governance structure, board composition and voting thresholds, capital contributions, profit and loss allocation, management rights, deadlock resolution mechanisms (Russian roulette, Texas shoot-out, expert determination), non-compete obligations, exit strategies (put/call options, ROFO/ROFR, shotgun clauses, tag-along/drag-along), intellectual property ownership and licensing (background IP/foreground IP), and dissolution procedures. Addresses tax structuring implications across entity types. Primary coverage: US (Delaware LLC and C-Corp structures), UK (England and Wales companies/LLPs), EU (cross-border JVs and merger control), and India (Companies Act 2013 / FEMA compliance).

### [legalcode-letter-of-intent-review](skills/legalcode-letter-of-intent-review/SKILL.md)

Review letters of intent (LOIs), memoranda of understanding (MOUs), term sheets, heads of terms, and agreements in principle for corporate transactions. Identifies binding vs. non-binding provisions, assesses enforceability risks from purportedly non-binding language, and flags provisions creating unintended binding obligations. Analyzes exclusivity and no-shop clauses (scope, duration, fiduciary-out carveouts, penalty for breach), break-up fees and reverse break-up fees (trigger events, market benchmarks, Takeover Panel inducement fee rules), confidentiality obligations (standalone vs. integrated, duration, residuals clauses), conditions precedent to closing (satisfactory due diligence risk, financing conditions, regulatory clearances), expense allocation (reliance damages exposure, culpa in contrahendo under civil law), and governing law provisions.

### [legalcode-ma-due-diligence-checklist](skills/legalcode-ma-due-diligence-checklist/SKILL.md)

Generate comprehensive M&A legal due diligence checklists tailored to transaction type (asset purchase, stock/share purchase, merger), target company characteristics, and applicable jurisdictions. Use when conducting legal due diligence for mergers, acquisitions, carve-outs, joint ventures, or corporate investments. Covers all 12 workstreams (corporate structure, contracts, IP, litigation, employment, regulatory, real estate, environmental, tax, data privacy, antitrust/FDI, insurance) with deal-type-specific considerations, red flag identification, and jurisdiction-variant requirements. Triggers on "M&A due diligence", "legal dd checklist", "acquisition due diligence", "asset purchase diligence", "stock purchase diligence", "merger legal review", "target company legal review", "data room checklist", or "deal due diligence". Jurisdiction-agnostic with markers for US, UK, EU, India, and Australia variants.

### [legalcode-merger-agreement-analysis](skills/legalcode-merger-agreement-analysis/SKILL.md)

Analyze merger agreements clause-by-clause against market standards or a transaction playbook. Covers deal structure (forward merger, reverse triangular merger, statutory merger), representations and warranties (bring-down conditions, materiality scrape, fundamental vs. general reps, survival periods), MAC/MAE clause drafting and judicial standards (Akorn, Snow Phipps), interim operating covenants (ordinary course, consent thresholds, efforts standards), conditions to closing (regulatory approvals, HSR, CMA, EU merger regulation, CFIUS), deal protection mechanisms (no-shop, fiduciary out, matching rights, go-shop), termination rights and fees (breakup fees, reverse termination fees), consideration structures (cash, stock-for-stock, mixed, earnouts), and dissenter/appraisal rights (DGCL Section 262, UK scheme squeeze-out).

### [legalcode-purchase-agreement-review](skills/legalcode-purchase-agreement-review/SKILL.md)

Review stock purchase agreements (SPAs) and asset purchase agreements (APAs) clause-by-clause against market standards or a transaction playbook. Analyzes representations and warranties (fundamental vs. general, materiality and knowledge qualifiers, materiality scrape), purchase price adjustment mechanisms (locked box vs. completion accounts, NWC targets, true-up), indemnification mechanics (tipping baskets, true deductibles, caps, survival periods, fraud carve-outs), MAC/MAE clauses and closing conditions, earnout provisions (metrics definition, anti-manipulation covenants, accounting standards, dispute resolution), escrow and holdback arrangements, representations and warranties insurance (RWI/W&I), non-compete and non-solicitation covenants, pre- and post-closing covenants, employee and benefits provisions, and specific indemnities (tax, environmental, pending litigation).

### [legalcode-shareholders-agreement-review](skills/legalcode-shareholders-agreement-review/SKILL.md)

Review shareholders agreements clause-by-clause — flag governance imbalances, generate confidence-scored redlines, and produce an auditable minority protection analysis. Use when reviewing shareholders agreements, voting agreements, investor rights agreements, subscription agreements, or any governance document covering drag-along and tag-along rights, anti-dilution protections (full ratchet vs. weighted average), ROFR/ROFO, pre-emptive rights, board composition and nomination rights, reserved matters, information and inspection rights, dividend policies, deadlock resolution mechanisms, and exit provisions (IPO, trade sale, buyback, redemption). Jurisdiction-aware with detailed US/UK/IN/AU coverage and [JURISDICTION-SPECIFIC] markers. GREEN/YELLOW/RED classification with redline suggestions. Evaluates minority protection adequacy and majority control balance across all 12 core SHA clause categories. Produces an auditable Glass Box analysis with Glass Box audit trail.

### [legalcode-venture-financing-suite](skills/legalcode-venture-financing-suite/SKILL.md)

Comprehensive venture financing suite covering instrument selection (SAFE vs. ASA vs. convertible note vs. priced equity round), cross-border structuring, securities exemption analysis, tax incentive routing (QSBS/Section 1202, SEIS/EIS/EMI, Singapore Sections 13H/13O/13U/13X), employee equity comparison (ISO/NSO, EMI, ESOP, 83(b)), and jurisdiction-specific frameworks for US, UK, EU, Singapore, and India. Use when a founder, investor, or counsel needs to: select the right early-stage financing instrument; understand tax relief eligibility; structure a cross-border investment or flip-up; review SAFE or convertible note terms; analyze QSBS or EIS/SEIS qualification; compare ISO vs. NSO vs. EMI equity for employees; or assess securities exemption availability under Reg D 506(b)/506(c), UK s.86, EU Prospectus Regulation, or MAS rules.

## General / Ip (6)

### [legalcode-ai-training-data-copyright](skills/legalcode-ai-training-data-copyright/SKILL.md)

Analyze copyright implications of AI training data. Use when evaluating whether scraped or licensed content can be used to train AI/ML models, assessing legal exposure from bulk data acquisition, reviewing TDM (text and data mining) rights under EU DSM Directive Articles 3 and 4, analyzing US fair use defenses for model training, checking compliance with EU AI Act Article 53 training data transparency obligations, assessing opt-out mechanisms (robots.txt, TDM reservations), reviewing Creative Commons and data license compatibility with AI training, evaluating right of publicity risks in training datasets, analyzing DMCA Section 1202 copyright management information claims, or preparing a litigation risk assessment for an AI training dataset. Covers the NYT v. OpenAI and Getty Images v.

### [legalcode-copyright-infringement-assessment](skills/legalcode-copyright-infringement-assessment/SKILL.md)

Assess copyright infringement risk across US, EU, and UK law. Use when determining whether a work infringes an existing copyright, evaluating defenses to an infringement claim, clearing a proposed use before publication or distribution, responding to a DMCA takedown or cease-and-desist letter, or advising on copyright risk in AI training datasets, sampling, digital media, software development, or creative works. Covers substantial similarity analysis, fair use four-factor evaluation (17 USC 107), EU InfoSoc Directive exceptions (2001/29/EC), UK fair dealing (CDPA 1988 ss.29–30A), de minimis use, independent creation defense, DMCA safe harbor (17 USC 512), statutory damages and willfulness (17 USC 504), and AI-generated content copyright. Also triggers when asked about parody, satire, remix, sampling, text and data mining, educational use, news reporting, or platform liability for user-generated content. Jurisdiction-agnostic workflow with deep US/EU/UK coverage.

### [legalcode-dmca-takedown-workflow](skills/legalcode-dmca-takedown-workflow/SKILL.md)

Manages DMCA takedown and counter-notification workflows under 17 USC 512, and EU Digital Services Act (DSA, Regulation 2022/2065) notice-and-action obligations. Use when drafting, sending, or evaluating DMCA takedown notices; handling counter-notifications and put-back timelines; assessing safe harbor eligibility for online service providers; building or auditing repeat infringer policies; registering or verifying a designated DMCA agent; responding to wrongful takedowns; assessing 512(f) misrepresentation liability; or mapping DSA Art. 16 notice obligations, DSA Art. 20 internal complaint procedures, and CDSM Directive Art. 17 upload-filter obligations for OCSSPs.

### [legalcode-licensing-agreement-review](skills/legalcode-licensing-agreement-review/SKILL.md)

Review IP licensing agreements of all categories — patents, trademarks, copyright, trade secrets, know-how, and mixed-IP bundles — against organizational positions or general market standards. Identifies deviations, generates confidence-scored redlines, and produces an auditable analysis. Use when reviewing any IP license for grant scope, field-of-use or territory restrictions, sublicensing chain provisions, royalty structures and audit rights, improvement and grant-back clauses, IP title warranties, infringement indemnification, licensor insolvency protections (including §365(n)), and termination effects on licensed rights. Covers pharmaceutical licenses, software licenses, trademark franchise-adjacent licenses, copyright and music licenses, trade secret licenses, know-how licenses, university technology transfer, and mixed-IP bundles.

### [legalcode-patent-landscape-analysis](skills/legalcode-patent-landscape-analysis/SKILL.md)

Conduct patent landscape analyses and freedom-to-operate (FTO) assessments covering patent family mapping, claim scope analysis, prior art assessment, white space identification, competitive intelligence, prosecution history review, and infringement risk scoring. Use when a company is entering a new technology area, evaluating M&A or licensing targets, planning R&D investment, clearing a product for commercialization, assessing competitor patent portfolios, or building IP filing strategy. Covers USPTO, EPO/UPC, WIPO/PCT, and JPO databases with IPC/CPC classification-based search methodology. Jurisdiction-agnostic framework with US, EU/UPC, UK, Japan, and WIPO-specific markers. Supports strategic landscape mode (broad competitive intelligence, white space identification, filing trend analysis) and FTO mode (product-specific element-by-element claim analysis and infringement risk scoring). Also supports validity / prior art searches and M&A patent due diligence.

### [legalcode-trade-secret-audit](skills/legalcode-trade-secret-audit/SKILL.md)

Audit an organization's trade secret protection program against US DTSA (18 U.S.C. §§ 1836–1839), state UTSA variations, and EU Trade Secrets Directive 2016/943. Conducts a comprehensive crown-jewels identification, reasonable-measures gap analysis, contractual portfolio review, employee-departure-protocol assessment, and litigation-readiness evaluation. Produces a severity-scored findings register, prioritized remediation roadmap, and Glass Box audit trail. Use when assessing trade secret program strength before litigation, M&A due diligence, regulatory review, or proactive compliance improvement. Also triggers for: "trade secret audit," "reasonable measures assessment," "crown jewels identification," "trade secret protection review," "inevitable disclosure analysis," "DTSA compliance check," "EU Trade Secrets Directive gap analysis," "employee departure trade secret risk," "misappropriation risk assessment," or "trade secret litigation readiness."

## General / Litigation (24)

### [legalcode-appellate-brief-drafter](skills/legalcode-appellate-brief-drafter/SKILL.md)

Draft appellate briefs for US federal circuit courts (FRAP), US state appellate courts, and UK Court of Appeal proceedings. Use when drafting an opening brief, appellant's brief, appellee's response brief, reply brief, or cross-appeal brief; when structuring grounds of appeal and standard-of-review arguments; when preparing a record appendix or joint appendix; when writing UK skeleton arguments and assembling appeal bundles; or when checking compliance with FRAP Rule 28/32, circuit-specific local rules, or CPR Part 52.

### [legalcode-arbitration-clause-review](skills/legalcode-arbitration-clause-review/SKILL.md)

Review and analyze arbitration clauses for enforceability, pathological defects, and commercial suitability — identify unclear scope, missing essential elements, inconsistent provisions, and jurisdiction-specific risks. Use when reviewing dispute resolution provisions in commercial contracts, evaluating arbitration clauses for New York Convention enforceability, assessing institutional arbitration clause compliance (ICC, LCIA, AAA/ICDR, SIAC, HKIAC, SCC), checking for multi-tiered escalation clause defects, or advising on seat selection and procedural adequacy. Covers ad hoc and institutional arbitration, emergency arbitrator provisions, consolidation rights, joinder clauses, confidentiality obligations, cost allocation mechanisms, and waiver provisions (class action, jury, punitive damages).

### [legalcode-arbitration-demand-drafter](skills/legalcode-arbitration-demand-drafter/SKILL.md)

Drafts and reviews arbitration demands (Requests for Arbitration, Notices of Arbitration), Statements of Claim, Answers/Responses, and Counterclaims for international and domestic commercial arbitration proceedings under ICC (2021 Rules), LCIA (2020 Rules), AAA Commercial Arbitration Rules, ICDR International Arbitration Rules, SIAC (2016/2025 Rules), and HKIAC (2018 Rules). Also supports UNCITRAL ad hoc arbitration and UNCITRAL Model Law jurisdictions.

### [legalcode-case-summarizer](skills/legalcode-case-summarizer/SKILL.md)

Summarize case law into structured, citation-quality briefs covering holding, key facts, reasoning, concurrence/dissent, procedural history, and precedential value. Use when building a case library, preparing for trial or arbitration, conducting legal research on a doctrinal issue, mapping the development of a legal doctrine, performing due diligence on the strength of legal authority, or analyzing opposing counsel's cited cases. Supports single-case deep summaries, batch processing of multiple cases, proper citation formatting (Bluebook, OSCOLA, AGLC, McGill Guide), and precedent chain mapping showing how a case fits into the broader development of a legal rule. Jurisdiction-agnostic at baseline with localization markers for US federal, England & Wales, and Australia. Also triggers on: "brief this case," "summarize this opinion," "what did the court hold in X," "map the precedent on Y," "is case X still good law," "digest these cases."

### [legalcode-citation-checker](skills/legalcode-citation-checker/SKILL.md)

Verify, correct, and audit legal citations across Bluebook (22nd ed.), California Style Manual (4th ed.), OSCOLA (5th ed.), and AGLC (4th ed.) — format compliance, current treatment checks, Shepardizing flags, pin cite accuracy, and local court rule compliance. Use when proofreading briefs, motions, memoranda, law review articles, or any legal document containing case citations, statute citations, regulatory citations, or secondary source citations. Covers US federal and state courts, English and Welsh courts, and Australian courts. Flags overruled, reversed, distinguished, and criticized cases with VERIFY markers, and checks pin cites against cited propositions. Supports both full-document audit mode and targeted single-citation lookup mode.

### [legalcode-complaint-drafter](skills/legalcode-complaint-drafter/SKILL.md)

Drafts civil complaints, petitions, and originating applications by mapping client facts to the legal elements of each cause of action. Validates plausibility under Twombly/Iqbal (US federal), applies heightened pleading for fraud (Rule 9(b)) and securities claims (PSLRA), and structures jurisdictional allegations, factual narratives, causes of action, and prayer for relief. Supports US federal, state, England & Wales (Particulars of Claim under CPR Part 16), and Australia (Statement of Claim under Federal Court Rules). Produces court-ready complaints with numbered paragraphs, element-mapped causes of action, exhibit references, and verification where required. Includes pre-suit requirement checks, Rule 11 compliance validation, and strategic claim selection guidance.

### [legalcode-complaint-drafter-ew](skills/legalcode-complaint-drafter-ew/SKILL.md)

Drafts Particulars of Claim, claim forms, and other statements of case for civil proceedings in England & Wales under the Civil Procedure Rules (CPR). Maps client facts to the legal elements of each cause of action under English law, validates compliance with CPR Part 16 and relevant Practice Directions, checks pre-action protocol compliance, and structures jurisdictional allegations, factual narratives, causes of action, and prayer for relief. Covers County Court and High Court proceedings across all tracks (small claims, fast track, intermediate track, multi-track). Produces court-ready Particulars of Claim with numbered paragraphs, statements of truth, schedules of loss, and document attachments as required. Includes pre-action protocol compliance checks, SRA professional conduct validation, and strategic claim selection guidance. Companion to legalcode-complaint-drafter (US federal/state).

### [legalcode-complaint-drafter-is](skills/legalcode-complaint-drafter-is/SKILL.md)

Drafts stefnur (writs of summons / statements of claim) for civil proceedings in Iceland under lög um meðferð einkamála nr. 91/1991 (Code of Civil Procedure). Maps client facts to the legal elements of each cause of action under Icelandic law, validates compliance with Article 80 requirements, and structures dómkröfur (claims), málavextir (factual narrative), lagarök (legal arguments), and sönnunargögn (evidence list). Covers héraðsdómur (district court), Landsréttur (Court of Appeal), and Hæstiréttur (Supreme Court) proceedings. Produces court-ready stefnur in the concise Icelandic format (5-6 pages typical), with proper kennitala identification, Icelandic-language drafting, and Art. 36 Codex Ethicus pre-litigation settlement verification. Companion to legalcode-complaint-drafter (US) and legalcode-complaint-drafter-ew (England & Wales). Based on Nordic civil law tradition with EEA/Lugano cross-border framework.

### [legalcode-damages-calculation](skills/legalcode-damages-calculation/SKILL.md)

Structure and calculate damages across economic, non-economic, punitive, and statutory categories for civil litigation, arbitration, and settlement negotiations. Use when quantifying harm, building damages models, preparing expert briefings, evaluating settlement ranges, or supporting early case assessment with defensible exposure analysis. Covers lost profits, consequential damages, diminution in value, pain and suffering, emotional distress, punitive/exemplary multipliers, statutory penalties, and fee-shifting. Jurisdiction-agnostic with [JURISDICTION-SPECIFIC] markers for US federal/state, England & Wales, and Australia. Integrates with legalcode-early-case-assessment for case-level exposure modeling and legalcode-brief-analyzer for damages-section persuasiveness review.

### [legalcode-deadline-calculator](skills/legalcode-deadline-calculator/SKILL.md)

Calculate litigation deadlines based on triggering events, applicable court rules, and jurisdictional requirements. Use when computing FRCP response deadlines (answer to complaint, discovery responses, MSJ oppositions, post-trial motions), appeals windows (FRAP Rule 4 notice of appeal), statute of limitations expiry dates with tolling analysis, EEOC charge filing deadlines (180/300 days), FTCA administrative claim windows (2 years + 6 months), government tort claims notice requirements, and regulatory filing deadlines. Applies FRCP Rule 6 day-count mechanics including weekend/holiday extensions, service-method additions under Rule 6(d) (2016 amendment), and calendar vs. business day distinctions. Handles multi-jurisdiction deadline tracking for matters pending in multiple courts.

### [legalcode-demand-letter-drafter](skills/legalcode-demand-letter-drafter/SKILL.md)

Drafts demand letters and cease and desist letters for common dispute types including breach of contract (UCC and common law), personal injury, employment disputes (wrongful termination, wage theft, FLSA violations, discrimination), consumer protection violations (CLRA, state UDAP, ACL), intellectual property infringement (trademark, copyright, patent cease and desist), debt collection (FDCPA and Regulation F compliant), property damage, and professional malpractice. Covers proper party identification, factual narrative development, legal basis articulation with specific statutory references, damages calculation and demand amount, response deadlines, consequences of non-compliance, and settlement offer frameworks.

### [legalcode-deposition-preparation](skills/legalcode-deposition-preparation/SKILL.md)

Prepare comprehensive deposition outlines with question sequences organized by topic and chronology, exhibit lists with foundation requirements, impeachment areas mapped to prior testimony and documents, objection anticipation guides, and witness demeanor assessment frameworks. Use when preparing Rule 30(b)(6) corporate designee depositions, expert witness depositions, adverse party depositions, or fact witness depositions in federal or state civil litigation. Covers deposition outline design, exhibit strategy, impeachment preparation, Daubert foundation mapping for experts, real-time note-taking templates, and post-deposition summary workflows. Calibrated to US federal practice (FRCP 30–32) with [JURISDICTION-SPECIFIC] markers for state variants and international deposition contexts.

### [legalcode-discovery-request-drafter](skills/legalcode-discovery-request-drafter/SKILL.md)

Draft interrogatories, requests for production (RFPs), and requests for admission (RFAs) tailored to specific case types. Generate objection responses with proper specific objection bases. Analyze proportionality under FRCP 26(b)(1), assert privilege, and advise on document preservation obligations. Use when drafting initial discovery packages, responding to discovery requests, building case-type templates for commercial, employment, IP, or personal injury litigation, or preparing for meet-and-confer on discovery disputes. Covers US federal practice (FRCP 26-37) and state-level variants with [JURISDICTION-SPECIFIC] markers. Supports both propounding side (drafting requests) and responding side (drafting objections and responses).

### [legalcode-discovery-response-drafter](skills/legalcode-discovery-response-drafter/SKILL.md)

Draft defensible responses to interrogatories, requests for production (RFPs), and requests for admission (RFAs) with specific objections, substantive answers, and privilege assertions. Covers FRCP 26(b)(1) proportionality defense, Rule 34(b)(2) objection-specificity requirements, FRCP 26(b)(5) privilege log drafting, FRE 502 clawback integration, and Rule 26(e) supplement obligations. Use when responding to received discovery requests in federal or state civil litigation, drafting specific objections with identifying particularity, asserting attorney-client privilege or work-product protection with compliant log entries, arguing proportionality as a limiting principle, or preparing meet-and-confer positions on discovery disputes.

### [legalcode-early-case-assessment](skills/legalcode-early-case-assessment/SKILL.md)

Run a litigation early case assessment (ECA) to evaluate merits, evidence strength, procedural leverage, expected spend, and settlement posture before major discovery spend. Use when legal teams need a defensible go/no-go recommendation, phase-based budget, risk-adjusted strategy branches, and executive-ready decision support for civil disputes across U.S., UK, AU, and other jurisdictions with localization markers.

### [legalcode-evidence-admissibility-analysis](skills/legalcode-evidence-admissibility-analysis/SKILL.md)

Analyze evidence admissibility under the Federal Rules of Evidence with rule-by-rule assessment for trial preparation, motions in limine, and evidentiary objection strategy. Use when evaluating whether specific evidence items can be admitted at trial, preparing motions in limine to exclude opposing evidence, anticipating evidentiary objections and building responses, assessing privilege claims before disclosure, analyzing hearsay and identifying applicable exceptions, evaluating expert witness qualification under Daubert or Frye, building foundation requirements checklists for any evidence type, or challenging expert methodology under the post-2023 FRE 702 preponderance standard.

### [legalcode-injunctive-relief-motion](skills/legalcode-injunctive-relief-motion/SKILL.md)

Drafts preliminary injunction and TRO (temporary restraining order) applications, analyzes prospects under the Winter v. NRDC four-factor test (US), and applies UK American Cyanamid principles (serious question to be tried / balance of convenience). Use when you need to obtain emergency or interim injunctive relief, stop ongoing harm, preserve the status quo, enforce covenants (non-compete, confidentiality, non-solicitation), protect IP rights, prevent asset dissipation, or seek a freezing order (Mareva), search order (Anton Piller), or anti-suit injunction. Covers FRCP Rule 65 TROs and preliminary injunctions, FRCP 65(c) bond requirements, ex parte / without-notice procedures (FRCP 65(b) / CPR Part 25), mandatory vs. prohibitory standards, circuit-by-circuit sliding-scale variations, and UK High Court interim injunction practice. Generates argument outlines, factor-by-factor prospect assessments, draft declaration and brief structures, and bond/undertaking analysis with Glass Box audit trail.

### [legalcode-litigation-hold-notice](skills/legalcode-litigation-hold-notice/SKILL.md)

Draft, review, and implement litigation hold notices and preservation workflows for anticipated or pending disputes. Use when users ask for legal hold implementation, document preservation memos, custodian scope planning, suspension of deletion policies, ESI retention instructions, or defensible hold release procedures. Supports cross- jurisdictional commercial matters with confidence-scored analysis and auditable output. Includes custodian tracking, reminder workflows, and defensible release procedures.

### [legalcode-litigation-risk-assessment](skills/legalcode-litigation-risk-assessment/SKILL.md)

Evaluate litigation risk across four dimensions — legal merit, factual strength, damages exposure, and reputational/strategic risk — to produce risk matrices with confidence-weighted probability assessments, cost-benefit analysis across three resolution branches (litigate, settle, mediate), and strategic recommendations. Use when deciding whether to file or defend a claim, re-evaluating litigation posture at a case milestone, advising a board or executive team on litigation exposure, preparing for settlement negotiations, or building a litigation budget with risk-adjusted spend scenarios. Supports pre-litigation (demand letter stage), early litigation (pre-discovery), mid-case (post-discovery), and late-case (trial approaching) assessment phases. Jurisdiction-agnostic with [JURISDICTION-SPECIFIC] markers for US federal/state, England & Wales, Australia, and EU commercial courts.

### [legalcode-mediation-preparation](skills/legalcode-mediation-preparation/SKILL.md)

Prepare comprehensive mediation materials including opening and confidential mediation statements, BATNA/WATNA/MLATNA analysis, settlement range development with probability-weighted outcomes, zone of possible agreement (ZOPA) identification, and strategic concession planning. Use when preparing for a commercial mediation session, selecting a mediator, organizing pre-mediation discovery and evidence, confirming settlement authority and decision-maker attendance, drafting opening statements, or developing phase-by-phase negotiation tactics. Evaluates cost-benefit of settlement vs. continued litigation with risk-adjusted present value analysis. Covers mediator selection criteria, multi-party coordination, joint session and caucus strategy, impasse diagnosis, and exit protocols. Supports evaluative and facilitative mediation approaches from claimant, defendant, or multi-party perspectives.

### [legalcode-privilege-review](skills/legalcode-privilege-review/SKILL.md)

Run defensible privilege review for litigation, investigations, and regulatory responses. Classify attorney-client / legal-advice privilege, litigation privilege, and work-product protection; detect waiver risk; produce privilege logs and challenge-ready rationale across U.S., UK, AU, and CA workflows with jurisdiction markers.

### [legalcode-settlement-agreement-drafter](skills/legalcode-settlement-agreement-drafter/SKILL.md)

Draft and review settlement agreements covering mutual releases, payment terms and schedules, confidentiality and non-disparagement, representations and warranties, tax indemnification, enforcement mechanisms, court approval requirements, and dismissal stipulations. Handles employment (ADEA/OWBPA over-40 waiver, FLSA court approval, NLRA-compliant non-disparagement), commercial, and class action settlements. Supports both US and UK frameworks. Use when settling employment discrimination claims, wage-and-hour disputes, commercial contract disputes, personal injury claims, class actions, or any civil matter requiring a written settlement agreement, release of claims, or dismissal stipulation. Jurisdiction-agnostic core with [JURISDICTION-SPECIFIC] markers for US federal, US state, and UK practice. Integrates with legalcode-settlement-negotiation for pre-drafting BATNA/ZOPA analysis and legalcode-early-case-assessment for merits input.

### [legalcode-settlement-negotiation](skills/legalcode-settlement-negotiation/SKILL.md)

Structure settlement negotiation frameworks with probability-weighted outcome modeling, risk-adjusted present values, and decision tree analysis. Use when preparing for settlement discussions, evaluating opponent's position, building a negotiation playbook, or advising clients on walk-away thresholds across civil disputes. Covers BATNA/WATNA/ZOPA analysis, opening position calculation, concession strategy, non-monetary terms, confidentiality provisions, release scope, and probability-weighted damages modeling. Supports both claimant and defendant perspectives. Jurisdiction-agnostic with [JURISDICTION-SPECIFIC] markers for US, UK, and AU practice. Integrates with legalcode-early-case-assessment for merits input and legalcode-damages-calculation for exposure quantification.

### [legalcode-witness-preparation](skills/legalcode-witness-preparation/SKILL.md)

Prepare lay witnesses and corporate designees for deposition and trial testimony in US civil litigation. Generates structured preparation packages covering anticipated direct and cross-examination questions, exhibit familiarity sessions, prior statement reconciliation, rules-of-the-road orientation, demeanor and conduct coaching, objection protocol instructions, deposition-vs-trial distinctions, and redirect rehabilitation planning. Covers all witness types: first-time lay witnesses, fact witnesses with prior testimony history, corporate Rule 30(b)(6) designees, former employees, and hostile/reluctant witnesses. Produces per-topic preparation cards, a witness readiness score, a mock examination plan, and a logistics checklist.

## General / Real Estate (4)

### [legalcode-real-estate-due-diligence](skills/legalcode-real-estate-due-diligence/SKILL.md)

Conducts comprehensive real estate due diligence for property acquisitions, financing, development, and disposal transactions. Covers eight workstreams: title examination, survey and boundary review, environmental assessments (Phase I/II ESA), zoning and planning compliance, permit and certificate verification, lease audit, property tax review, and encumbrance identification. Generates a PASS/FLAG/FAIL risk-scored report with priority tiers and actionable remediation recommendations. Use when acquiring commercial or residential property, securing real estate financing, conducting pre-development due diligence, or reviewing a vendor's due diligence pack.

### [legalcode-residential-lease-review](skills/legalcode-residential-lease-review/SKILL.md)

Review residential leases and tenancy agreements for tenants, landlords, and property managers — identify problematic clauses, flag illegal provisions, generate compliance checklists, and produce jurisdiction-specific remediation actions. Use when reviewing an Assured Shorthold Tenancy (AST) or periodic assured tenancy in England and Wales, a US state residential lease, an Australian residential tenancy agreement, or a German Mietvertrag (tenancy contract under BGB). Covers: rent and payment terms, security deposit / bond / Kaution, tenant and landlord rights, maintenance and repairs, habitability standards, termination and eviction grounds, rent control and increase limits, fair housing and anti-discrimination obligations, renewal provisions, and statutory compliance gaps.

### [legalcode-title-review](skills/legalcode-title-review/SKILL.md)

Reviews title commitments and title registers for real estate transactions — purchase, refinance, and development. Use when analyzing an ALTA 2021 title commitment (Schedule B-I requirements, Schedule B-II exceptions), a UK HM Land Registry official copy of register entries, a California Preliminary Report, or any title abstract or opinion letter. Analyzes easements, judgment and tax liens, mechanic's and materialmen's liens, restrictive covenants and CC&Rs, survey exceptions, mineral reservations, gap coverage risks, and endorsement requirements. Generates a closing checklist with prioritized curative action items, responsible parties, and deadlines. Supports the US ALTA/CLTA title insurance framework (owner's and lender's policies) and the UK Land Registration Act 2002 framework (absolute, good leasehold, possessory, and qualified title grades).

### [legalcode-zoning-land-use-analysis](skills/legalcode-zoning-land-use-analysis/SKILL.md)

Analyze zoning and land use compliance for any property or development project. Covers permitted use classification (by-right vs. discretionary), conditional/special use permits (CUPs/SUPs), area and use variances, nonconforming use rights (legal nonconforming status, abandonment, expansion), setback and bulk standards, subdivision regulation and platting, development agreements and vesting rights, environmental review (CEQA/NEPA), historic preservation (Section 106 NHPA, UK Planning (Listed Buildings and Conservation Areas) Act 1990), and exaction proportionality (Nollan/Dolan/Koontz/Sheetz). US and UK coverage: US Euclidean zoning, form-based codes, state enabling legislation, California Development Agreements (Gov.

## General / Risk Assessment (1)

### [legalcode-legal-risk-assessment](skills/legalcode-legal-risk-assessment/SKILL.md)

Assess legal risk across an organization, transaction, product, or initiative — identify risks by category (regulatory, contractual, litigation, IP, data privacy, employment, corporate governance), score probability and impact, classify severity as CRITICAL / HIGH / MEDIUM / LOW, and produce a confidence-scored, auditable risk register with prioritized mitigation strategies. Use when evaluating legal exposure for a new product launch, market entry, M&A transaction, regulatory change, contract portfolio, operational initiative, or enterprise-wide legal risk review. Jurisdiction-agnostic with localization markers for any governing law. Supports risk-appetite playbook or general-standard assessment. Produces a structured risk register with Glass Box audit trail.

## General / Workflows (20)

### [legalcode-client-intake-workflow](skills/legalcode-client-intake-workflow/SKILL.md)

Guide law firms through a structured client intake process from initial contact through engagement. Use when onboarding a new client, conducting conflict of interest checks, performing KYC/AML due diligence, preparing engagement letters, or setting up a new matter. Covers conflict screening, client qualification, risk assessment, fee structures, engagement letter drafting, and matter file setup. Jurisdiction-agnostic with localization markers for ABA Model Rules (US), SRA requirements (UK), and other bar regulations. Integrates with legalcode-conflict-check and legalcode-matter-triage-workflow for comprehensive intake workflows.

### [legalcode-conflict-check](skills/legalcode-conflict-check/SKILL.md)

Conduct comprehensive conflict of interest checks for law firms before accepting new client representations. Use when screening prospective clients, lateral hires, new matters for existing clients, related party transactions, or any engagement requiring professional responsibility clearance. Covers ABA Model Rules 1.7-1.10 (US), SRA Code of Conduct (UK), and common law/civil law jurisdiction frameworks. Identifies direct, imputed, positional, and corporate family conflicts. Produces auditable conflict clearance documentation with waiver recommendations and ethical wall protocols. Integrates with legalcode-client-intake-workflow for full intake process.

### [legalcode-cross-reference-analyzer](skills/legalcode-cross-reference-analyzer/SKILL.md)

Analyzes document sets for cross-reference integrity: builds a defined terms register, audits internal section references, maps inter-document reference chains, detects conflicting provisions, flags mismatched dates, and surfaces undefined or orphaned terms. Use when reviewing a contract suite, M&A document package, loan facility agreement with schedules, franchise disclosure document, or any multi-document transaction set where internal consistency is critical. Also use for single-document integrity checks before execution, during due diligence, or after substantial redlining. Jurisdiction-agnostic with [JURISDICTION-SPECIFIC] markers. Triggers on: cross-reference check, defined terms audit, internal consistency review, document suite integrity, conflicting provisions analysis, undefined terms check, orphaned references, mismatched definitions.

### [legalcode-defined-term-audit](skills/legalcode-defined-term-audit/SKILL.md)

Extracts and audits all defined terms in one or more legal documents — flags unused (orphaned) definitions, terms used but never defined, circular definitions, inconsistent usage, overly broad definitions, precision gaps, shadowed definitions, and conflicting definitions across related documents. Use when conducting pre-execution quality review of any contract, agreement, policy, regulation, or legislation; during due diligence on acquired contract portfolios; after substantial redlining or document merging; before filing regulatory submissions; or when preparing complex multi-document transaction sets (loan facilities with schedules, M&A agreements, franchise disclosure documents, software license suites). Jurisdiction-agnostic with [JURISDICTION-SPECIFIC] markers.

### [legalcode-document-classifier](skills/legalcode-document-classifier/SKILL.md)

Classify documents for e-discovery by relevance, privilege, and issue coding. Generates confidence-scored classification decisions, hot document flags, privilege log entries, and production-ready summaries for civil and commercial litigation. Use when conducting first-pass or second-pass document review, organizing a privilege log, identifying key custodian documents, applying issue codes to a review set, running quality control on a classified batch, or preparing a production transmittal. Supports Technology-Assisted Review (TAR) validation workflows, inadvertent-disclosure analysis, clawback procedures under FRE 502, and cross-border privilege assessment. Jurisdiction-agnostic with [JURISDICTION-SPECIFIC] markers; deepest coverage for US federal (FRCP), US state, UK, EU, and cross-border matters.

### [legalcode-document-summarizer](skills/legalcode-document-summarizer/SKILL.md)

Produce structured legal document summaries tailored to audience and purpose. Use when summarizing any legal document including contracts and commercial agreements, court pleadings and motions, regulatory filings (SEC, administrative), corporate governance documents (board resolutions, bylaws, shareholder agreements), and legislation or regulations. Outputs include executive summaries, key terms matrices, party identification tables, obligation maps, risk registers, and plain-language briefs. Adapts depth and language to the target audience: C-suite executives, in-house counsel, business stakeholders, paralegals, junior associates, or clients. Flags non-standard provisions, risk items, and missing mandatory elements. Jurisdiction-agnostic with [JURISDICTION-SPECIFIC] markers; operates without legalcode-mcp but uses it when connected for verified legal authority.

### [legalcode-engagement-letter-drafter](skills/legalcode-engagement-letter-drafter/SKILL.md)

Generate attorney/solicitor engagement letters from intake data. Use when drafting, reviewing, or auditing an engagement letter for a new or existing client matter. Covers all required elements: scope of representation, fee structures (hourly, flat fee, contingency, retainer, hybrid), billing practices, expense reimbursement, client responsibilities, conflict of interest disclosures, advance conflict waivers, confidentiality and attorney-client privilege, termination rights, file retention, ethics disclosures, and no-guarantee-of-outcome language. Aligned with ABA Model Rules 1.5, 1.6, 1.8, and 1.16; SRA Code of Conduct and Transparency Rules; New York 22 NYCRR Part 1215; California Business and Professions Code § 6148; and general bar requirements across US and UK jurisdictions. Produces jurisdiction-adapted, practice-area-specific engagement letters ready for attorney review. Also use for: client care letters, retainer agreements, letters of engagement, representation agreements, engagement audits.

### [legalcode-entity-compliance-tracker](skills/legalcode-entity-compliance-tracker/SKILL.md)

Track corporate entity compliance obligations across jurisdictions and generate compliance calendars. Use when managing annual reports, franchise tax filings, registered agent maintenance, officer and director changes, good standing certificates, business license renewals, or beneficial ownership filings for one or more legal entities. Covers domestic and foreign-qualified entities across all US states, UK Companies House, Australian ASIC, Canadian federal and provincial, and other major jurisdictions. Flags overdue and upcoming filings, classifies compliance status (COMPLIANT / SCHEDULED / APPROACHING / URGENT / CRITICAL / UNKNOWN), and produces executive dashboards, operational calendars, entity-level reports, and prioritized action lists. Also use when onboarding acquired entities, building compliance programs from scratch, or auditing a multi-subsidiary corporate structure for compliance gaps. Jurisdiction-agnostic with [JURISDICTION-SPECIFIC] markers.

### [legalcode-jurisdiction-mapper](skills/legalcode-jurisdiction-mapper/SKILL.md)

Produces comparative legal matrices across multiple jurisdictions for privacy and data protection, employment law, data localization, consumer protection, contract enforcement, and corporate governance. Identifies where legal requirements harmonize, diverge, or directly conflict, and surfaces actionable compliance recommendations. Use when planning global operations, structuring cross-border contracts, conducting multi-jurisdiction due diligence, designing global compliance programs, preparing regulatory filings in multiple markets, or advising on international expansion. Triggers on requests for "compare laws across countries," "how does [legal topic] differ in [jurisdictions]," "global compliance matrix," "jurisdiction comparison," "cross-border legal analysis," "which countries require [X]," or "harmonization opportunities."

### [legalcode-legal-project-management](skills/legalcode-legal-project-management/SKILL.md)

Structure and execute legal project management (LPM) across the full matter lifecycle — from scope definition and task decomposition through resource allocation, budget tracking, milestone management, risk identification, stakeholder communication, and post-matter review. Applies IILPM Define → Plan → Deliver → Close methodology and CLOC Core 12 operational competency framework. Use when opening a new legal matter, managing an active litigation or transaction, building a matter plan for outside counsel, conducting a mid-matter health check, setting up a budget with LEDES/UTBMS tracking, establishing alternative fee arrangements (AFAs), creating a risk register for a complex matter, drafting a communication plan for a legal engagement, or running a post-matter retrospective. Jurisdiction-agnostic. Works for in-house legal departments, law firms, and legal operations professionals.

### [legalcode-legislation-verification](skills/legalcode-legislation-verification/SKILL.md)

Verify cited statutes, regulations, directives, rules, and public guidance for currency, accuracy, and proposition support. Use when a legal document, brief, opinion, contract, or AI-generated output contains citations to legislation and you need to confirm that each provision exists, is currently in force (or was in force at the relevant date), has been correctly cited, has not been repealed or materially amended since citation, applies to the claimed territory, and actually supports the legal proposition advanced. Covers primary legislation (Acts, codes, statutes), secondary and delegated legislation (Statutory Instruments, regulations, orders, decrees), EU legislation (regulations directly applicable, directives requiring transposition), court procedural rules, and regulatory guidance.

### [legalcode-matter-scoping](skills/legalcode-matter-scoping/SKILL.md)

Generate comprehensive legal matter scope statements, fee arrangement analyses, staffing plans, phased budgets, milestone frameworks, and competitive-bid RFP templates. Use when engaging outside counsel, responding to a legal services RFP, structuring a panel tender, building an alternative-fee-arrangement (AFA) proposal, budgeting a litigation or transaction, planning a regulatory matter, or reviewing an existing engagement for scope creep. Covers hourly, fixed/flat, capped, blended, and portfolio fee arrangements with pros/cons analysis. Supports in-house legal departments, law firm business development, legal operations teams, CLO offices, and external counsel preparing engagement letters. Jurisdiction-agnostic with [JURISDICTION-SPECIFIC] markers.

### [legalcode-matter-triage-workflow](skills/legalcode-matter-triage-workflow/SKILL.md)

Route incoming legal requests to the appropriate resource based on matter type, urgency, complexity, and organizational risk. Use when a new legal request arrives, when prioritizing a backlog of open matters, or when deciding whether to handle a matter in-house or refer to outside counsel. Covers intake classification across all practice areas (contracts, employment, litigation, regulatory, IP, corporate, real estate, finance, tax), urgency scoring with SLA targets (CRITICAL/HIGH/STANDARD/LOW), complexity assessment (ROUTINE/MODERATE/COMPLEX/BET-THE-COMPANY), resource matching (self-service, paralegal, junior counsel, senior counsel, GC, outside counsel, specialist, ALSP), budget routing with authority levels, and escalation protocols for matters crossing risk thresholds. Supports configurable routing rules by business unit, geography, and matter type.

### [legalcode-offer-letter-drafter](skills/legalcode-offer-letter-drafter/SKILL.md)

Drafts and reviews US employment offer letters that are state-compliant across all 50 states. Covers at-will language, base salary and variable compensation, equity grants (options/RSUs/restricted stock), benefits summary, contingency clauses (background check, drug testing, I-9), confidentiality and IP assignment references, non-compete disclosures, and mandatory pay-transparency language for California (SB 1162), New York City (Local Law 32), Colorado (EPEWA / COMPS Order 38), Washington State (SB 5761), New York State (§194-b), and Illinois (SB 2038). Use when onboarding a new hire, extending an offer, converting a contractor, or reviewing a draft offer letter for compliance issues. Also covers offer rescission risk, implied-contract traps, 83(b) election notices, and state-specific IP assignment restrictions (CA, DE, IL, MN, NC, WA). US employers only — for international employment offers use jurisdiction-specific skills.

### [legalcode-outside-counsel-guidelines](skills/legalcode-outside-counsel-guidelines/SKILL.md)

Draft, update, or audit outside counsel guidelines (OCGs) — the overarching billing and conduct policies governing law firm relationships for corporate legal departments. Covers billing rates, staffing requirements, block-billing prohibition, expense policies, budget management, LEDES/UTBMS e-billing compliance, alternative fee arrangements (AFAs), diversity and inclusion reporting, performance scorecards, AI and technology provisions, and enforcement mechanisms. Supports two modes: (1) Draft or update an OCG from scratch for a legal department or organization, and (2) Audit existing outside counsel invoices or billing practices against an established OCG. Jurisdiction-agnostic with [JURISDICTION-SPECIFIC] markers for local billing ethics rules.

### [legalcode-plain-language](skills/legalcode-plain-language/SKILL.md)

Rewrites legal text for specified audiences while maintaining legal accuracy and precision. Covers legalese simplification, active-voice conversion, jargon replacement, archaic-phrase elimination, readability scoring (Flesch-Kincaid Reading Ease, Flesch-Kincaid Grade Level, Gunning Fog Index, SMOG, Coleman-Liau), and plain language compliance assessment.

### [legalcode-precedent-analyzer](skills/legalcode-precedent-analyzer/SKILL.md)

Analyzes completed deal corpora — contract archives, CLM exports, closing binders, or raw document folders — to extract standard positions, negotiation outcomes, client preferences, clause evolution trends, and market deviations. Use when a legal team wants to mine institutional knowledge from historical deals, generate or refresh a negotiation playbook backed by real data, understand win/loss rates on specific clause positions, identify client preference profiles from recurring counterparties, benchmark the firm's standard positions against market norms, or track how clause language has shifted over time.

### [legalcode-precedent-search](skills/legalcode-precedent-search/SKILL.md)

Search firm knowledge bases, document repositories, and legal precedent libraries for relevant prior agreements, templates, clauses, memoranda, court filings, transaction documents, and legal positions. Use when drafting new contracts and need proven language, advising clients on recurring legal issues and need prior advice letters, evaluating counterparty positions against prior deals, building or refreshing a clause library, or identifying subject matter experts within the organization. Covers semantic search by legal concept (not just keyword), multi-dimensional filtering (jurisdiction, counterparty, matter type, practice area, date range, document type), precedent applicability assessment, currency and staleness evaluation, conflicting-positions detection, subject matter expert identification, and privilege and confidentiality handling.

### [legalcode-proofread](skills/legalcode-proofread/SKILL.md)

Proofreads legal documents for defined term consistency, cross-reference accuracy, party name consistency, date logic, pronoun and referent consistency, section numbering, signature block completeness, exhibit and schedule references, and legalese errors (shall/will misuse, and/or, archaic boilerplate). Generates a structured redlined correction report classifying every finding as ERROR, WARNING, or SUGGESTION with specific correction language. Use for contracts, NDAs, employment agreements, leases, corporate documents, court filings, policies, and any legal document requiring pre-execution quality review. Triggers on phrases like "proofread this contract", "check for consistency errors", "review for defined terms", "find errors in this agreement", "check my cross-references", "proofread before signing", "check the signature blocks", "review for shall vs will", or "check for and/or usage".

### [legalcode-strategic-equilibrium-analysis](skills/legalcode-strategic-equilibrium-analysis/SKILL.md)

Analyze multi-party legal and business strategy problems using a game-theory workflow: identify visible and hidden players, map incentives and constraints, enumerate strategy space, eliminate dominated moves, build a simplified payoff matrix, identify likely Nash equilibria, and recommend concrete move sequences with counter-strategy defenses. Use when assessing disputes, litigation posture, settlement leverage, regulatory standoffs, board conflicts, internal investigations, commercial negotiations, founder disputes, partnership breakdowns, enforcement risk, or any high-stakes legal matter where multiple actors are making interdependent decisions. Jurisdiction-agnostic with [JURISDICTION-SPECIFIC] markers for legal constraints, procedure, and regulatory power.

## Jurisdictions / Australia (5)

### [legalcode-au-asic-regulatory-compliance](skills/legalcode-au-asic-regulatory-compliance/SKILL.md)

Assess compliance with the Australian Securities and Investments Commission (ASIC) regulatory framework.

### [legalcode-au-consumer-law-compliance](skills/legalcode-au-consumer-law-compliance/SKILL.md)

Assess compliance with the Australian Consumer Law (ACL) — Schedule 2 of the Competition and Consumer Act 2010 (Cth). Covers misleading or deceptive conduct (s 18), false representations (s 29), unconscionable conduct (ss 20–22), consumer guarantees (ss 51–64A), unfair contract terms (ss 23–28) including the expanded civil penalty regime effective 9 November 2023 (up to $50 million per contravention), product safety obligations (ss 104–140), and ACCC enforcement risk profiling. Generates COMPLIANT / PARTIAL / NON-COMPLIANT findings with CRITICAL / HIGH / MEDIUM / LOW risk tiers, clause-level remediation language, and a compliance roadmap. Use when auditing terms and conditions, returns/refund policies, marketing and advertising materials, subscription contracts, warranty documentation, standard form agreements, or any consumer-facing practice for ACL compliance. Jurisdiction: Australia (national — all states and territories). Enforced by ACCC and state/territory consumer protection agencies.

### [legalcode-au-fair-work-compliance](skills/legalcode-au-fair-work-compliance/SKILL.md)

Assess compliance with the Fair Work Act 2009 (Cth) — including the 11 National Employment Standards (NES), modern award coverage and minimum entitlements, enterprise agreement obligations, general protections and adverse action exposure, sham contracting risk, termination and unfair dismissal procedural fairness, record-keeping obligations, and FWO enforcement risk profiling. Fully covers the Closing Loopholes Acts (2023–2024): right to disconnect, new casual definition, fixed-term contract limits, wage theft criminalisation (effective 1 January 2025), labour hire same-job-same-pay orders, employee-like platform worker standards, and flexible work request reforms. Generates COMPLIANT / PARTIAL / NON-COMPLIANT findings with CRITICAL / HIGH / MEDIUM / LOW risk tiers, clause-level remediation language with revised drafts, penalty exposure estimates, and a prioritised remediation roadmap.

### [legalcode-au-unfair-contract-terms](skills/legalcode-au-unfair-contract-terms/SKILL.md)

Review contracts for unfair terms under Australia's unfair contract terms (UCT) regime — Australian Consumer Law (ACL) ss 23–28 and ASIC Act ss 12BH–12BK.

### [legalcode-franchise-agreement-review-au](skills/legalcode-franchise-agreement-review-au/SKILL.md)

Review franchise agreements for Australian operations against the Franchising Code of Conduct 2025 (Competition and Consumer (Industry Codes—Franchising) Regulations 2024) and Australian Consumer Law (Competition and Consumer Act 2010, Schedule 2) — verify disclosure document compliance with Schedule 1, screen for unfair contract terms under the expanded UCT regime (penalties from 9 November 2023), evaluate good faith obligation compliance (s 6), analyse restraint of trade provisions including new s 42 prohibition on non-renewal restraints, review significant capital expenditure disclosure (Items 14(1A), 14(1B) from 1 November 2025), assess early termination compensation obligations (s 43), evaluate "reasonable opportunity for return on investment" requirement (s 44), review specific purpose fund obligations, verify 14-day consideration period and cooling-off compliance, and assess ACCC enforcement risk.

## Jurisdictions / Brazil (2)

### [legalcode-br-clt-employment-review](skills/legalcode-br-clt-employment-review/SKILL.md)

Reviews Brazilian employment contracts, HR policies, payroll calculations, and termination packages for CLT (Consolidação das Leis do Trabalho) compliance. Covers all contract types (prazo indeterminado, experiência, intermitente, teletrabalho), 13th salary (décimo terceiro salário), férias and dobra de férias, FGTS deposits and multa rescisória, overtime (horas extras) and banco de horas, termination types and calculations (rescisão, aviso prévio proporcional, TRCT), union obligations, and eSocial event deadlines. Applies 2017 Reforma Trabalhista (Lei 13.467/2017) and Lei 14.442/2022 (teletrabalho update). Use when auditing Brazilian employment agreements, reviewing severance packages, validating payroll calculations, assessing vínculo empregatício (misclassification) exposure, or conducting HR compliance reviews for Brazilian operations.

### [legalcode-venture-financing-br](skills/legalcode-venture-financing-br/SKILL.md)

Brazilian venture financing advisor covering the full lifecycle from pre-seed to exit. Analyze, draft, and review MISTO (Latitud open-source), CICC (Contrato de Investimento em Capital Conversível), and Mútuo Conversível instruments. Assess Ltda vs. S.A. corporate structure selection, Acordo de Quotistas and Acordo de Acionistas terms, FIP (Fundo de Investimento em Participações) fund vehicle structuring under CVM Resolution 175/22 and its Normative Annex IV, Marco Legal das Startups (Lei Complementar 182/2021), CICC legislative framework (PLP 252/2023), CVM sandbox exemptions, IOF tax analysis, LGPD compliance, FGTS equity-compensation interaction, anti-dilution mechanics (broad-based weighted average), liquidation preference (preferência de liquidação), tag-along, drag-along, offshore flip structures, CADE antitrust thresholds, and ABStartups/ABVCAP market standards.

## Jurisdictions / Canada (3)

### [legalcode-ca-competition-act-assessment](skills/legalcode-ca-competition-act-assessment/SKILL.md)

Assess Competition Act (R.S.C., 1985, c. C-34) compliance for Canadian businesses and counsel. Covers criminal cartel offences (price-fixing, market allocation, bid-rigging, wage-fixing, no-poach), civil reviewable matters (abuse of dominance, price maintenance, exclusive dealing, tied selling, refusal to deal), merger notification and substantive review (post-2024 amendments including repealed efficiency defence and rebuttable presumption), deceptive marketing practices (misleading advertising, drip pricing, greenwashing pre-substantiation obligations), Competition Bureau enforcement and investigation procedures, consent agreements, immunity and leniency programs, private rights of action expanded by Bills C-56 and C-59, and the section 90.1 non-competitor civil collaboration regime in force December 2024.

### [legalcode-ca-employment-standards-review](skills/legalcode-ca-employment-standards-review/SKILL.md)

Reviews employment standards compliance across all Canadian jurisdictions — federal Canada Labour Code (Part III) and all 13 provincial/territorial Employment Standards Acts. Covers minimum wage, hours of work, overtime, vacation entitlements, statutory holidays, termination notice, severance pay, leaves of absence (maternity, parental, sick, family violence, compassionate care, bereavement), and equal pay obligations. Produces a jurisdiction-mapped compliance gap report with COMPLIANT/PARTIAL/NON-COMPLIANT classifications, remediation actions, and prioritized risk register. Use when auditing employment practices for a Canadian workforce, onboarding a new employer entity in Canada, reviewing employment contracts or HR policies for Canadian legal minimums, or advising on multi-provincial employment operations. Covers federally regulated employers (banks, telecoms, rail, air, federal Crown) and all provincial/territorial workforces. Jurisdiction-specific with province-by-province mapping.

### [legalcode-ca-pipeda-compliance](skills/legalcode-ca-pipeda-compliance/SKILL.md)

Comprehensive PIPEDA compliance assessment for Canadian private-sector organizations. Evaluates organizational practices against all 10 Fair Information Principles (PIPEDA Schedule 1 Clauses 4.1–4.10), the OPC 2019 Meaningful Consent Guidelines, cross-border transfer accountability obligations, individual access and correction rights, and the breach of security safeguards framework (ss.10.1–10.3, SOR/2018-64). Generates a structured compliance gap report with COMPLIANT/PARTIAL/NON-COMPLIANT findings, CRITICAL/ HIGH/MEDIUM/LOW risk prioritization, and actionable remediation steps. Covers provincial interaction with BC PIPA (SBC 2003, c.63), Alberta PIPA (SA 2003, c.P-6.5), and Quebec Law 25, and includes a CPPA readiness gap analysis against the proposed Consumer Privacy Protection Act (Bill C-27).

## Jurisdictions / China (1)

### [legalcode-non-compete-analysis-cn](skills/legalcode-non-compete-analysis-cn/SKILL.md)

Deep enforceability analysis of Chinese non-compete clauses (竞业限制) governed by Labor Contract Law of the PRC (劳动合同法) Articles 23-24 and the SPC Consolidated Judicial Interpretation on Labor Disputes (最高人民法院关于审理劳动争议案件适用法律问题的解释(一), effective 1 January 2021) and SPC Judicial Interpretation II (Fa Shi [2025] No. 12, effective 1 September 2025).

## Jurisdictions / European Union (7)

### [legalcode-eu-competition-law-assessment](skills/legalcode-eu-competition-law-assessment/SKILL.md)

Assess EU competition law compliance across all major enforcement pillars: Article 101 TFEU (anti-competitive agreements, cartels, block exemptions including VBER 2022/720 and horizontal BERs), Article 102 TFEU (abuse of dominant position, predatory pricing, exclusivity rebates, tying, margin squeeze, post-Intel AEC test), EU Merger Regulation 139/2004 (EU dimension thresholds, Phase I/II review, gun-jumping, SIEC test, Article 22 post-Illumina/GRAIL), State Aid (Articles 107-109 TFEU, GBER 651/2014, De Minimis 2023/2831), dawn raid preparedness (Regulation 1/2003 Article 20, legal privilege, digital evidence), and EU leniency programmes (cartel immunity, fine reductions, corporate statements, private damages interaction under Directive 2014/104/EU).

### [legalcode-eu-csrd-sustainability-reporting](skills/legalcode-eu-csrd-sustainability-reporting/SKILL.md)

EU CSRD (Directive 2022/2464/EU) sustainability reporting compliance assessment. Determine CSRD applicability and wave classification under Omnibus I thresholds (≥1,000 employees + €50M turnover or €25M balance sheet), assess double materiality assessment (DMA) completeness against ESRS 1 Chapter 3, evaluate ESRS disclosures across all cross-cutting (ESRS 1, ESRS 2) and topical standards (E1–E5, S1–S4, G1), review Scope 1/2/3 GHG methodology against ESRS E1, assess value chain data collection and CSDDD alignment, check XBRL/iXBRL digital tagging readiness, and evaluate limited assurance readiness under ISSA 5000. Classifies findings as COMPLIANT / PARTIAL / NON-COMPLIANT / CRITICAL. Outputs executive summary, ESRS gap matrix, DMA assessment, assurance readiness report, and remediation roadmap with phased timelines.

### [legalcode-eu-dma-compliance](skills/legalcode-eu-dma-compliance/SKILL.md)

Assess compliance with the EU Digital Markets Act (Regulation (EU) 2022/1925, "DMA") for any organisation that may be a gatekeeper or that provides products or services on a designated gatekeeper's core platform service.

### [legalcode-eu-dsa-compliance](skills/legalcode-eu-dsa-compliance/SKILL.md)

Assess compliance with the EU Digital Services Act (Regulation (EU) 2022/2065, "DSA") for any provider of intermediary services, online platforms, or online search engines serving EU users.

### [legalcode-eu-gdpr-breach-notification-operations](skills/legalcode-eu-gdpr-breach-notification-operations/SKILL.md)

Runs the complete EU GDPR personal data breach response workflow from initial incident triage through post-incident remediation. Use when: (1) a data breach or security incident involving personal data has occurred or is suspected, (2) an organisation needs to determine whether GDPR Articles 33 or 34 notification obligations are triggered, (3) a controller or processor needs to manage the 72-hour notification clock and lead supervisory authority determination, (4) a phased or supplementary notification must be prepared under Art. 33(4), (5) an operator needs to draft the Art. 33 SA notification, Art. 34 data subject communication, or processor-to-controller notification, (6) a forensic coordination plan or post-breach mitigation playbook is required, (7) Art. 33(5) internal documentation must be produced for regulatory audit. Covers controller-only, processor-only, and hybrid scenarios.

### [legalcode-eu-prospectus-regulation](skills/legalcode-eu-prospectus-regulation/SKILL.md)

Guides compliance with the EU Prospectus Regulation (Regulation (EU) 2017/1129, as amended by the EU Listing Act Regulation (EU) 2024/2809).

### [legalcode-eu-whistleblower-directive](skills/legalcode-eu-whistleblower-directive/SKILL.md)

Implement and audit compliance with EU Whistleblower Directive 2019/1937. Covers internal reporting channel design, protected persons scope, reportable breach categories, 7-day acknowledgment and 3-month feedback obligations, investigator independence, confidentiality requirements, anti-retaliation framework (Article 19 burden-of-proof reversal), external reporting authorities, public disclosure conditions (Article 15), GDPR interaction, and national transposition variations across all EU Member States.

## Jurisdictions / France (7)

### [legalcode-fr-bail-commercial](skills/legalcode-fr-bail-commercial/SKILL.md)

Draft or review a French commercial lease (bail commercial) governed by the statut des baux commerciaux — Code de commerce Art. L145-1 to L145-60, as reformed by Loi Pinel 2014 and Décret 2014-1317. Covers the mandatory 9-year term and triennial break rights (Art. L145-4), rent review using ILC (Indice des Loyers Commerciaux) or ILAT (Indice des Loyers des Activités Tertiaires) with plafonnement and déplafonnement rules, lissage (10% annual cap), clause tunnel (Art. L145-39 at 25% indexation variance), renewal rights (renouvellement), refusal without indemnity (motif sérieux et légitime), eviction indemnity (indemnité d'éviction — Art. L145-14) calculation and components, lease assignment (cession du bail / cession du fonds de commerce — Art. L145-16), subletting (sous-location — Art. L145-31), charges and property tax allocation (Art.

### [legalcode-fr-cnil-privacy-compliance](skills/legalcode-fr-cnil-privacy-compliance/SKILL.md)

Assess an organization's privacy compliance against French data protection law: the Loi Informatique et Libertés (LIL, Loi n°78-17 du 6 janvier 1978 modifiée), CNIL regulatory guidance, and GDPR as implemented in France. Covers CNIL cookie guidelines (2020/2022), France's 15-year digital age of consent, employee data and CSE consultation obligations, DPO designation and CNIL registration, mandatory DPIA (AIPD) list, data breach notification, processing register (Article 30), data subject rights, international transfers, and CNIL enforcement trends. Use when conducting a CNIL compliance assessment, preparing for a CNIL inspection (contrôle), auditing a privacy program in France, advising on French-specific GDPR derogations, reviewing cookie consent mechanisms for French audiences, assessing employee monitoring compliance under French labor law, or performing M&A privacy due diligence on a French entity. France-specific skill covering CNIL enforcement cases and administrative sanction procedure.

### [legalcode-fr-contrat-de-travail-cdi](skills/legalcode-fr-contrat-de-travail-cdi/SKILL.md)

Draft or review a French CDI (contrat de travail à durée indéterminée — permanent employment contract) for an employer or employee in France. Covers all mandatory clauses under the Code du travail, convention collective alignment (Syntec IDCC 1486, Métallurgie IDCC 3248, and major sector CCNs), non-compete clause (clause de non-concurrence) validity and mandatory financial compensation, mobility clauses (clause de mobilité), intellectual property assignment and employee inventions (Art. L113-9 / L611-7 Code de la propriété intellectuelle), forfait jours for autonomous executives, telework (télétravail) provisions, RGPD/CNIL employee data clause, probationary period (période d'essai) rules, termination (licenciement) procedure and Barème Macron, and rupture conventionnelle.

### [legalcode-fr-sapin-ii-compliance](skills/legalcode-fr-sapin-ii-compliance/SKILL.md)

Assess an organization's anti-corruption compliance program against France's Loi Sapin II (Loi n° 2016-1691 du 9 décembre 2016) and its Loi Waserman (2022) whistleblower amendments. Covers all eight Article 17 pillars: code of conduct, internal whistleblowing system, risk mapping, third-party due diligence, accounting controls, training, disciplinary sanctions, and monitoring. Also assesses AFA (Agence Française Anticorruption) control readiness, Commission des Sanctions exposure, CJIP risk, and interaction with the Loi de Vigilance and international anti-bribery regimes (FCPA, UK Bribery Act). Use when auditing a Sapin II compliance program, preparing for an AFA control, conducting M&A anti-corruption due diligence in France, or advising a multinational group on group-wide Sapin II rollout. France-specific skill with extraterritorial reach analysis for French parent company groups.

### [legalcode-franchise-agreement-review-eu-fr](skills/legalcode-franchise-agreement-review-eu-fr/SKILL.md)

Review franchise agreements for French operations against the Loi Doubin (Art. L330-3 Code de commerce) and Decree 91-337 (Art. R330-1) — verify Document d'Information Précontractuelle (DIP) compliance with mandatory 20-day pre-contractual disclosure period, screen for significant imbalance (déséquilibre significatif) under Art. L442-1 I(2) Code de commerce, evaluate post-term non-compete enforceability under Art. L341-2 (Macron Law 2015: maximum 1 year, limited to premises, indispensable for know-how protection), analyse abrupt termination (rupture brutale) exposure under Art.

### [legalcode-non-compete-analysis-fr](skills/legalcode-non-compete-analysis-fr/SKILL.md)

Deep enforceability analysis of a French non-compete clause (clause de non-concurrence) against the five cumulative Cour de cassation criteria established by the landmark decisions of 10 juillet 2002 (Cass. Soc. n° 00-45.135 and 00-45.387). Covers mandatory financial compensation (contrepartie financière) and its calculation basis, collective bargaining agreement (CCN/CBA) overlay including Syntec IDCC 1486, Métallurgie IDCC 3248, and other major sector agreements, geographic and activity scope proportionality, maximum duration, employer renunciation (waiver) mechanics and deadlines, consequences of non-payment and employee breach (Cass. Soc. 24 janvier 2024), and special situations (rupture conventionnelle, licenciement économique, période d'essai, Art. L1224-1 business transfers).

### [legalcode-venture-financing-fr](skills/legalcode-venture-financing-fr/SKILL.md)

French venture financing suite covering BSPCE (Art. 163 bis G CGI; 2025 Finance Law reform), BSA (Bons de Souscription d'Actions), SAS structural flexibility (actions de préférence L228-11 to L228-19; pacte d'associés), AMF private placement rules (Art. L411-2 CMF; less than 150 investors; qualified investor exemption), obligations convertibles (OC/OCABSA/BSAR; Arts. L228-91–L228-106 Code de Commerce), and French Tech ecosystem instruments (BPI France; Tibi initiative; French Tech Visa). Use when a founder, investor, or counsel needs to: select BSPCE vs. BSA vs.

## Jurisdictions / Germany (6)

### [legalcode-de-agb-review](skills/legalcode-de-agb-review/SKILL.md)

Reviews German General Terms and Conditions (AGB — Allgemeine Geschäftsbedingungen) under BGB §§ 305–310. Use when drafting, reviewing, or auditing standard terms for German-law contracts — whether B2C, B2B, online, or employment. Covers incorporation requirements (§ 305), surprising clause prohibition (§ 305c), transparency (§ 307 Transparenzgebot), conditional prohibitions (§ 308), absolute prohibition catalogue (§ 309), B2C vs. B2B distinctions (§ 310), consequences of invalidity and the prohibition of Geltungserhaltende Reduktion (§ 306). Also applies to e-commerce AGB, software licensing terms, IT procurement, and post-2022 subscription/auto-renewal changes. Triggers on "review our AGB", "check German T&Cs", "BGB 305", "AGB Inhaltskontrolle", "German general conditions", "standard terms Germany", "AGB enforceable", or any request to draft or validate general terms under German law.

### [legalcode-de-betriebsrat-consultation](skills/legalcode-de-betriebsrat-consultation/SKILL.md)

Guide employers through works council (Betriebsrat) consultation obligations under German Betriebsverfassungsgesetz (BetrVG). Use when planning hiring, reclassification, transfers, or dismissals in Germany (§§ 99–102), rolling out technical monitoring or AI systems, mobile work policies, or working-time changes that trigger § 87 mandatory codetermination, or when conducting operational changes (Betriebsänderung) requiring Interessenausgleich and Sozialplan under §§ 111–113. Also covers § 80 information rights, Einigungsstelle deadlock procedure, European Works Council (EBRG) requirements, and Betriebsvereinbarung drafting and validity. Triggers on: Betriebsrat consultation, BetrVG compliance, works council hearing, § 99 consent, § 102 Anhörung, § 87 Mitbestimmung, Interessenausgleich, Sozialplan, Nachteilsausgleich, Einigungsstelle, Betriebsvereinbarung, EWC, EBRG, SE-BetrVG, German labor law.

### [legalcode-de-gmbh-formation](skills/legalcode-de-gmbh-formation/SKILL.md)

Guide the formation of a German GmbH (Gesellschaft mit beschränkter Haftung) or UG (haftungsbeschränkt / Unternehmergesellschaft) from inception through operational status. Use when founding a German limited liability company, drafting or reviewing the Gesellschaftsvertrag (articles of association), deciding between Musterprotokoll and custom articles, structuring share capital (Stammkapital), appointing a Geschäftsführer (managing director), filing with the Handelsregister (commercial register), and registering with the Finanzamt (tax office). Also covers shareholder agreement (Gesellschaftervereinbarung) considerations, UG capital accumulation rules (§5a GmbHG), Vorgesellschaft liability during the pre-registration phase, and post-formation compliance obligations. Triggers on: GmbH gründen, GmbH formation, UG haftungsbeschränkt, Gesellschaftsvertrag, Musterprotokoll, Handelsregister, Stammkapital, Geschäftsführer appointment, German company formation, DiRUG online founding.

### [legalcode-de-kuendigungsschutz](skills/legalcode-de-kuendigungsschutz/SKILL.md)

Analyze German dismissal protection (Kündigungsschutz) for any employment termination scenario in Germany. Use when advising on KSchG social justification (betriebsbedingt, personenbedingt, verhaltensbedingt), Sozialauswahl criteria and scoring, BGB § 622 statutory notice periods, BGB § 626 extraordinary dismissal (außerordentliche Kündigung), special protection categories (pregnancy/MuSchG, parental leave/BEEG, severely disabled/ SGB IX, works council members/BetrVG § 103, DPOs/BDSG), Abfindung negotiation and § 1a KSchG statutory severance, works council consultation under BetrVG § 102, and the § 4 KSchG three-week claim period. Also use when drafting Aufhebungsverträge, assessing Massenentlassung (collective redundancy) obligations, or reviewing a proposed dismissal strategy for legal risk. Jurisdiction: Germany.

### [legalcode-non-compete-analysis-de](skills/legalcode-non-compete-analysis-de/SKILL.md)

Deep-analysis skill for German post-employment non-compete clauses (Nachvertragliches Wettbewerbsverbot) governed by HGB §§ 74-75a. Use when reviewing, drafting, or advising on a non-compete agreement in Germany for any commercial employee (Handlungsgehilfe), whether as employer or employee.

### [legalcode-venture-financing-de](skills/legalcode-venture-financing-de/SKILL.md)

German venture financing skill covering the full lifecycle from pre-seed instrument selection through Series A and beyond. Use when advising on Wandeldarlehen (convertible loans under BGB §488), GESSI standard bilingual documents, GmbH/UG startup structure, mandatory § 15 GmbHG notarization for share transfers, the INVEST federal angel grant (15% acquisition + 25% exit via BAFA), founder liability under § 43 GmbHG, VSOP/ESOP under German law including § 19a EStG deferral, the EuVECA passport (Regulation EU 345/2013), and German VC market term sheet standards (Gesellschaftervereinbarung, Liquidationspräferenz, Verwässerungsschutz, Mitverkaufspflicht).

## Jurisdictions / Iceland (4)

### [legalcode-anti-gold-plating-is](skills/legalcode-anti-gold-plating-is/SKILL.md)

Comprehensive section-by-section, word-by-word detection of gold-plating (gullhúðun) in Icelandic implementing legislation — identify where the local act imposes a more restrictive, more onerous, or more complicated regime than the original EU/EEA directive required, then trace each divergence back to its source in the legislative pre-law materials (frumvarp, greinargerð, athugasemdir við einstakar greinar, mat á áhrifum, samanburðartafla, samráðsgátt drög, umsagnir, nefndarálit, breytingartillögur, framsöguræða, 1./2./3. umræða, þingskjöl) via the current Legalcode MCP unified tool surface: legalcode_trace, legalcode_search, legalcode_fetch, legalcode_discover, and legalcode_analyze.

### [legalcode-eea-conformity-assessment-is](skills/legalcode-eea-conformity-assessment-is/SKILL.md)

Run an ESA-style assessment of Icelandic implementation of an EU act incorporated into the EEA Agreement. Build or validate a provision-level samanburðartafla; retrieve the act, Joint Committee Decision, Icelandic measures, pre-law, guidance, and case law through Legalcode MCP; then separately test notification, transposition completeness, substantive conformity, State-attributable application, legal certainty, enforceability, institutions, sanctions, and remedies. Use for ministry self-review, Form 1 or correlation-table review, ESA correspondence or complaints, implementation bills, post-enactment audits, under-implementation, incorrect transposition, systemic bad application, and paired gold-plating review. Triggers on samraemisathugun, conformity check, samanburdartafla, EEA transposition, ESA implementation review, or whether Iceland correctly implemented or applies an EEA act.

### [legalcode-iceland-real-estate-contracts](skills/legalcode-iceland-real-estate-contracts/SKILL.md)

Generate and review Icelandic real estate contract documents including kauptilbod (bid agreements), kaupsamningur (purchase agreements), and kostnadaruppgjor (expense settlements). Use when drafting or reviewing real estate transaction documents for residential or commercial property purchases in Iceland. Covers all required elements under log nr. 40/2002 um fasteignakaup (Real Estate Purchase Act), integrates with HMS (Housing Financing Fund) loan requirements, and produces professionally formatted Word documents. Includes comprehensive terminology glossary and contract review checklist for identifying missing or unusual provisions. Jurisdiction-specific for Iceland with all Icelandic legal terminology preserved alongside English translations.

### [legalcode-is-contract-law-general](skills/legalcode-is-contract-law-general/SKILL.md)

Review, draft, and analyse contracts governed by Icelandic law. Covers Act No. 7/1936 on Contracts, Agency and Void Legal Acts (samningsgerð, umboð og ógilda löggerninga), freedom of contract (samningsfrelsi), Section 36 general fairness clause, standard terms (staðlaðir samningsskilmálar), consumer protection (neytendavernd), Sale of Goods Act No. 50/2000, limitation periods under Act No. 150/2007 (4-year general rule), price indexation (verðtrygging) under Act No. 38/2001, GDPR implementation (Act No. 90/2018 — Persónuvernd), and the EEA/EU-aligned consumer acquis including Directives 93/13, 2011/83, and 2019/771. Use for any commercial agreement, service contract, consumer purchase, software licence, employment contract, or other legal instrument governed by Icelandic law. Identifies deviations, generates confidence-scored redlines, flags mandatory consumer provisions, and produces an auditable Glass Box output.

## Jurisdictions / India (1)

### [legalcode-venture-financing-in](skills/legalcode-venture-financing-in/SKILL.md)

India venture financing skill covering the full lifecycle from pre-seed to IPO exit. Deep analysis of India-specific instruments and regulatory frameworks: iSAFE (structured as CCPS under Companies Act 2013), Compulsorily Convertible Preference Shares (CCPS), Compulsorily Convertible Debentures (CCD), and priced equity rounds. Covers FEMA/NDI Rules 2019 pricing and reporting (Form FC-GPR, Form FC-TRS), SEBI Alternative Investment Fund (AIF) Category I angel fund regulations (including September 2025 restructuring), angel tax abolition (Finance Act 2024, effective FY 2025-26), Section 80-IAC startup tax holiday (3-year profit exemption), DPIIT recognition requirements and benefits, RBI External Commercial Borrowing (ECB) automatic route for startups, and SEBI ICDR IPO eligibility.

## Jurisdictions / Ireland (1)

### [legalcode-ie-company-formation](skills/legalcode-ie-company-formation/SKILL.md)

Guides Irish company formation under the Companies Act 2014 — entity type selection (LTD, DAC, PLC, CLG, UC), CRO registration and Form A1 preparation, constitution drafting, director and company secretary requirements (including EEA residency and Section 137 bond), annual return obligations, audit exemption qualification, and Section 110 SPV structures under the Taxes Consolidation Act 1997. Use when forming a new Irish company, advising on entity type choice, setting up a Section 110 SPV, checking post-incorporation compliance obligations, reviewing CRO filing requirements, or auditing annual return status and audit exemption eligibility. Covers all Companies Registration Office procedures, Revenue tax registration, and ongoing statutory compliance for Irish companies.

## Jurisdictions / Japan (2)

### [legalcode-jp-labor-standards-compliance](skills/legalcode-jp-labor-standards-compliance/SKILL.md)

Assess compliance with Japanese labor law for employers operating in Japan. Covers the Labor Standards Act (労働基準法, LSA), work rules (就業規則 shugyo kisoku), Article 36 overtime agreements (三六協定), annual paid leave mandatory designation (年次有給休暇), dismissal restrictions and the abuse of right doctrine (解雇権濫用法理), fixed-term employment 5-year conversion rule (無期転換申込権, Labor Contract Act Article 18), Work Style Reform Act (2018) overtime caps and equal pay for equal work obligations, minimum wage compliance, childcare and family care leave (育児・介護休業法), workplace harassment prevention obligations, and social insurance enrollment. Use when conducting a Japan HR compliance audit, reviewing employment practices for a Japan market entry, assessing risk before dismissal actions, or advising on work rule drafts. Triggers on: Japan labor law, rodo kijun ho, 36 agreement, sangyo kyotei, shugyo kisoku, mukitenkan, karoshi compliance, Work Style Reform, Japan overtime caps, Japan employment compliance.

### [legalcode-venture-financing-jp](skills/legalcode-venture-financing-jp/SKILL.md)

Japanese venture financing adviser covering the full lifecycle of startup capital formation under Japanese law. Use when structuring or reviewing J-KISS (新株予約権 convertible warrant), KK preferred share rounds, shareholder agreement terms, FIEA Article 63 fund-formation exemption, METI/JVCA standard documentation, the Enterprise Value Charge (企業価値担保権, spring 2026 enforcement), shinkabu yoyakuken employee stock options, angel tax incentive qualification, and FEFTA foreign investment screening. Covers instrument selection (J-KISS vs. priced preferred round), KK corporate mechanics (Articles 108, 199, 236 of the Companies Act), fund structuring (ILP vs. TK/GK), securities exemption compliance, and cross-border considerations for foreign VC investing in Japanese startups. Japan-specific. Requires qualified Japanese legal counsel review.

## Jurisdictions / New Zealand (1)

### [legalcode-nz-employment-relations](skills/legalcode-nz-employment-relations/SKILL.md)

Assess New Zealand employment law compliance and disputes under the Employment Relations Act 2000 (ERA) — good faith obligations, personal grievances, unjustified dismissal, 90-day trial periods, breaks and minimum entitlements (Holidays Act 2003), restructuring and redundancy protections, triangular employment, restraints of trade, and ERA/Employment Court proceedings. Use when advising on NZ employment disputes, reviewing NZ employment agreements, assessing restructuring processes, conducting HR compliance audits, or preparing for mediation and ERA proceedings. Covers the Employment Relations Act 2000, Holidays Act 2003, Minimum Wage Act 1983, Parental Leave and Employment Protection Act 1987, Health and Safety at Work Act 2015 (HSWA) employment intersection, Human Rights Act 1993 discrimination grounds, Privacy Act 2020 employment obligations, and KiwiSaver Act 2006 employer duties.

## Jurisdictions / Nordic (1)

### [legalcode-franchise-agreement-review-nordic](skills/legalcode-franchise-agreement-review-nordic/SKILL.md)

Review franchise agreements for operations in Norway, Sweden, Denmark, Finland or Iceland. Assess disclosure, unfair terms, competition restrictions, non-competes, termination and dispute resolution under the applicable national and EU/EEA rules. Produce prioritized findings, confidence assessments and an auditable review.

## Jurisdictions / Poland (3)

### [legalcode-pl-contract-review](skills/legalcode-pl-contract-review/SKILL.md)

Review commercial contracts under Polish law (Kodeks cywilny / Civil Code) — flag deviations, generate confidence-scored redlines with Polish-law citations, and produce an auditable analysis with business impact assessment. Use when reviewing vendor contracts, customer agreements, SaaS agreements, professional services contracts, licences, partnership agreements, procurement contracts, or any commercial agreement governed by Polish law requiring clause-by-clause analysis against standard positions or market practice. Covers KC mandatory rules (Art. 353¹, 58, 473, 483-485), kara umowna analysis, abusive clause register (UOKiK), fields of exploitation (pola eksploatacji), RODO/GDPR data processing addendum requirements, UZNK trade-secret protection, limitation periods (przedawnienie), and dispute resolution in Polish courts and arbitration (SA KIG, Lewiatan). Consolidates IURA methodology with Legalcode gold-standard quality frameworks.

### [legalcode-pl-employment-agreement](skills/legalcode-pl-employment-agreement/SKILL.md)

Draft or review Polish employment agreements (umowa o pracę) under the Kodeks pracy (Labour Code). Covers all mandatory content requirements (Art. 29 KP), probation period rules (Art. 25 KP), fixed-term limits (33 months / 3 contracts under Art. 25¹ KP), notice and termination procedures (Art. 36, 52, 53 KP), severance pay, non-compete clauses (zakaz konkurencji — Art. 101¹–101² KP), remote work provisions (Art. 67¹⁹–67³⁶ KP, effective April 7 2023), IP ownership (UPAPP Art. 12, 74; PrWłPrzem Art. 11), personal data and monitoring rules (Art. 22¹–22² KP + GDPR), ZUS contribution structure, and whistleblower protection (Ustawa o ochronie sygnalistów 2024). Also assesses misclassification risk: whether a civil law contract (umowa zlecenia / umowa o dzieło) or B2B arrangement would be reclassified as employment under Art. 22 KP and the 2026 PIP reclassification powers.

### [legalcode-pl-legal-memorandum](skills/legalcode-pl-legal-memorandum/SKILL.md)

Draft and review Polish law legal memoranda (opinia prawna) covering statutory interpretation (wykładnia prawa), Civil Code (Kodeks cywilny, KC) analysis, commercial company law (Kodeks spółek handlowych, KSH), administrative law (Kodeks postępowania administracyjnego, KPA), court structure, and precedent treatment. Applies the canonical Polish opinia prawna structure (Przedmiot / Podstawa prawna / Podstawa faktyczna / Analiza prawna / Wnioski / Zastrzeżenia). Consolidates IURA-methodology subsumption analysis with Legalcode quality frameworks.

## Jurisdictions / Singapore (2)

### [legalcode-sg-employment-act-compliance](skills/legalcode-sg-employment-act-compliance/SKILL.md)

Assess Singapore Employment Act (Cap. 91) compliance for employers and employees. Covers scope and coverage thresholds, Part IV protections (hours, overtime, rest days), salary payment and itemised payslip obligations, leave entitlements (annual, sick, maternity, paternity, shared parental, childcare), notice periods, termination and wrongful dismissal, retrenchment notification, MOM enforcement, Employment Claims Tribunals (ECT), TADM mediation, National Wages Council guidelines, tripartite guidelines on flexible work arrangements, and Workplace Fairness Act 2025. Use when auditing employment practices in Singapore, reviewing employment contracts for EA compliance, advising on employee rights or employer obligations under Singapore law, or preparing for a Ministry of Manpower inspection. Covers the 2019 major amendments (PME coverage expansion), Platform Workers Act 2024, Workplace Fairness Act 2025, and the April 2025 paternity/shared parental leave increases.

### [legalcode-venture-financing-sg](skills/legalcode-venture-financing-sg/SKILL.md)

Singapore venture financing advisor covering the full early-stage investment lifecycle under Singapore law: CARE agreements and VIMA 2.0 (February 2025) document suite, Series A term sheet analysis against SVCA/SAL market standards, convertible note review, VCFM fund manager licensing (post-RFMC repeal August 2024), Section 13O/13OA/13U/13H fund tax incentive qualification (January 2025 revamp), Variable Capital Company (VCC) fund structuring, Singapore Pte Ltd formation for startups, and ASEAN cross-border DTA and regulatory considerations.

## Jurisdictions / Switzerland (3)

### [legalcode-ch-cantonal-law-navigator](skills/legalcode-ch-cantonal-law-navigator/SKILL.md)

Navigate Switzerland's 26-canton legal patchwork: map federal vs. cantonal authority, compare commercial register procedures and fees, model effective corporate and inheritance tax rates by canton, identify the correct labor court (Arbeitsgericht / Tribunal des prud'hommes) and civil court of first instance, understand real estate transfer taxes (Handänderungssteuer / droits de mutation) and land registry (Grundbuch / Registre foncier) requirements, clarify notarization obligations under the Staatliches vs. Freies Notariat distinction, and flag cantonal variations that affect entity formation, property transactions, succession planning, or litigation strategy. Use when a client's matter touches Switzerland and you need to know which canton's rules apply and how they differ from other cantons. Covers ZH Zurich, ZG Zug, GE Geneva, VD Vaud, BE Bern, BS Basel-Stadt, LU Lucerne, SG St.

### [legalcode-ch-ndsg-compliance](skills/legalcode-ch-ndsg-compliance/SKILL.md)

Switzerland revised Federal Act on Data Protection (nDSG / revDSG / FADP, SR 235.1, in force 1 September 2023) compliance assessment. Use when an organisation needs to determine nDSG applicability, assess compliance posture against processing principles, information obligations, DPIA requirements, breach notification to the FDPIC, cross-border transfer safeguards, data processing agreement requirements, and criminal sanction exposure.

### [legalcode-ch-or-contract-review](skills/legalcode-ch-or-contract-review/SKILL.md)

Review contracts governed by Swiss law under the Code of Obligations (Obligationenrecht/OR/CO, SR 220). Covers formation requirements (OR Art. 1-10), defects of consent — error (Art. 23-24), fraud (Art. 28), duress (Art. 29-30) — penalty clauses and Konventionalstrafe (Art. 160-163), assignment of claims / Abtretung (Art. 164-174), prescription and limitation periods (Art. 127-142, including the 2020 reform), and all five major specific contract types: sales/Kaufvertrag (Art. 184-238, Rügepflicht Art. 201), lease/Mietvertrag (Art. 253-304), work contract/Werkvertrag (Art. 363-379, 2026 warranty reform), mandate/Auftrag (Art. 394-406), and employment/Arbeitsvertrag (Art. 319-362, non-compete OR 340-340c, mass layoffs). Includes international private law / IPRG choice-of-law analysis (Art. 116-121), general standard terms (AGB) control, and Swiss enforcement mechanisms (SchKG/LP).

## Jurisdictions / United Kingdom (10)

### [legalcode-non-compete-analysis-ew](skills/legalcode-non-compete-analysis-ew/SKILL.md)

Analyse English law restrictive covenant enforceability (England & Wales) covering the common law reasonableness test (legitimate proprietary interest + proportionality of duration, geography, and activity scope), Tillman v Egon Zehnder [2019] UKSC 32 blue-pencil severance, garden leave and PILON interaction (Credit Suisse v Armstrong credit principle; Tullett Prebon combined-period assessment), springboard injunctions (Roger Bullivant doctrine; QBE v Dymoke [2012] team-move analysis; Aquinas Education v Miller [2023] continuing-benefit requirement), employee versus shareholder/business-sale covenant distinction (Nordenfelt permissive standard; Law by Design v Ali [2022] equity- stake spectrum), tiered/cascading covenants, consideration and mid-employment amendment requirements, and pending UK Government reform (November 2025 Working Paper; consultation closed 18 February 2026; four reform options including 3-month cap).

### [legalcode-uk-advertising-compliance](skills/legalcode-uk-advertising-compliance/SKILL.md)

Review UK advertising and marketing communications for compliance with the CAP Code (non-broadcast), BCAP Code (broadcast), ASA enforcement practice, CMA consumer-protection expectations, pricing and discount claim rules, influencer and affiliate disclosure obligations, green and environmental claims, comparative advertising rules, distance selling disclosures, sector-specific restrictions (financial promotions, alcohol, gambling, food/nutrition/health, children's advertising, vaping/tobacco, crypto-assets), PECR and UK GDPR direct marketing obligations, and the Digital Markets, Competition and Consumers Act 2024 (DMCCA) consumer protection regime including fake reviews, drip pricing, and subscription contract obligations. Produces COMPLIANT / ADVISORY / NON-COMPLIANT / CRITICAL EXPOSURE findings with prioritised remediation and a Glass Box audit trail.

### [legalcode-uk-bribery-act-compliance](skills/legalcode-uk-bribery-act-compliance/SKILL.md)

UK Bribery Act 2010 compliance assessment for England and Wales covering all four criminal offences (s.1 active bribery, s.2 passive bribery, s.6 bribery of foreign public officials, s.7 corporate failure to prevent bribery), the adequate procedures defence and its six Ministry of Justice principles (proportionate procedures, top-level commitment, risk assessment, due diligence, communication, monitoring and review), associated person analysis under s.8 (employees, agents, subsidiaries, intermediaries, distributors, joint venture partners), facilitation payment prohibition, hospitality and gifts framework, and territorial scope for UK-incorporated and UK-nexus organisations.

### [legalcode-uk-corporate-governance-code](skills/legalcode-uk-corporate-governance-code/SKILL.md)

Reviews UK Corporate Governance Code 2024 (FRC) compliance for companies listed on the London Stock Exchange commercial companies and closed-ended investment funds categories. Covers all five Code sections: Board Leadership and Company Purpose (Principles A-E, Provisions 1-5), Division of Responsibilities (Principles F-H, Provisions 6-13), Composition, Succession and Evaluation (Principles I-L, Provisions 14-23), Audit, Risk and Internal Control (Principles M-O, Provisions 24-31), and Remuneration (Principles P-R, Provisions 32-41). Assesses compliance against all 18 Principles and 41 Provisions, generates comply-or-explain analysis, identifies material control gaps, evaluates malus and clawback provisions, assesses board independence and diversity disclosures, and produces a governance compliance roadmap.

### [legalcode-uk-employment-tribunal-claim](skills/legalcode-uk-employment-tribunal-claim/SKILL.md)

Guide UK Employment Tribunal proceedings in England and Wales from ACAS early conciliation through to final remedy calculation. Use for ET1 claim drafting, ET3 response review, time limit analysis, preliminary hearing preparation, disclosure strategy, witness statement advice, hearing tactics, costs risk assessment, and remedy quantification (unfair dismissal basic/compensatory awards, discrimination Vento bands, whistleblowing, equal pay, unlawful deductions). Covers the full tribunal lifecycle: ACAS early conciliation (12-week period from 1 December 2025), ET1/ET3 forms, case management orders, disclosure, Polkey reductions, ACAS uplift/reduction, and Employment Rights Bill 2024-25 reforms. Jurisdiction-specific to England and Wales under the Employment Tribunal (Constitution and Rules of Procedure) Regulations 2013 (SI 2013/1237) and Employment Rights Act 1996.

### [legalcode-uk-fca-regulatory-compliance](skills/legalcode-uk-fca-regulatory-compliance/SKILL.md)

Assess, audit, and remediate Financial Conduct Authority (FCA) regulatory compliance for UK-regulated firms across the full FCA Handbook: authorization under FSMA 2000 s.19 and the Regulated Activities Order 2001 (RAO), Principles for Businesses (PRIN 1–12 including Consumer Duty Principle 12), Senior Managers and Certification Regime (SM&CR — SYSC 2–4, COCON), Consumer Duty (FCA PS22/9 — four outcomes, cross-cutting rules, annual board report), Conduct of Business Sourcebook (COBS — client categorisation, suitability, best execution, MiFID II/UK MiFIR transaction reporting), Client Assets Sourcebook (CASS 6 custody, CASS 7 client money), financial promotions (FSMA 2000 s.21, FP Gateway February 2024, COBS 4), prudential requirements (MiFIDPRU ICARA, IFPR, legacy BIPRU/GENPRU), regulatory reporting (RegData/Gabriel, CMAR), Systems and Controls (SYSC — governance, risk management, compliance function, operational resilience), and financial crime controls (SYSC 6 AML/KYC, sanctions screening).

### [legalcode-uk-jct-nec-contract-review](skills/legalcode-uk-jct-nec-contract-review/SKILL.md)

Reviews UK construction contracts under JCT and NEC4 for England and Wales projects. Use when reviewing, negotiating, or advising on JCT Standard Building Contract (SBC/Q 2016 or 2024), JCT Design and Build Contract (DB 2016/2024), NEC4 Engineering and Construction Contract (ECC), or any contract governed by the Housing Grants, Construction and Regeneration Act 1996. Covers payment provisions, adjudication rights, extension of time, loss and expense, practical completion, defects liability, professional indemnity insurance, collateral warranties, and retention. Also use for Building Safety Act 2022 liability exposure, concurrent delay analysis, and smash-and-grab adjudication risk. Triggers on: JCT, NEC, NEC4, SBC, DB contract, construction contract review, HGCRA, Construction Act, adjudication, extension of time, practical completion, collateral warranty, retention, PI insurance construction, Building Safety Act construction.

### [legalcode-uk-prospectus-and-fca-offering-compliance](skills/legalcode-uk-prospectus-and-fca-offering-compliance/SKILL.md)

Reviews UK capital raising and securities offering compliance across the full regulatory stack: the Public Offers and Admissions to Trading Regulations 2024 (POATR 2024, in force 19 January 2026), FSMA 2000 s.21 financial promotion restriction, FCA Financial Promotion Gateway (from 7 February 2024), COBS 4 financial promotion rules, public-offer exemptions (£5 million de minimis, 150-person, qualified investor, Public Offer Platform), sophisticated-investor and high-net-worth pathways under the FPO 2005 (Articles 19, 48, 50, 50A), AIM/Main Market sensitivities under UKLR 2024 and AIM Rules, MTF admission prospectus obligations, offering document risk factor standards, Protected Forward-Looking Statements (PFLS), PISCES disclosure requirements, and cross-border UK/EU marketing boundaries including National Private Placement Regimes (NPPRs).

### [legalcode-uk-whistleblower-program-builder](skills/legalcode-uk-whistleblower-program-builder/SKILL.md)

Build, audit, and design UK whistleblowing frameworks under the Public Interest Disclosure Act 1998 (PIDA) and Employment Rights Act 1996 Part IVA (ss.43A-43L, s.47B, s.103A) for England and Wales.

### [legalcode-venture-financing-uk](skills/legalcode-venture-financing-uk/SKILL.md)

UK venture financing analysis and drafting skill covering the full stack of England & Wales early-stage and growth equity law: Advanced Subscription Agreements (ASAs/SeedFASTs), BVCA/UK Private Capital model documents (Feb 2025 suite), SEIS/EIS tax relief (expanded April 2026 — new limits), EMI options (individual limit doubled April 2026), Companies Act 2006 ss 549-561 pre-emption rights and Pre-emption Group Statement of Principles, new UK prospectus regime (FCA rules effective January 2026 under FSMA 2000 as amended by FSMA 2023), convertible loan notes, term sheets, shareholder agreements, cap table mechanics, anti-dilution, liquidation preferences, drag/tag-along, board governance, FSMA 2000 s.21 financial promotion restrictions, and ECCTA 2023 Companies House reforms.

## Jurisdictions / United States (11)

### [legalcode-franchise-agreement-review-us-ca](skills/legalcode-franchise-agreement-review-us-ca/SKILL.md)

Review franchise agreements for California operations against the California Franchise Investment Law (Corp. Code §31000-31516) and California Franchise Relations Act (Bus. & Prof. Code §20000-20043) — verify DFPI registration and FDD California addendum compliance, screen for non-waivable franchisee protections (good cause termination §20020, 60-day cure §20020, 180-day non-renewal notice §20025, transfer approval §20028, forum selection §20040.5), analyse post-termination non-compete enforceability under Bus. & Prof. Code §16600 (as broadened by AB 1076 and SB 699), review FDD 23-item compliance with California- specific addendum requirements (Cal. Code Regs. tit. 10, §310.114.1), evaluate escrow and financial assurance conditions, assess FAST Act (AB 1228) implications for fast food franchises, and flag anti-reliance disclaimer violations under AB 676.

### [legalcode-us-aia-construction-contract-review](skills/legalcode-us-aia-construction-contract-review/SKILL.md)

Review US construction contracts with emphasis on AIA standard forms (A101, A102, A133, A201 General Conditions, A401 Subcontract) and US owner-contractor risk allocation. Covers scope of work and contract sum mechanics, change orders and constructive changes, schedule and delay risk, retainage and payment applications, liquidated damages, insurance and performance/payment bonds, indemnification and anti-indemnity statutes, mechanic's lien exposure, substantial and final completion, and dispute forum strategy under AIA Article 15. Use when reviewing AIA prime contracts, subcontracts, ConsensusDocs, or owner-modified AIA forms on US commercial, institutional, healthcare, or public construction projects. Flags deviations from AIA standard, classifies risk (GREEN/YELLOW/RED), generates redlines with AIA fallback language, and produces a confidence-scored, auditable analysis. Also applies to CM-at-Risk (A133) and Design-Build delivery variants. Supports both owner-side and contractor-side review.

### [legalcode-us-delaware-entity-formation](skills/legalcode-us-delaware-entity-formation/SKILL.md)

Guide Delaware C-corporation formation end-to-end — Certificate of Incorporation drafting (8 Del. C. § 102), Section 102(b)(7) director and officer exculpation (including 2022 amendment), authorized shares structuring for franchise tax minimization (Authorized Shares vs. Assumed Par Value Capital Method under 8 Del. C. § 503), blank check preferred stock for VC readiness, bylaws adoption under DGCL § 109, initial organizational actions (board and stockholder written consents under §§ 141(f) and 228), registered agent requirements (§ 132), Section 83(b) election timing, 409A valuation sequencing, IP assignment at formation, and multi-state foreign qualification.

### [legalcode-us-fcpa-compliance](skills/legalcode-us-fcpa-compliance/SKILL.md)

Assesses Foreign Corrupt Practices Act (FCPA) compliance for US issuers, domestic concerns, and companies with US-nexus operations. Covers anti-bribery provisions (15 U.S.C. §§ 78dd-1 to 78dd-3), foreign official definition and instrumentality test (Esquenazi standard), books-and-records and internal controls (§ 78m(b)(2)), third-party due diligence (7-step lifecycle, 14-category red flag matrix), gifts/travel/ entertainment policy assessment, facilitation payment exposure, DOJ Corporate Enforcement Policy voluntary self-disclosure analysis (August 2024 120-day rule), DOJ Evaluation of Corporate Compliance Programs (ECCP September 2024) adequacy scoring, individual accountability framework, M&A successor liability analysis, and penalty structure (criminal/civil/disgorgement).

### [legalcode-us-federal-regulatory-comment](skills/legalcode-us-federal-regulatory-comment/SKILL.md)

Draft, structure, and sharpen federal regulatory comments for APA notice-and-comment rulemaking (5 U.S.C. § 553). Use when responding to a Notice of Proposed Rulemaking (NPRM), submitting comments to a federal agency docket on regulations.gov, challenging agency statutory authority, invoking the major questions doctrine (West Virginia v. EPA, 2022), analyzing the post-Chevron landscape after Loper Bright Enterprises v. Raimondo (2024), building an administrative record for judicial review, raising arbitrary and capricious arguments under APA § 706, analyzing Congressional Review Act implications, or preparing standing documentation. Covers comment structure, legal argument construction, policy argumentation, data and scientific evidence presentation, record preservation, and judicial review strategy. US federal jurisdiction only.

### [legalcode-us-ftc-advertising-compliance](skills/legalcode-us-ftc-advertising-compliance/SKILL.md)

Assess FTC advertising compliance for US advertisers — covering FTC Act Section 5 deceptive and unfair practices, advertising substantiation doctrine (prior substantiation, competent and reliable scientific evidence), FTC Endorsement and Testimonial Guides (16 CFR Part 255, 2023 amendments), material connection disclosures, influencer and social media requirements, clear and conspicuous disclosure standards, Made in USA claims (16 CFR Part 323, 2021 rule), FTC Green Guides environmental marketing (16 CFR Part 260), native advertising and deceptively formatted advertisements, negative option and subscription marketing (ROSCA, 2024 Negative Option Marketing Rule, click-to-cancel requirements), consumer reviews and testimonials (16 CFR Part 465, 2024 fake reviews rule), children's advertising (CARU, COPPA implications), and civil penalty exposure analysis.

### [legalcode-us-ofac-sanctions-screening](skills/legalcode-us-ofac-sanctions-screening/SKILL.md)

Conducts comprehensive US OFAC (Office of Foreign Assets Control) sanctions screening and compliance program analysis. Use when screening counterparties, customers, vendors, investors, or transactions against the SDN list, sectoral sanctions (SSI/CAPTA/NS-MBS), and country/territory programs. Applies the 50 Percent Rule across corporate ownership chains, assesses secondary sanctions exposure, evaluates correspondent and payable-through account risks, analyzes general and specific license availability, supports voluntary self-disclosure drafting, and designs or audits OFAC compliance programs against OFAC's 2019 Framework for Compliance Commitments. Triggers on OFAC screening, SDN check, sanctions due diligence, OFAC compliance program review, sanctions risk assessment, blocked person analysis, sectoral sanctions, secondary sanctions risk, 50 percent rule analysis, OFAC license application, voluntary self-disclosure, IEEPA sanctions, TWEA Cuba sanctions, Russia CAATSA, Iran sanctions, North Korea sanctions.

### [legalcode-us-private-offering-and-blue-sky-compliance](skills/legalcode-us-private-offering-and-blue-sky-compliance/SKILL.md)

Reviews US private securities offerings and resale transactions for Securities Act compliance — validates exemption selection (Reg D Rules 504/506(b)/506(c), Reg A/A+, Reg CF, Section 4(a)(2), Section 4(a)(7), Rule 144/144A), audits accredited investor verification procedures, performs bad actor disqualification checks under Rule 506(d), analyzes general solicitation controls, reviews offering materials and investor disclosures, maps Blue Sky notice filing obligations across all states, applies the integration doctrine, identifies broker-dealer and finder touchpoints, and builds a post-closing compliance calendar.

### [legalcode-us-section-409a-valuation-review](skills/legalcode-us-section-409a-valuation-review/SKILL.md)

Review nonqualified deferred compensation arrangements for IRC Section 409A compliance — assess valuation methodologies, verify safe harbor qualification (independent appraisal, illiquid startup presumption, formula method), analyze stock option pricing, audit permissible payment events, evaluate the short-term deferral exception, apply the six-month delay rule, identify operational and documentary failures, assess correction program eligibility, and model penalty exposure. Use when conducting 409A compliance audits, granting stock options or SARs, reviewing deferred compensation plan documents, preparing for M&A transactions involving executive compensation, advising on employment or separation agreements with deferred pay, or evaluating IRS correction program eligibility for prior violations. US federal law only (IRC § 409A and 26 CFR § 1.409A).

### [legalcode-us-state-non-compete-analysis](skills/legalcode-us-state-non-compete-analysis/SKILL.md)

Analyze non-compete agreement enforceability across all 50 US states. Use when reviewing a non-compete clause, covenant not to compete, restrictive covenant, post-employment restriction, or garden leave agreement — whether for an employer, employee, in-house counsel, or transactional attorney. Covers: 6-state total ban screening (California, Minnesota, North Dakota, Oklahoma, Montana, Wyoming), salary threshold screening for 12+ states, reasonableness factor analysis (geographic scope, duration, scope of activity, legitimate business interest), consideration requirements (at-hire vs. mid-employment), blue-pencil vs. red-pencil reformation doctrine, garden leave mechanics and salary requirements, choice-of-law enforceability (California SB 699 extraterritorial reach, DraftKings v. Hermalyn analysis), FTC rulemaking status post-Ryan LLC v.

### [legalcode-us-whistleblower-program-builder](skills/legalcode-us-whistleblower-program-builder/SKILL.md)

Builds US federal whistleblower reporting and investigation programs covering SOX Section 806 employee protections (18 U.S.C. § 1514A; 29 C.F.R. Part 1980), SOX Section 301 audit committee complaint procedures (15 U.S.C. § 78j-1(m)(4)), Dodd-Frank Section 922 SEC Whistleblower Program (15 U.S.C. § 78u-6; Rules 21F-1 through 21F-17), CFTC Whistleblower Program (7 U.S.C. § 26), OSHA's 25+ whistleblower protection statutes, False Claims Act qui tam (31 U.S.C. § 3730), Anti-Money Laundering Act of 2020 FinCEN whistleblower (31 U.S.C. § 5323), and IRS whistleblower awards (26 U.S.C. § 7623). Covers hotline and intake channel architecture, Rule 21F-17 anti-impediment employment agreement audit, anti-retaliation controls and burden-of-proof analysis (SOX contributing-factor standard; Dodd-Frank heightened standard; Digital Realty Trust v.
