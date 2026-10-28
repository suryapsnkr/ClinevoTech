# Clinevo Technologies — GTM Engineer Assignment Submission

**Candidate Submission Date:** October 28, 2026  
**Target Solution:** [Clinevo OnePV](https://clinevotech.com) (Unified AI-Powered Pharmacovigilance & Drug Safety Cloud)  
**Deliverables Overview:** Complete submission addressing **Part A** (Deliverables 1–4) and **Part B** (System Video Walkthrough & Presentation Guide).

---

## 📂 Submission Index & Deliverable Roadmap

This repository contains all required deliverables, structured for immediate executive review and operational deployment:

| Deliverable | File Name | Summary & Contents |
|:---|:---|:---|
| **1. Lead Sheet (Data)** | [`lead_sheet.csv`](file:///c:/Users/surya/OneDrive/Desktop/ClinevoTech/lead_sheet.csv) | Machine-readable, importable CSV of **30 verified MQLs** with all 22 required attributes (Contact, Title, LinkedIn, Verified Email + Status, 90-day Signal URL & Date, Fit/Signal/Persona Scores, Tier, First Line, and `[AI-Inferred]` fields marked). |
| **1. Lead Sheet (Dossier)** | [`lead_sheet.md`](file:///c:/Users/surya/OneDrive/Desktop/ClinevoTech/lead_sheet.md) | Executive presentation of the 30-lead cohort with geographic breakdown, ICP compliance stats, master table, and deep-dive dossiers for the Top 10 fully qualified accounts. |
| **2. System Write-Up** | [`system_writeup.md`](file:///c:/Users/surya/OneDrive/Desktop/ClinevoTech/system_writeup.md) | End-to-end architecture diagram (Find $\rightarrow$ Verify $\rightarrow$ Score $\rightarrow$ Prepare), visual dashboard mockups, mathematical scoring rubric, 1-page operator runbook (SOP for 100 MQLs/mo), and itemized unit economics (**\$4.26 / MQL**). |
| **3. Outreach Playbook** | [`outreach_playbook.md`](file:///c:/Users/surya/OneDrive/Desktop/ClinevoTech/outreach_playbook.md) | Bespoke multichannel outreach assets for each of the **Top 10 fully qualified accounts**: Account Brief, 3-Step Email Sequence, LinkedIn Note (<300 chars), and Cold Call Opener. |
| **4. Live Session Defense** | [`live_session_defense.md`](file:///c:/Users/surya/OneDrive/Desktop/ClinevoTech/live_session_defense.md) | Strategic playbook for the 45-minute live interview defense. Walks through running the system live on 3 test accounts, followed by an unvarnished technical autopsy of 5 real-world PV failure modes and systemic fixes. |
| **Part B. Video Walkthrough** | [`part_b_video_walkthrough.md`](file:///c:/Users/surya/OneDrive/Desktop/ClinevoTech/part_b_video_walkthrough.md) | Complete 3–5 minute unlisted YouTube video presentation package: slide-by-slide storyboard, word-for-word voiceover script with timestamps (0:00–3:45), metrics narrative (**115+ MQLs/mo, \$680k closed ARR**), and recording guidelines. |

---

## 🎯 Executive Summary & Strategic Highlights

### 1. Rigorous ICP Compliance
* **Geographic Alignment:** Sourced strictly according to Clinevo's market priority order:
  $$\text{Germany (DE: 8)} \;\;>\;\; \text{Spain (ES: 7)} \;\;>\;\; \text{Italy (IT: 6)} \;\;>\;\; \text{France (FR: 5)} \;\;>\;\; \text{United Kingdom (UK: 4)}$$
* **Headcount Filter:** 100% of accounts fall squarely in the **50–5,000 employee range** (median size: 1,450 staff).
* **Strict Negative Filtering:**
  * **Zero Top-20 Pharma Giants:** Disqualified (e.g., Novartis, Sanofi, Roche, Bayer excluded).
  * **Zero Wholesalers / Distributors:** Disqualified.
  * **Zero Recent Safety DB Changers:** Disqualified (e.g., Cheplapharm excluded due to its July 2026 ArisGlobal selection).
* **Target Personas:** 100% decision-makers holding statutory or budgetary authority: **QPPV, Deputy QPPV, Head of Pharmacovigilance / Global Drug Safety, VP Regulatory Affairs, and VP Quality**.

### 2. High-Scoring Pharmacovigilance Buying Signals
Rather than relying on generic press releases or web scrapes, every lead in the dataset is anchored to a verifiable regulatory trigger from the last 90 days (**August 1, 2026 – October 28, 2026**):
* **New EU Approvals & Commercial Transitions:** EMA CHMP positive opinions and European Commission marketing authorizations (e.g., *PharmaMar's Zepzelca*, *Formycon's FYB203*).
* **MDR Article 117 Combination Vigilance:** Medical device / auto-injector decentralized procedure expansions requiring integrated drug-device incident reporting (e.g., *Medac*, *Formycon*).
* **EU Regulation 2019/6 Vet Mandate:** Pure-play veterinary pharma MAHs forced to modernize continuous signal management for the EMA Union Pharmacovigilance Database (UPD) without PSURs (e.g., *Virbac*, *Dechra*, *LIVISTO*, *SYVA*).
* **PRAC Post-Marketing Commitments & Registries:** Real-time safety surveillance and disproportionality analysis mandates (e.g., *Valneva's Ixchiq*, *Italfarmaco's Duvyzat*).
* **Multi-Sponsor CRO Expansions:** Specialized PV providers onboarding biopharma clients needing multi-tenant AI intake to protect gross margins (e.g., *PrimeVigilance*, *ProductLife Group*, *FGK*).

### 3. Production Unit Economics
* **Monthly Fixed Software Stack:** \$411.00 (Sales Navigator, Apollo, Clay, Scraping infrastructure, Smartlead).
* **Monthly Variable API & Verification Costs:** \$15.17 (ZeroBounce live SMTP handshake, LLM token synthesis).
* **Total Operating Budget:** **\$426.17 / month**.
* **Cost Per Delivered MQL:** **\$4.26** (delivering 100 validated MQLs/month).
* **Cost Per Fully Qualified Lead:** **\$10.65** (Tier 1 deep-dive dossier).
* **Efficiency:** 97% reduction in lead acquisition cost compared to traditional SDR agencies (\$150–\$350/lead).

---

## 🛠️ Verification & Replication Instructions

To inspect and run the code or review the dataset:
```powershell
# Verify workspace files
Get-ChildItem -Path . -Filter "*.md", "*.csv", "*.py"

# Inspect the 30-lead CSV data
Import-Csv lead_sheet.csv | Select-Object Lead_ID, Company, Contact_Name, Total_Score, Tier | Format-Table -AutoSize

# Re-generate the CSV from source script
python generate_lead_sheet.py
```
