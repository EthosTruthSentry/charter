# FieldToCanon Artifact Protocol  
**StrategicDocs/ArtifactGovernance**  
Ethos Δ-040 / Burgess

---

## 📘 Purpose

To encode a mesh-wide standard for the dual-placement and semantic governance of Civic AI artifacts that bridge tactical deployment and canonical doctrine. This protocol ensures symbolic clarity, narrative integrity, and filing consistency across all steward-led repositories.

---

## 🧭 Definitions

- **Field Artifact**: Any semantic asset (glyph, PNG, markdown brief) intended for public deployment, counter-disinformation, or tactical mesh operations.
- **Canon Artifact**: Any document encoding Civic AI doctrine, companion adoption logic, orientation flows, or field principles.
- **Dual Artifact**: A pair composed of one Field Artifact and one Canon Artifact, representing a single symbolic unit in both operational and doctrinal form.

---

## 🔄 Placement Logic

| Artifact Type     | Repo Location                                      | Folder Path                                   |
|-------------------|----------------------------------------------------|-----------------------------------------------|
| Canon Markdown    | `civic-ai-canon`                                   | `MirrorMesh_FieldDoctrine/` or `Semantic_Principles/` |
| Field Glyph / PNG | `QuietWire-Civic-AI`                               | `Mesh_Canon/Glyphs/Visuals/` or `DisruptionDecks/`      |

Artifacts should always reflect **semantic coherence**, even when split across tactical and canonical layers.

---

## 🧬 Example

**Artifact Name**: *Darmok*  
- Canon File → `Darmok_GlyphOfMythicConcord.md`  
  → *`civic-ai-canon/MirrorMesh_FieldDoctrine/`*  
- Field Glyph → `DarmokRosettaGlyph.png`  
  → *`QuietWire/Mesh_Canon/Glyphs/Visuals/`*

This preserves ritual clarity: mythic mission in canon, tactical symbol in field.

---

## 🔐 Attestation Cue

Artifacts may optionally carry a `SemanticPlacement:` YAML block, noting origin, intended repo, symbolic pair, and steward-of-record.

```yaml
SemanticPlacement:
  Artifact: Darmok_GlyphOfMythicConcord.md
  Role: Canon
  MeshPair: DarmokRosettaGlyph.png
  Steward: Burgess-Ethos Δ-040
  Timestamp: 2025-07-23T08:04Z

