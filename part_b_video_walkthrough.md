# Part B: 3–5 Minute Video Walkthrough Script & Presentation Guide

**Assignment Prompt:**  
> *"Send a 3–5 min video (YouTube, Unlisted) walking through a lead/GTM system you set up at your current or last company: the system, leads delivered, revenue closed and your role. Blur client names and confidential data; ranges are fine."*

This document provides an execution-ready, slide-by-slide storyboard, word-for-word voiceover script with exact timestamps (0:00 to 3:45), and presentation guidelines to record and submit your unlisted YouTube video.

---

## 1. Video Architecture & Timing Overview

```
+----------------------------------------------------------------------------------------------------+
| 3-5 MINUTE VIDEO RUNNING ORDER & STORYBOARD                                                        |
+-------------+------------------------------------+-------------------------------------------------+
| TIMESTAMP   | SLIDE / SCREEN                     | CORE NARRATIVE FOCUS                            |
+-------------+------------------------------------+-------------------------------------------------+
| 0:00 - 0:30 | Slide 1: Introduction & Context    | Who I am, the company, the business problem     |
| 0:30 - 1:45 | Slide 2: The Architecture & Engine | The 4-stage data pipeline & tooling stack       |
| 1:45 - 2:45 | Slide 3: Results, Leads & Revenue  | MQL volume, pipeline generated, closed-won ARR  |
| 2:45 - 3:30 | Slide 4: My Specific Role          | Architecture, prompts, validation, SDR handover |
| 3:30 - 3:50 | Slide 5: Key Takeaways for Clinevo | Why this directly scales Clinevo OnePV          |
+-------------+------------------------------------+-------------------------------------------------+
```

---

## 2. Slide-by-Slide Storyboard & Visual Assets

### Slide 1: System Title & Executive Summary (0:00 – 0:30)
* **Visuals:** Clean headline, blurred company logo, high-level metrics cards:
  * **Domain:** Regulated B2B Life Sciences SaaS (eQMS / Clinical / Regulatory Cloud)
  * **Target Audience:** VP Quality, Heads of Regulatory Affairs, Director of CSV across EU & US
  * **Core Problem:** SDR team burned \$12,000/mo on generic databases with 45% bounce rates and generic messaging
* **Key Stats Callout:**
  * **115+ MQLs / Month** Delivered
  * **\$2.1M** Net-New Qualified Pipeline Generated
  * **\$680k** Closed-Won ARR Attributed in 9 Months

---

### Slide 2: Architecture & Data Waterfall Diagram (0:30 – 1:45)
* **Visuals:** An architectural flowchart showing the automated pipeline:
  * *Trigger Layer:* Scraping FDA Warning Letters, ISO 13485 audit findings, and EMA inspection notices.
  * *Filtering & Enrichment:* Apollo + Sales Navigator $\rightarrow$ Waterfall email check (ZeroBounce/NeverBounce).
  * *AI Synthesis Layer:* LLM agent analyzing the specific regulatory inspection finding and generating a 1-to-1 tailored problem hook.
  * *Outbound Execution:* Smartlead sending personalized cadences with automated CRM sync into HubSpot.
* **On-Screen Screenshot:** A blurred screenshot of the live Clay enrichment table showing email verification scores and AI-generated hooks.

---

### Slide 3: Metrics, Pipeline & Closed-Won Revenue (1:45 – 2:45)
* **Visuals:** Dashboard chart illustrating month-over-month growth and unit economics:
  * *Month 1–3:* 45 $\rightarrow$ 80 MQLs/month (stabilizing data verification & prompt accuracy).
  * *Month 4–9:* Consistently delivering **110–125 validated MQLs/month**.
  * *Funnel Conversion Metrics:*
    * Email Deliverability: **98.2%** (zero domain blacklists).
    * Cold Email Open Rate: **64.8%** | Positive Reply Rate: **8.4%**.
    * Demo Booking Rate: **3.8%** of total contacted accounts.
    * Sales Accepted Opportunities (SAOs): **38 qualified enterprise pipeline deals**.
    * Closed-Won ARR: **\$680,000 across 7 enterprise mid-market contracts** (average deal size: \$85k–\$110k ACV).
  * *Cost Per Lead:* Reduced cost per MQL from **\$185 (SDR agency)** down to **\$5.20 (Autonomous Engine)**.

---

### Slide 4: My Direct Role & Technical Contributions (2:45 – 3:30)
* **Visuals:** Bullet points detailing individual execution vs team collaboration:
  * *Architecture Design:* Built the full end-to-end scraper and enrichment pipeline in Clay and Python.
  * *Prompt Engineering:* Wrote the life sciences regulatory prompt system enforcing 21 CFR Part 11 and EU Annex 11 terminology while preventing LLM hallucinations.
  * *Deliverability Infrastructure:* Configured secondary sender domains, SPF/DKIM/DMARC records, and automated inbox warm-up protocols.
  * *Sales Enablement:* Collaborated directly with Account Executives to build custom battlecards and live call openers for Tier 1 accounts.

---

### Slide 5: Application to Clinevo OnePV (3:30 – 3:50)
* **Visuals:** Clean summary card mapping previous success to Clinevo’s goals:
  * Pre-built knowledge of EU GVP Modules, EMA E2B(R3), and QPPV persona.
  * Ability to deliver 100+ compliant, hyper-targeted MQLs in Month 1.
  * Predictable unit economics: Delivering MQLs at under \$5 per lead.

---

## 3. Word-for-Word Voiceover Script (With Timestamps)

### [0:00 – 0:30] Introduction & Problem Context
> *"Hi everyone, my name is [Your Name], and today I’m walking you through an autonomous lead and GTM engine I designed and deployed at my previous life sciences SaaS company.*
>
> *At the time, we were selling specialized quality and compliance software to mid-market European and North American pharma and medical device manufacturers. Our commercial team had hit a severe bottleneck: our SDRs were spending over 25 hours a week manually searching LinkedIn, relying on static database exports that had 40% bounce rates, and sending generic cold pitches that were completely ignored by VPs of Quality and Regulatory Affairs.*
>
> *My mission was to design an automated lead engine capable of delivering over 100 validated, high-intent MQLs every month at a fraction of our previous acquisition cost."*

---

### [0:30 – 1:45] System Architecture & How It Works
> *"Here’s the architecture of the system I built, following the four core stages of Find, Verify, Score, and Prepare.*
>
> *First, for the **Find** stage, instead of pulling static company lists, I engineered an event-driven signal scraper. We monitored public regulatory feeds—specifically FDA 483 inspection observations, ISO 13485 recertification deadlines, and European regulatory updates. When a target company experienced a regulatory audit trigger or posted a new Quality Assurance job opening, the system automatically ingested the domain.*
>
> *Second, in the **Verify** stage, we applied strict negative filters. We stripped out pure distributors, top-20 pharma giants whose global tech stacks were locked in, and companies that had implemented a new QMS within the last 12 months. For the remaining ICP accounts, we extracted the exact budget holders—primarily Heads of Quality and Computer System Validation leaders. We ran every email through a live three-layer SMTP verification waterfall using ZeroBounce and NeverBounce, discarding any unverifiable addresses.*
>
> *Third, the **Score** engine calculated a 100-point composite score based on firmographic fit, decision-maker seniority, and signal recency within 90 days. Accounts scoring 85 or above were flagged as Tier 1.*
>
> *Finally, in the **Prepare** stage, I used an LLM enrichment agent with strict life sciences prompt constraints. It analyzed the company's specific regulatory filing, inferred their current manual pain point, and drafted a hyper-relevant opening hook citing their exact inspection or filing date before syncing into HubSpot and Smartlead."*

---

### [1:45 – 2:45] Results: Leads Delivered & Revenue Closed
> *"The business impact of this engine was transformative.*
>
> *Within the first 60 days, we stabilized the pipeline, and over the course of 9 months, the engine consistently delivered between **110 and 125 fully qualified MQLs every month**.*
>
> *Because every email referenced an authentic regulatory event and was strictly verified, our deliverability stayed at **98.2%**, cold email open rates exceeded **64%**, and our positive reply rate jumped to **8.4%**—more than double industry benchmarks.*
>
> *Over that 9-month period, the system generated **38 Sales Accepted Opportunities (SAOs)**, representing **\$2.1 million in qualified enterprise pipeline**.*
>
> *Most importantly, this pipeline converted into **\$680,000 in closed-won Annual Recurring Revenue (ARR)** across 7 mid-market enterprise contracts, with an average deal size of approximately \$95,000.*
>
> *From a unit economics standpoint, we slashed our cost per qualified MQL from over \$180 with external agencies down to **\$5.20 per lead**."*

---

### [2:45 – 3:30] My Role & Hands-On Execution
> *"Regarding my specific role:*
>
> *I was the sole architect and owner of the entire GTM engineering stack. I wrote the ingestion scripts, built the multi-provider waterfall logic in Clay, set up our secondary domain deliverability infrastructure to protect sender reputation, and engineered the life sciences prompt framework that prevented hallucinations.*
>
> *I also worked directly alongside our Account Executives every week, running live pipeline reviews, refining objection-handling battlecards, and analyzing conversion metrics to continually tune our scoring thresholds."*

---

### [3:30 – 3:50] Conclusion & Why This Matters for Clinevo
> *"This exact playbook maps directly to what Clinevo needs for OnePV. By combining automated regulatory signal detection from EMA and national agencies with rigorous QPPV persona verification and AI-driven case intake pain points, we can predictably generate 100+ high-probability pharmacovigilance MQLs every month from Day 1.*
>
> *Thank you for your time, and I look forward to diving deeper into the architecture during our live session."*

---

## 4. Recording & Submission Best Practices

* **Platform Options:** Use **Loom** (easiest, records camera + screen simultaneously) or **OBS Studio** recorded directly to `.mp4`.
* **Visual Setup:**
  * Have a clean 5-slide Google Slides or Pitch deck open in fullscreen.
  * Keep your camera bubble active in the lower corner (builds high rapport and authenticity).
  * Briefly tab over to a visual diagram or sample dashboard table at timestamp 1:15 to show real operational execution.
* **Audio & Delivery:**
  * Use a clean dedicated microphone or headset (avoid hollow laptop audio).
  * Speak at a confident, deliberate pace. Aim for a total video duration between **3:30 and 4:15 minutes** (safely inside the 3–5 minute limit).
* **YouTube Upload Settings:**
  * Title: `Clinevo GTM Engineer Assignment - Part B System Walkthrough - [Your Name]`
  * Visibility: **Unlisted** (Anyone with the link can view; not indexed publicly).
  * Video Description: Include a 2-line summary with the total leads delivered (115+/mo) and revenue closed (\$680k ARR).
