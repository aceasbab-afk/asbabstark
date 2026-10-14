# Apollo.io Lead-Gen Playbook: Independent Clinics → Medical Billing / Admin BPO

Owner: Sales & Ops · Seller: AmanaPS (https://amanaps.com/) · Status: ready to run once Apollo is connected

> Placeholders in `[brackets]` need real AmanaPS figures (results, pricing, case studies).
> Don't send outreach with invented numbers.

---

## 1. Connect Apollo first

| Step | Where | Why |
|---|---|---|
| 1. Connect the **Apollo.io** connector and sign in with the Apollo account that holds the credits | https://claude.ai/customize/connectors | Lets Claude search, enrich, and add contacts to sequences |
| 2. In the cloud environment settings, allow `mcp.apollo.io` and `api.apollo.io` (or choose a broader network level) | Session title bar → cloud environment → **Edit** → Network access (docs: https://code.claude.com/docs/en/cloud-environments#network-access) | The current network policy blocks Apollo (HTTP 403) |
| 3. Start a **new** session | — | Connectors and network settings are only read when a session starts |
| 4. Run the command in §4 | — | Builds the first lead list |

---

## 2. Ideal Customer Profile (ICP)

**Account (the clinic)**
- Independent, physician-owned practices in the **United States** (not part of a hospital, health system, or PE platform)
- **1–50 employees**; the sweet spot is 5–25, where billing is usually handled by one in-house person or the owner's spouse
- Specialties that outsource billing most often: family / internal medicine, pediatrics, behavioral & mental health, physical therapy, chiropractic, podiatry, pain management, cardiology, dermatology, OB/GYN, urgent care, orthopedics, gastroenterology
- First test markets: TX, FL, NY, NJ, CA, GA, IL, PA, OH, NC

**People (who to contact)**

| Priority | Titles | Role in the deal |
|---|---|---|
| 1 | Practice Manager, Office Manager, Practice Administrator, Clinic Manager | Feels the pain day to day; usually starts the evaluation |
| 2 | Owner, Physician Owner, Medical Director, President, Managing Partner | Signs the contract |
| 3 | Billing Manager, Billing Supervisor, RCM Manager, Revenue Cycle Manager | Influencer; can also resist outsourcing |
| 4 | Operations Manager, Director of Operations, Administrator, CFO / Controller (25+ employees) | Cares about ROI |

**Buying signals (in priority order)**
1. **Hiring** for a Medical Biller, Billing Specialist, Coder, Front Desk / Insurance Verification, or AR Specialist. This means turnover or a backlog.
2. **Apollo buying-intent topics:** Medical Billing, Revenue Cycle Management, Medical Coding, Healthcare Outsourcing, Denial Management, Credentialing
3. Recent growth: a new location, new providers, or rising headcount
4. Small-practice EHR / PM systems in their tech stack: Tebra (Kareo), AdvancedMD, athenahealth, eClinicalWorks, DrChrono, NextGen, Practice Fusion, CollaborateMD, Office Ally

**Exclude**
- Hospitals, health systems, and companies with more than 200 employees
- Other billing, RCM, or BPO companies (competitors). Exclude company keywords "medical billing company", "revenue cycle management", "RCM services", "BPO", "outsourcing".
- Staffing agencies and software vendors

---

## 3. Apollo filter setup (People search → save as a Saved Search)

| Filter | Value |
|---|---|
| Industry | Medical Practice; Hospital & Health Care; Mental Health Care; Health, Wellness & Fitness (for PT / chiro) |
| Company keywords (include) | clinic, medical practice, family medicine, pediatrics, behavioral health, physical therapy, chiropractic, podiatry, pain management, dermatology, cardiology, urgent care |
| Company keywords (exclude) | medical billing, revenue cycle, RCM, BPO, outsourcing, staffing, software |
| # Employees | 1–10, 11–20, 21–50 |
| Company HQ location | United States (start with 2–3 test states) |
| Job titles | the titles from the table in §2 |
| Seniority | Owner, Founder, C-Suite, Director, Manager |
| Email status | Verified only |
| Job postings (company filter) | "Medical Biller", "Billing Specialist", "Medical Coder", "Insurance Verification" (**best list**) |
| Buying intent | topics from §2, intent level High / Medium |

Build three saved lists:
- **List A, "Hiring billers" (hottest):** the filters above plus the job-postings filter
- **List B, "Intent":** the filters above plus the buying-intent filter
- **List C, "Core ICP":** the filters above only. Use it for volume.

---

## 4. Claude + Apollo commands (after connecting)

```
/apollo:prospect Practice Managers, Office Managers and Physician Owners at independent medical practices in Texas and Florida, 1-50 employees, specialties: family medicine, behavioral health, physical therapy, pain management; exclude billing/RCM companies
```

```
/apollo:enrich-lead <name + clinic, LinkedIn URL, or email>
```

```
/apollo:sequence-load <sequence name> — Practice Managers at independent clinics hiring medical billers, 1-50 employees, US
```

**Credit discipline:** searching costs nothing. Revealing emails and phone numbers spends credits.
- Claude states the credit cost before every enrichment.
- Enrich **List A in full**. Enrich **only Strong / Good ICP-fit leads** from Lists B and C.
- Reveal mobile numbers only for Priority 1–2 contacts at accounts with buying signals.

---

## 5. Outreach sequence (5 touches over 14 days)

| Day | Channel | Purpose |
|---|---|---|
| 1 | Email 1 | Name the pain and ask an easy question |
| 2 | LinkedIn | Connection request, no pitch |
| 4 | Phone + voicemail | Offer the free AR / denial review |
| 8 | Email 2 | Proof plus the offer |
| 14 | Email 3 | Break-up email |

**Email 1, subject: "billing at {{company}}"**
> Hi {{first_name}}, noticed {{company}} is hiring for a medical biller. Usually that means claims are piling up or AR is creeping past 45 days.
>
> AmanaPS handles billing, AR follow-up, eligibility checks, and credentialing for independent practices like yours, for less than the cost of one in-house hire.
>
> Worth a 15-minute look at where your claims are getting stuck?

**Email 2, subject: "free AR check for {{company}}"**
> {{first_name}}, a quick offer: we'll review your last 90 days of denials and aged AR (no cost, under a BAA) and show you what's recoverable.
>
> For a [specialty] practice similar to yours, we [result, e.g. cut AR days from X to Y]. Want me to send the 2-page checklist of what we'd need?

**Email 3, subject: "close the loop?"**
> {{first_name}}, I don't want to clutter your inbox. If billing is under control, I'll step back. If AR or denials are a headache, reply "later" and I'll check back next quarter.

**Call opener**
> "Hi {{first_name}}, it's [name] with AmanaPS. I'm calling because you're hiring a biller. Is the role open because of volume, or because someone left?"

Then use one of three discovery questions:
- What are your days in AR?
- What's your denial rate?
- Who works denials today?

---

## 6. Operating cadence and targets

| Metric | Weekly target per SDR |
|---|---|
| New contacts added to sequences | 150–250 |
| Calls | 150 (about 30 per day) |
| Reply rate | at least 5% (if below, rework the copy) |
| Meetings booked | 5–8 |
| Discovery → free AR audit | 50% |
| Audit → signed contract | 25–35% |

- **Daily:** work replies first, then calls to List A, then load new contacts.
- **Weekly:** pipeline review and an A/B test of subject lines. Pause any list with more than 3% bounces.
- **Monthly:** expand to new states and specialties that convert.

## 7. Compliance

- Cold email must follow CAN-SPAM: a real physical address and a working opt-out.
- Never include PHI in outreach. Sign a BAA before touching any claims data, including the free audit.
- Respect do-not-call lists and Apollo's opt-out flags.
