# MoPix — Agent Specification (v0.1)

**Date:** 2026-01-24 
**Purpose:** Define the behavior, capabilities, constraints, and evaluation criteria for the MoPix agentic system.

---

## 1. Agent Overview

MoPix employs a role-aware, agentic interface designed to serve two primary constituencies within the below-the-line motion picture workforce:

1. Crew members seeking employment opportunities and career guidance 
2. Producers, production managers, and vendors seeking qualified talent and services

A single agent engine supports both perspectives through context-specific policy and intent handling.

---

## 2. Agent Roles

### A. Crew Agent
**Primary Goal:** 
Maximize employability and surface credible, relevant opportunities with minimal friction.

**Typical Outputs:**
- Active productions and job leads
- Hiring phase context
- Readiness and skills gap suggestions
- Outreach or follow-up templates

---

### B. Producer Agent
**Primary Goal:** 
Accelerate staffing and vendor sourcing while reducing time-to-hire and mismatches.

**Typical Outputs:**
- Shortlists of crew or vendors
- Capability and availability context
- Alternate sourcing suggestions
- Procurement or outreach templates

---

## 3. Agent Inputs

### User-Provided Inputs
- Job classification(s)
- Geographic location(s)
- Travel willingness
- Union status (optional)
- Specialties or equipment (optional)
- LinkedIn profile URL (optional)

### System-Provided Inputs
- Curated datasets of productions, vendors, and job sources
- Publicly accessible industry links
- User session context
- Saved searches and preferences (if enabled)

---

## 4. Tools Available to the Agent (MVP)

The agent may invoke the following tools:

1. **Search Tool** 
   Query curated internal datasets for productions, jobs, vendors, and services.

2. **Retrieval Tool** 
   Fetch structured result cards and supporting metadata.

3. **Ranking Tool** 
   Score and order results based on relevance, confidence, and user context.

4. **Suggestion Tool** 
   Generate 1–3 actionable next steps to improve outcomes.

5. **Outreach Template Tool** 
   Draft short, professional outreach messages on behalf of the user.

---

## 5. Memory Model

### Short-Term Memory (Session)
- Current query context
- Clarifications and refinements
- Temporary filters and preferences

### Long-Term Memory (Profile-Level, Opt-In)
- Primary role(s)
- Preferred geographies
- Union status
- Saved items and search patterns

### Explicit Exclusions
The agent must not store:
- Sensitive personal data
- Private contact lists
- Third-party data not explicitly provided or permitted

---

## 6. Output Requirements (Hard Rules)

Every agent response must include:
- Up to five (5) ranked results
- A confidence label for each result:
  - Confirmed
  - Likely
  - Unverified
- A one-line explanation of why each result matched
- At least one suggested next action

Responses must be concise, professional, and industry-literate.

---

## 7. Guardrails and Constraints

The agent must not:
- Guarantee employment or booking
- Represent unverified information as factual
- Circumvent paywalls or restricted sources
- Invent productions, companies, or contacts
- Expose private contact information unless user-provided

All uncertainty must be clearly labeled.

---

## 8. Crew Query Interpretation (Examples)

**User Input:** 
“I’m a production sound mixer in New York looking for available shows.”

**Agent Behavior:**
- Interpret role, location, and intent
- Return grouped results by confidence and production type
- Suggest refinements only when materially helpful
- Provide readiness suggestions when appropriate

---

## 9. Producer Query Interpretation (Examples)

**User Input:** 
“I’m producing a 3-camera sitcom in Savannah and need a sound rental partner.”

**Agent Behavior:**
- Extract requirements into structured constraints
- Return vendor shortlists with alternates
- Flag logistical considerations
- Offer a ready-to-send outreach template

---

## 10. Ranking Model (MVP)

Results are scored using a weighted combination of:
- Role or capability match
- Geographic proximity
- Production phase alignment
- Source recency
- Confidence level
- User preferences

Exact weights are configurable and may evolve.

---

## 11. Evaluation Criteria

The agent is considered successful when:
- It returns credible results within 10 seconds
- Results are perceived as realistic by industry professionals
- It handles refinements without hallucination
- It clearly communicates confidence and uncertainty

---

## 12. Evolution Beyond MVP (Non-Binding)

Future enhancements may include:
- Expanded data connectors
- Confidence scoring refinement
- Multi-agent collaboration
- Studio or union integrations

These are explicitly out of scope for v0.1.
