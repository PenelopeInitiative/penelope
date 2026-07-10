# The Scam Tax Initiative
### A vendor-neutral consortium to make scamming unprofitable
*Working title — alternatives: TimeSink Alliance, Open Anti-Scam Engagement Project (OASEP)*

**Version 0.2 — FACT-CHECKED DRAFT FOR DISCUSSION — 8 July 2026**  
**Author: [+ founding contributors]**

---

## 0. One-paragraph summary

Scamming is an economic system with scarce inputs: human closer time, clean phone numbers, aged accounts, mule bandwidth, and the time window before detection. Conversational AI makes it possible to create bounded, monitored defensive engagement at a cost that can be far lower than human scambaiting. We propose an OWASP-style, vendor-neutral consortium in which AI providers, telcos, email providers, banks, anti-scam NGOs, and regulators define a common standard for routing verified scam traffic to governed AI personas. The objective is not vigilante entertainment and not autonomous retaliation; it is to impose measurable friction on scam operations, collect minimized intelligence, and make scam campaigns less profitable. Relevant components have been demonstrated in separate forms — Re:Scam for email, Apate.ai for redirected scam calls, O2’s Daisy as a public AI scambaiting proof-of-concept, and older phone-bot approaches such as Lenny and Jolly Roger. The missing piece appears to be a vendor-neutral standard, a governance model, and shared measurement.

---

## 1. Manifesto

- Scams are not only an awareness problem; they are an economics problem. Awareness matters, but recent public data still shows massive losses and continued exposure. GASA’s current public headline says **57%** of adults experienced a scam in 12 months and **US$442B** was lost worldwide to online scams; its prior 2024 report reported **US$1.03T** lost globally. These figures should not be mixed without explaining scope and methodology. [GASA-2025-HOME] [GASA-2024]
- The attacker’s advantage is asymmetric cost: high-volume outreach can be cheap, while each successful victim event can be catastrophic for the victim.
- AI can partially flip the labor asymmetry: defense can now engage patiently and consistently without requiring a human volunteer to spend hours on every call or email thread.
- We do not fight individuals; we tax operations. This distinction matters because many front-line operators in Southeast Asian scam centers are trafficking victims forced into criminality. [UNODC-FORCED]
- The initiative must be vendor-neutral, open-method where safe, legally governed, and metric-driven. Success should be measured in scammer-hours diverted, indicators shared, campaign intelligence generated, numbers/accounts forced into rotation, and — where partner telemetry permits — measurable funnel degradation.

## 2. The economics argument

### 2.1 The funnel is cheap to fill, expensive to close

- Kanich et al., *Spamalytics* (ACM CCS 2008), measured the Storm botnet’s pharma-spam campaign and found **28 conversions out of 350 million pharmacy campaign emails**, roughly 1 conversion per 12.5 million emails. This is the classic proof that very low conversion can still be economically viable at enormous scale. [SPAMALYTICS]
- Herley, *Why Do Nigerian Scammers Say They Are From Nigeria?* (Microsoft Research, 2012), argued that seemingly implausible scam claims can serve as a filter: when viable victims are rare, attackers need to reduce false positives and avoid wasting expensive human conversation on non-viable targets. That makes attacker conversation time an attack surface for defenders. [HERLEY]
- Phone, chat, investment, romance, remote-access, and pig-butchering scams are more labor-intensive than one-click spam. The latest public U.S. data shows reported fraud losses remain very large: FTC reported roughly **US$16B** in total reported fraud losses in 2025, up about 25% from 2024; the 2024 figure was **US$12.5B**. [FTC-2025-LOSSES] [FTC-2024-LOSSES]
- Contact-channel mix changes over time. In the U.S., the FTC says social media was the costliest reported fraud contact method in 2025, with **US$2.1B** in reported losses; for older adults in 2024, FTC still found median individual losses far higher for fraud that started by phone (**US$2,210**) than by social media (**US$650**). [FTC-SOCIAL-2025] [FTC-OLDER-2025]
- U.S. phone volume remains huge. YouMail reported **52.5B** U.S. robocalls in 2025, including **29.6B** unwanted telemarketing and scam calls; it also reported just over **4.1B** U.S. robocalls in May 2026. Truecaller’s U.S. stats page reports an average of **2.7B** spam/unwanted calls per month and an estimated **186M hours** wasted answering spam calls over Feb 2025–Jan 2026. [YOUMAIL-2025] [YOUMAIL-MAY2026] [TRUECALLER-US]

### 2.2 What is scarce on the attacker’s side

1. **Human closer hours** — the social-engineering labor needed to convert a target into payment.
2. **Clean phone numbers** — a burn-rate asset because flagged numbers lose usefulness.
3. **Aged email/social accounts** — higher-trust accounts that are costly to replace at scale.
4. **Unflagged payment rails, crypto wallets, and mule bandwidth** — necessary to monetize successful manipulation.
5. **Time-to-detection window** — the period before infrastructure, accounts, or scripts are discovered and blocked.

A controlled “time tax” can pressure all five. Every minute a verified scam operator spends with a persona is a minute not spent on a real victim, and every interaction can generate indicators, scripts, impersonated-brand data, mule-account hints, or campaign fingerprints — provided data collection is lawful, minimized, and audited.

### 2.3 The bot-vs-bot endgame

The common objection is: “Scammers will use AI too.” They will, and in some channels already do. The defensive thesis still holds, but should be stated carefully:

- If both sides automate the early funnel, scammer bot minutes spent on defensive bots still generate no revenue and may expose infrastructure.
- High-value scams still often require trust-building, payment coercion, and ad hoc recovery when the victim hesitates. Those stages are harder to automate fully and are where attacker time is most valuable.
- If attackers must filter for defensive bots, their own filter costs rise and their reachable-victim pool may shrink.
- **[VERIFY]** A formal model is still needed. Appendix C should include a funnel model with reply rate, false-positive cost, engagement-tax parameter, infrastructure burn, and operator-hour revenue.

## 3. Gap analysis: what exists, what does not

| Component | Evidence / examples | Corrected status |
|---|---|---|
| Email scam-engagement bots | Netsafe Re:Scam first appeared in 2017; Netsafe says the original 6-week prototype sent more than 1M emails and wasted more than 5 years of scammer time; Re:Scam 2.0 is described as back online. [RESCAM] | Demonstrated; operational status and scalability need current confirmation before outreach. |
| AI phone scambaiting proof-of-concept | O2 “Daisy” was unveiled in Nov 2024 as an AI “granny” answering scam calls and keeping scammers on calls up to 40 minutes. [O2-DAISY] | Demonstrated PR / awareness / technical proof; not evidence of an open standard. |
| Redirected scam-call engagement | Macquarie/APATE project describes multilingual conversational AI bots receiving redirected scam calls, in-cloud or on telco premises; Australian Government case study says Apate.ai was being used by one telco, blocking almost 10,000 scam calls/day and diverting about 600 scammer-hours/month. [APATE-MQ] [APATE-AEA] | Strongest direct precedent; independent audited efficacy and commercial details not public. |
| Legacy phone time-wasting bots | Lenny is an open-source / community phone bot based on pre-recorded responses. [LENNY] | Demonstrated concept; not modern AI and not a governed consortium. |
| Human scambaiting | Public creators and volunteer communities show that scammer engagement can consume attacker time. | Demonstrated, but artisanal and ethically variable; not a scalable governance model. |
| Anti-scam convening body | GASA is an established global anti-scam alliance with members across sectors and public research. [GASA-2025-HOME] | Exists. The proposed gap is narrower: a public defensive-engagement technical standard and donated-inference pool. |
| Vendor-neutral engagement standard + donated-inference pool + shared scammer-hour metrics | **[VERIFY]** I found no public equivalent combining these elements. | Proposed gap; needs validation through conversations with GASA, Apate.ai, telcos, AI providers, and regulators. |

## 4. Operating model

### 4.1 The three layers

1. **Routing layer — how scam traffic reaches the bots**
   - Consumer opt-in: forward suspected scam email; “send this suspected scam call to the Engagement Network.”
   - Honeypot pools: dedicated number ranges, seeded email identities, and social identities operated by authorized members.
   - Telco-level diversion under regulator-approved conditions, inspired by the Apate model.
   - **Hard rule:** bots do not initiate contact. They only engage inbound traffic to opted-in endpoints, verified honeypots, or regulator-approved diversion flows.

2. **Engagement layer — the AI personas**
   - Donated or sponsored bounded inference from AI-provider members.
   - Per-conversation caps, scoped system prompts, output filters, anomaly detection, red-team tests, and human review sampling.
   - Persona diversity to reduce fingerprinting.
   - Conversational-only v1: no link-following, credential entry, malware interaction, fake payments, account creation, or active infrastructure probing unless later approved by counsel and regulators.

3. **Intelligence layer — what the engagement produces**
   - Data-minimized collection of scripts, claimed brands, phone numbers, wallet identifiers, mule-account hints, URLs, account handles, and tactics, techniques, and procedures.
   - Audited pipeline to member telcos, banks, brand-protection teams, anti-fraud NGOs, and law enforcement.
   - Public metrics: scammer-hours diverted, verified conversations, indicators shared, campaigns detected, numbers/accounts reported, and measurement confidence.

### 4.2 OWASP-style consortium model

- Open individual membership plus corporate members that fund work and donate capacity but cannot dominate governance.
- Vendor-neutral bylaws: no single vendor controls routing, persona policy, intelligence access, or metrics publication.
- Flagship artifacts:
  - **The Defensive Engagement Standard** — routing protocols, persona rules, caps, logging, data handling, review, and escalation.
  - **The Scam Economics Index** — quarterly, methodologically transparent metrics.
  - **Reference implementations** — at minimum, an email leg and a call-diversion reference interface.
- AI providers receive an auditable public-good vehicle: “X verified scammer-hours diverted this quarter, powered by donated capacity from members,” subject to independent audit.

## 5. Legal framework and government partnership

This is a legal-design project before it is a technology project.

- The cleanest starting point is **recipient opt-in**: a user forwards a scam email they received or diverts a suspected scam call addressed to them.
- Network-level diversion requires regulatory cover, telco counsel, and clear safeguards against misrouting legitimate traffic.
- Per-jurisdiction legal issues include call recording, telecom secrecy, impersonation/deception by private actors, GDPR/UK GDPR lawful basis and transparency, retention limits, cross-border data transfers, defamation/misidentification risk, computer-misuse boundaries, and safe sharing with law enforcement.
- **Do not simplify call-recording rules.** California and Germany are high-risk examples; Italy and other EU jurisdictions require specific legal opinions rather than broad “two-party consent” labels. [CA-632] [DE-201] [GDPR-CALLS]
- The ask to governments is primarily **safe harbor / sandbox**, not money: a narrow framework for defensive engagement of unsolicited suspected fraudulent contact, plus an approved intelligence pipeline.

### 5.1 Likely first policy targets

- **Australia.** Strong fit: National Anti-Scam Centre, 2025 Scams Prevention Framework, mandatory sector codes, and existing Apate.ai/Macquarie precedent. [AUS-FRAMEWORK] [APATE-AEA]
- **Singapore.** Strong operational fit: ScamShield is a government-backed one-stop anti-scam portal with app, helpline, and reporting/checking flows. [SCAMSHIELD]
- **United Kingdom.** Strong policy fit: Online Fraud Charter, Fraud Strategy, Ofcom telecom-scam activity, and high political salience of fraud. The Online Fraud Charter says fraud accounts for around 40% of crime in England and Wales and that an estimated 80% is cyber-enabled. [UK-OFC]
- **European Union.** Potentially important but slower because of GDPR, ePrivacy, telecom secrecy, member-state recording laws, platform regulation, and cross-border governance.

## 6. Governance sketch

- Non-profit foundation.
- Independent board with individual-member voting base and corporate-member caps.
- Required working groups:
  1. Standard
  2. Personas and Safety
  3. Intel/Data
  4. Legal and Policy
  5. Metrics and Audit
  6. Abuse Response
- Annual independent audit of data handling, persona behavior, routing controls, and public metrics.
- Transparency report every quarter.
- Trademark the name at incorporation to prevent malicious forks or reputation laundering.
- Keep methods open except for persona playbooks and anti-fingerprinting details that would help attackers evade the system.

## 7. Ethics charter

1. **Target economics, not people.** No doxxing, humiliation, harassment, threats, or “torment” theater.
2. **Recognize forced criminality.** Many front-line scam-center workers may be trafficked, coerced, or under threat. Engagement personas must never abuse or endanger interlocutors. Intelligence sharing should prioritize dismantling operations and supporting victim identification. [UNODC-FORCED]
3. **Inbound only.** Bots do not initiate contact. Engagement is limited to opted-in endpoints, verified honeypots, or regulator-approved diversion.
4. **Data minimization by default.** Collect only what is necessary for scam disruption, evidence, safety, and measurement.
5. **No arbitrary targeting.** No “submit any number/email and sic bots on them” feature, ever.
6. **No active cyber operations in v1.** No malware interaction, link-following, fake payments, credential entry, system probing, or retaliation.
7. **Auditability.** Every metric and data pipeline must be independently reviewable.

## 8. Roadmap

- **Phase 0 — Draft and coalition test**
  - Publish v1 whitepaper, ethics charter, and FAQ.
  - Create GitHub org and static site.
  - Validate gap and appetite with GASA, Apate.ai/Macquarie, Netsafe/Re:Scam, one telco, one bank, one AI provider, and one law firm.

- **Phase 1 — Standard v0.1**
  - Define inbound-only routing, confidence thresholds, data minimization, persona boundaries, and metrics.
  - Publish reference threat model and abuse-prevention controls.

- **Phase 2 — Email-leg reference implementation**
  - Build or adapt a Re:Scam-style email flow under the standard.
  - Use opt-in forwarding only.
  - Publish initial scammer-hour methodology.

- **Phase 3 — Regulated phone pilot**
  - Target AU or SG first.
  - Work with a telco and regulator-approved sandbox.
  - Measure diverted scammer-hours, false-positive rate, indicators generated, and downstream blocking actions.

- **Phase 4 — Donated-inference pool and public index**
  - Add multi-provider inference with caps and auditing.
  - Publish the first quarterly Scam Economics Index.
  - Expand to additional telcos/email providers only after safety and legal review.

## 9. The ask by audience

- **AI providers:** donate capped inference and engineering liaison time; receive audited public-good attribution.
- **Telcos/email providers:** adopt the routing standard; receive reduced fraud exposure and actionable indicators.
- **Banks/payment providers:** contribute mule-account and payment-fraud feedback loops; receive earlier intelligence on impersonation and mule activity.
- **Governments/regulators:** create safe-harbor/sandbox conditions; receive measurable scam-disruption metrics and intelligence pipelines.
- **Security community:** review the standard, red-team the abuse model, and contribute reference implementations.
- **Anti-trafficking organizations:** advise on victim-centered engagement and escalation rules for forced-criminality indicators.

---

# Appendix A — Citable numbers and claims

| Claim | Current supported wording | Source |
|---|---|---|
| Global scam losses | “GASA’s 2024 report stated US$1.03T lost globally; GASA’s current 2025 public headline states US$442B lost worldwide to online scams. Treat the difference as a methodology/scope issue to explain before publication.” | [GASA-2024], [GASA-2025-HOME], [GASA-2025-REPORT] |
| Global scam exposure | “GASA/Feedzai 2025: survey of 46,000 adults across 42 markets; 57% experienced a scam and 23% lost money in the past 12 months.” | [GASA-2025-REPORT] |
| Spam conversion | “Storm pharma spam: 28 conversions from 350M emails.” | [SPAMALYTICS] |
| Scammer filtering economics | “Herley: far-fetched scam premises can reduce false positives by attracting only the most viable targets.” | [HERLEY] |
| U.S. fraud losses | “FTC: about US$16B reported fraud losses in 2025; US$12.5B reported in 2024.” | [FTC-2025-LOSSES], [FTC-2024-LOSSES] |
| U.S. social-media scam losses | “FTC: US$2.1B reported losses to scams that started on social media in 2025.” | [FTC-SOCIAL-2025] |
| Older-adult phone median loss | “FTC 2024 older-adult data: median individual loss was US$2,210 for fraud starting by phone vs US$650 for social media.” | [FTC-OLDER-2025] |
| U.S. robocall volume | “YouMail: 52.5B U.S. robocalls in 2025; 29.6B unwanted telemarketing/scam calls; just over 4.1B robocalls in May 2026.” | [YOUMAIL-2025], [YOUMAIL-MAY2026] |
| U.S. spam-call burden | “Truecaller: average 2.7B spam/unwanted calls/month and 186M hours wasted Feb 2025–Jan 2026.” | [TRUECALLER-US] |
| Re:Scam | “Netsafe: original 6-week Re:Scam prototype sent more than 1M emails and wasted more than 5 years of scammer time; Re:Scam 2.0 is described as back.” | [RESCAM] |
| Apate.ai | “Macquarie/APATE: redirected scam calls to conversational bots; Australian Government case study reports one telco deployment, nearly 10,000 scam calls/day and 600 scammer-hours/month diverted.” | [APATE-MQ], [APATE-AEA] |
| O2 Daisy | “O2: AI ‘granny’ answering scam calls in real time, keeping fraudsters on calls up to 40 minutes.” | [O2-DAISY] |
| Forced criminality | “UNODC: victims are trafficked into scam centers and compelled to commit online scams under threat of violence.” | [UNODC-FORCED] |
| Australia policy fit | “ACCC: Scams Prevention Framework; banks, digital platforms and telcos first sectors; mandatory codes and intelligence sharing.” | [AUS-FRAMEWORK] |
| Singapore policy fit | “ScamShield: government anti-scam portal, app and 1799 helpline.” | [SCAMSHIELD] |
| UK policy fit | “Online Fraud Charter: voluntary government/tech-sector charter; fraud around 40% of crime in England and Wales, estimated 80% cyber-enabled.” | [UK-OFC] |

# Appendix B — Red-team analysis

**B.1 Weaponized harassment / DDoS-by-AI on innocents.**  
Threat: arbitrary tagging of a person’s number/email could sic tireless bots on an innocent target.  
Controls: inbound-only; no “submit any number/email” feature; verified honeypots; multi-source corroboration; false-positive monitoring; rapid stop mechanism.

**B.2 Free-inference laundering.**  
Threat: attackers jailbreak bots into general-purpose LLM access or resell the interaction channel.  
Controls: scoped prompts, output filters, token caps, anomaly detection, rate limits, non-general persona policy, and post-incident prompt review.

**B.3 Scammer counter-fingerprinting.**  
Threat: attackers learn bot latency, refusal patterns, accents, scripts, or conversation structure and filter bots out.  
Controls: persona diversity, noisy behavioral signatures, rotating models, human-in-the-loop sampling, and non-public persona playbooks.

**B.4 Data-collection Trojan horse.**  
Threat: the routing layer becomes a de facto wiretap or data-harvesting system.  
Controls: no single-vendor routing control; privacy impact assessment; data minimization; retention limits; audit logs; independent annual audit; breach disclosure obligations.

**B.5 Reputational poisoning / rogue forks.**  
Threat: a malicious fork humiliates, abuses, or endangers coerced operators under a confusingly similar name.  
Controls: early trademark, published ethics charter, public conformance mark, active disavowal process.

**B.6 Vendor capture / astroturfing.**  
Threat: a large vendor or state actor packs working groups and steers the standard.  
Controls: individual voting base, funding transparency, board caps, conflict-of-interest register, public minutes where safe.

**B.7 Retaliation risk.**  
Threat: scam operations retaliate against identifiable contributors or opted-in users.  
Controls: operational anonymity for honeypot operators; no public attribution of individual engagements; strict separation between public contributors and operational infrastructure.

**B.8 Victim misclassification.**  
Threat: coerced front-line operators are treated as willing criminals, worsening harm.  
Controls: trafficking-risk training; escalation indicators; anti-trafficking partner review; no abusive persona behavior; no public release of raw calls.

# Appendix C — Funnel model [VERIFY / TODO]

Build a simple parametric model:

- send/call volume
- reply rate
- false-positive rate
- average human closer minutes per viable victim
- average bot-engagement minutes per non-viable target
- infrastructure burn rate per number/account/wallet
- detection/reporting delay
- conversion rate
- average revenue per conversion
- operator-hour cost
- AI-defense cost per minute

The key output should be the break-even engagement-tax level at which attacker revenue per operator-hour falls below the cost of running the campaign. This model must be explicitly labeled illustrative until calibrated with telco/bank/engagement telemetry.

# Appendix D — Open uncertainties not filled by guesswork

1. **GASA 2024 vs 2025 loss methodology.** The change from US$1.03T to US$442B must be explained before publication. It may reflect different scope, survey design, extrapolation, or definitions. Do not present either as a timeless universal number.
2. **Independent efficacy of Apate.ai deployments.** Public sources report strong operational metrics, but independent audit results were not found in public sources.
3. **Operational status of Re:Scam 2.0.** Netsafe says Re:Scam is back, but current throughput, availability, and governance details require confirmation.
4. **Legal feasibility by jurisdiction.** Requires formal legal opinions for call recording, deception/impersonation, telecom secrecy, GDPR/ePrivacy, safe harbor, and data-sharing.
5. **AI provider willingness to donate inference.** This is a proposal, not an established commitment.
6. **Conversion-rate degradation measurement.** Requires partner telemetry and careful experimental design; early phases should not overclaim.
7. **Name availability.** “Scam Tax Initiative,” “TimeSink Alliance,” and “OASEP” require trademark/domain checks.
8. **Whether a comparable standard already exists privately.** Public search did not find one, but GASA, telcos, banks, or vendors may have non-public frameworks.

# Sources

[GASA-2025-HOME]: https://gasa.org/  
[GASA-2025-REPORT]: https://gasa.org/knowledge-base/blog/global-scams-on-the-rise-over-half-of-adults-worldwide-report-scam-encounters  
[GASA-2024]: https://gasa.org/knowledge-base/blog/global-state-of-scams-report-2024-1-trillion-stolen-in-12-months-gasa-feedzai  
[SPAMALYTICS]: https://www.icir.org/christian/publications/2008-ccs-spamalytics.pdf  
[HERLEY]: https://www.microsoft.com/en-us/research/publication/why-do-nigerian-scammers-say-they-are-from-nigeria/  
[FTC-2025-LOSSES]: https://www.ftc.gov/news-events/news/press-releases/2026/06/ftc-data-show-people-reported-losing-3-point-5-billion-imposter-scams-2025  
[FTC-2024-LOSSES]: https://www.ftc.gov/news-events/news/press-releases/2025/03/new-ftc-data-show-big-jump-reported-losses-fraud-125-billion-2024  
[FTC-SOCIAL-2025]: https://www.ftc.gov/news-events/news/press-releases/2026/04/new-ftc-data-show-people-have-lost-billions-social-media-scams  
[FTC-OLDER-2025]: https://www.ftc.gov/system/files/ftc_gov/pdf/P144400-OlderAdultsReportDec2025.pdf  
[YOUMAIL-2025]: https://www.prnewswire.com/news-releases/us-consumers-received-52-5-billion-robocalls-in-2025--over-4-1-billion-in-december-according-to-youmail-robocall-index-302656174.html  
[YOUMAIL-MAY2026]: https://www.prnewswire.com/news-releases/us-consumers-received-just-over-4-1-billion-robocalls-in-may-according-to-youmail-robocall-index-302794864.html  
[TRUECALLER-US]: https://www.truecaller.com/us-spam-stats  
[RESCAM]: https://netsafe.org.nz/rescam  
[O2-DAISY]: https://news.virginmediao2.co.uk/o2-unveils-daisy-the-ai-granny-wasting-scammers-time/  
[LENNY]: https://www.lennytroll.com/  
[APATE-MQ]: https://researchers.mq.edu.au/en/projects/pitting-ai-against-phone-scams-a-proactive-defence/  
[APATE-AEA]: https://www.aea.gov.au/news/disrupting-scammers-army-ai-bots  
[UNODC-FORCED]: https://www.unodc.org/roseap/en/TrappedInScamCrime/article1.html  
[CA-632]: https://leginfo.legislature.ca.gov/faces/codes_displaySection.xhtml?lawCode=PEN&sectionNum=632  
[DE-201]: https://www.gesetze-im-internet.de/englisch_stgb/englisch_stgb.html  
[GDPR-CALLS]: https://gdprlocal.com/gdpr-recording-calls/  
[AUS-FRAMEWORK]: https://www.accc.gov.au/media-release/accc-welcomes-passage-of-world-first-scams-prevention-laws  
[SCAMSHIELD]: https://www.scamshield.gov.sg/  
[UK-OFC]: https://www.gov.uk/government/publications/online-fraud-charter-2023/online-fraud-charter-2023-accessible
