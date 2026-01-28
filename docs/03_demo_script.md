# MoPix — Executive Demo Script (3–5 Minutes)

**Purpose:** A live, hands-on demo that proves MoPix can deliver credible, fast, role-aware results for both crew and producers. 
**Rule:** No dead clicks. Every screen must respond.

---

## 0) Demo Setup (30 seconds)

**Device:** Laptop preferred (mobile optional if identical UX). 
**Environment:** Demo account and seeded dataset enabled.

Preconfigured demo profiles:
- **Crew Profile:** Production Sound Mixer | NYC | Union status optional
- **Producer Profile:** Line Producer | Savannah, GA

---

## 1) Scene One — Crew Agent: Find Work (90 seconds)

### Prompt 1
“I’m a production sound mixer in New York. Show me available shows in production and where they’re staffing.”

### Expected Output (Must)
Return up to 5 ranked result cards, each with:
- Title / type (scripted / unscripted / commercial)
- Location
- Confidence label: Confirmed / Likely / Unverified
- One-line “Why this matched”
- Next action button: Save / Refine / Outreach Template

### Follow-Up Prompt
“Filter to scripted only. Prioritize the next 30 days.”

### Expected Output (Must)
- Results re-ranked
- Filters applied
- Clear reasoning for changes

### “Speed of Imagination” Moment (Should)
Agent suggests 1–2 readiness improvements, e.g.:
- Add secondary markets (NJ/CT) to increase match rate
- Clarify kit / wireless count / timecode ecosystem / IFB workflow
- Suggest a short skills or certification improvement aligned to demand

---

## 2) Scene Two — Producer Agent: Source Vendors (90 seconds)

### Prompt 2
“I’m producing a 3-camera sitcom in Savannah, GA. I need a production sound rental partner. Requirements: 8 wireless, timecode, IFB, cart build, backup recorder.”

### Expected Output (Must)
Return 3–5 vendor cards, each with:
- Capability match summary
- Logistics (local vs nearby)
- Confidence label
- Next action: Outreach template (ready-to-send)

### Follow-Up Prompt
“Show me two alternates in Atlanta if Savannah inventory is tight.”

### Expected Output (Must)
- 2 alternates displayed
- Notes on tradeoffs (distance, availability assumptions)

---

## 3) Scene Three — Producer Agent: Hire Crew (60 seconds)

### Prompt 3
“I need a sound mixer with multi-cam sitcom experience available within 3 weeks.”

### Expected Output (Must)
Return a shortlist of candidates with:
- Why match (experience fit, location, availability cues)
- Confidence label
- A short “What I still need” question only if necessary:
  - Union requirement?
  - Expected kit?
  - Dates?
  - Budget band?

---

## 4) Close (15 seconds)

**Close Line (Demo operator says):** 
“One platform: jobs, vendors, and readiness intelligence — purpose-built for below-the-line. This is the speed of imagination applied to staffing.”

---

## 5) Fail-Safes (Mandatory for Live Demo)

If results are low-confidence:
- Agent must say so clearly and provide:
  - broader radius suggestion
  - adjacent classifications suggestion
  - alternate sourcing suggestion (vendors, coordinators, etc.)

If dataset is incomplete:
- Agent must label results as “Unverified” and propose next actions rather than hallucinate facts.

---

## 6) Demo Acceptance Criteria (Pass/Fail)

**Pass if:**
- Each prompt returns useful results within 10 seconds
- Results appear industry-real and role-aware
- Confidence labeling prevents hallucinated certainty
- The role flip (crew → producer) feels seamless

**Fail if:**
- Dead clicks, blank pages, or slow responses
- Agent invents productions as fact
- Unclear why results were returned
