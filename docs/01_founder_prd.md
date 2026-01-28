# MoPix — Founder PRD (MVP v0.1)

**Version:** 0.1 
**Owner:** [Your Name] 
**Date:** 2026-01-24 
**Core Brand Value:** *The Speed of Imagination*

---

## 1. Product North Star

Build the fastest, most trustworthy way for below-the-line film and television professionals and hiring managers to find each other using an agentic interface that understands job classifications, production context, geography, and availability.

MoPix is designed to reduce friction, increase signal, and shorten time-to-hire across the motion picture industry workforce.

---

## 2. Problem Statement

Below-the-line hiring is fragmented across static job boards, union rosters, personal networks, Facebook groups, and informal text chains. These systems do not scale, do not adapt in real time, and do not support workforce evolution in the age of AI-assisted production.

The result is slow hiring, missed opportunities, uneven access, and poor visibility into readiness gaps for both crew and producers.

---

## 3. Target Users

### Supply (Crew)
- Production Sound Mixers, Boom Ops, Utilities
- Camera Department, G&E, Art, Wardrobe
- Post Production: Editors, Assistant Editors, Colorists, Sound Editorial

### Demand (Hiring)
- Producers, Line Producers, UPMs
- Production Managers, Coordinators
- Vendors and rental houses (sound, camera, grip, lighting, post)

---

## 4. MVP Objective

In a live executive demo, MoPix must:
- Accept a user’s role, location, and preferences
- Return credible job, production, or vendor opportunities in seconds
- Explain *why* each result matched
- Suggest actionable next steps
- Seamlessly flip perspectives between crew and producer use cases

---

## 5. MVP Scope (Included)

### A. Conversational Agent Interface
Users interact via natural language queries such as:
- “I’m a production sound mixer in New York. Show me available shows in production.”
- “I’m producing a 3-camera sitcom in Savannah and need a production sound rental partner.”

### B. Frictionless Profile Intake
- Name
- Primary job classification(s)
- Preferred work locations
- Union status (optional)
- LinkedIn profile URL (optional)

No resume parsing or document uploads in v0.1.

### C. Results Presentation
Each result includes:
- Title / type
- Location
- Confidence level (Confirmed / Likely / Unverified)
- One-line explanation of match
- Suggested next action (save, refine, outreach)

### D. Saved Items
Users may save jobs, vendors, and searches for later reference.

### E. Industry Resources
Curated links to publicly accessible industry news, events, and resources (no paywalled content).

---

## 6. Explicit Non-Goals (Out of Scope for MVP)

- Full social networking (DMs, groups, feeds)
- Verified union integrations
- Payments, contracts, or payroll
- Course marketplace or CE tracking
- Large-scale automated scraping

---

## 7. Key Differentiators

- Agentic, conversational search
- Below-the-line job classification literacy
- Two-sided marketplace (crew and hiring)
- Speed: time-to-first-useful-result under 10 seconds (demo target)

---

## 8. Data Strategy (MVP)

Phase 1:
- Curated, manually seeded datasets for productions, vendors, and job sources
- Periodic lightweight refresh

Phase 2 (post-MVP):
- Expanded monitoring
- User-contributed intelligence
- Confidence scoring improvements

---

## 9. Trust, Safety, and Accuracy

- No guarantee of employment
- No private contact exposure unless user-provided
- Clear confidence labeling
- Clear disclaimers regarding verification responsibility

---

## 10. Success Metrics

- Time to first useful result
- Saves per session
- Repeat usage within 7 days
- Producer search → outreach action rate

---

## 11. Technical Direction (MVP)

- Frontend: React Native (Expo) or responsive web
- Backend: lightweight API with hosted database
- Agent layer: LLM-powered agent with tool access for search, ranking, and suggestions
