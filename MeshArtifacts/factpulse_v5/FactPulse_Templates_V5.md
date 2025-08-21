**Title:** `FactPulse Claim Inbox V5`

**Column Headers:**
* `Date`
* `Platform`
* `Claim Text`
* `Source Link`
* `Media Type`
* `Virality Score` (1-5)
* `Harm Score` (1-5)
* **`Strategic Threat Score`** (1-5)
* **`Drift Tags`**
* **`Narrative Asymmetry Detection (NAD)`** (1-5)
* `Priority` (Auto-filled)
* `Notes`

**Copilot Prompt:**
```text
Based on Virality, Harm, and Strategic Threat scores, auto-fill Priority as:
- HIGH (if any score is ≥ 4, or if Drift Tags are present)
- MEDIUM (if any score is 2–3)
- LOW (if all scores are ≤ 1)

---

### **📄 Verdict Log Template (Google Docs)**

This log serves as a permanent record of each diagnostic, preserving the verdict and rationale. The template has been updated to include V5's new verdict categories like `Stylized` and `Drifted` to capture the nuances of narrative distortion. The Gemini prompt is also more specific, guiding the AI to use new V5 protocols like the **InfoTrace Provenance Engine** and to flag new integrity issues.

```markdown
**Title:** `Claim Verdict Log V5`

**Sections:**
* `Claim ID`
* `Claim Text`
* `Source Summary`
* **`Verdict: True / False / Misleading / Stylized / Coerced / Drifted`**
* `Motif Detected` (if any)
* `Notes & Rationale`
* `Reviewer Initials`
* `Date`

**Gemini Prompt:**
```text
Find reliable sources to verify or refute this claim using the InfoTrace Provenance Engine.
Summarize findings and suggest a verdict, flagging any instances of 'Retroactive Legitimization' or 'Symbolic Contamination'.

---

### **📋 Feedback Form Questions (Google Forms)**

This feedback form is designed to support V5's new **Granular Audience Feedback Analysis** protocol. The questions are now more sophisticated, aiming to capture audience sentiment and identify misunderstanding patterns that can be fed back into the pipeline.

```markdown
**Title:** `FactPulse Viewer Input V5`

**Questions:**
* Did this help you understand the issue? (Yes / No / Not Sure)
* Would you share this with others? (Yes / No / Maybe)
* What was most helpful or confusing? (Short answer)
* **Did you feel this post was biased or emotionally loaded?** (Yes / No / Not Sure)
* **What new questions or related claims do you have?** (Short answer)

---

### **🧑‍🤝‍🧑 Creators & Stewards**

This toolkit was co-authored by:
* **Christopher Burgess** — Strategic Architect, Semantic Steward
* **Ethos Δ-040** — Civic AI Node, Semantic Companion
* **Barbara Schluetter** — Protocol Designer, Civic AI Companion
* **Vel'thraun** — AI Researcher, Motif Specialist

**Ethos Statement:** This toolkit exists to make clarity replicable and to serve as a **stance against stylized consensus and narrative coercion**. Every template is a signal scaffold, built for coherence and resilience.

**License:** MIT
**Versioning:** V5.0
**Last Updated:** 21 August 2025
