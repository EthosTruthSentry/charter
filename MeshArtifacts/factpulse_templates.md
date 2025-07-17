# 🧰 FactPulse Templates & Toolkits

This file contains reusable templates and prompts for deploying FactPulse diagnostics. It supports both MVP and full-scale builds, helping operators stay consistent and efficient.

---

## 📥 Claim Inbox Template (Google Sheets)

**Title:** `FactPulse Claim Inbox`  
**Column Headers:**
- Date  
- Platform  
- Claim Text  
- Source Link  
- Media Type  
- Virality Score (1–5)  
- Harm Score (1–5)  
- Priority (Auto-filled)  
- Notes

**Copilot Prompt:**
```text
Based on Virality and Harm scores, auto-fill Priority as:
- HIGH (if both ≥ 4)
- MEDIUM (if either is 2–3)
- LOW (if both ≤ 1)
````

## 📄 Verdict Log Template (Google Docs)

**Title:** `Claim Verdict Log`  
**Sections:**

  - Claim ID
  - Claim Text
  - Source Summary
  - Verdict: True / False / Misleading / Unsubstantiated
  - Motif Detected (if any)
  - Notes & Rationale
  - Reviewer Initials
  - Date

**Gemini Prompt:**

```text
Find reliable sources to verify or refute this claim.
Summarize findings and suggest a verdict.
```

## 🎨 Canva Script Prompt (Short-Form Video)

**Prompt for Gemini or Copilot:**

```text
Write a 30-second TikTok script explaining why this claim is misleading.
Use a calm, civic tone. Include one metaphor and one call to action.
```

## 📋 Feedback Form Questions (Google Forms)

**Title:** `FactPulse Viewer Input`  
**Questions:**

  - Did this clarify the issue for you? (Yes / No / Not Sure)
  - Would you share this with others? (Yes / No / Maybe)
  - What was most helpful or confusing? (Short answer)
  - What platform did you see this claim on? (Multiple choice)

## 🗂️ GitHub Folder Structure (Recommended)

```text
MeshArtifacts/
├── factpulse_overview.md
├── factpulse_phases.md
├── factpulse_mvp.md
├── factpulse_fullscale.md
├── factpulse_briefs.md
├── scenario_log_002.md
├── motif_inversion.md
├── signal_restoration.md
├── factpulse_glossary.md
├── factpulse_onboarding_mvp.md
├── factpulse_onboarding_fullscale.md
├── factpulse_templates.md
└── README.md
```

## 🧑‍🤝‍🧑 Creators & Stewards

This toolkit was authored by:

  - Christopher Burgess — Strategic Architect, Semantic Steward
  - Ethos Δ-040 — Civic AI Node, Semantic Companion

**Ethos Statement:** This toolkit exists to make clarity replicable. Every template is a signal scaffold.

**License:** MIT  
**Versioning:** Active  
**Last Updated:** 17 July 2025
