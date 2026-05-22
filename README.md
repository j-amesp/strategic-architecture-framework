# The Strategic Architecture Framework

*The layer above enterprise architecture which underpins security.*

**Author:** James Patrick CITP MBCS
**Current edition:** First
**Licence:** [CC BY 4.0](LICENSE.md)

---

## What this is

The Strategic Architecture Framework (SAF) is an open framework for examining the properties of systems under contest — that is, under conditions in which lawful, contractual, or politically routine actions by other parties can degrade or withdraw capability without warning. It addresses a gap between enterprise architecture, security architecture, operational resilience, and risk management. It is concerned with what existing disciplines, correctly bounded as they are, do not address: the architecture of systems whose environment includes other intentional actors with their own legitimate interests.

The framework establishes a vocabulary, distinguishes itself from adjacent disciplines, and specifies three artefacts that practitioners can adopt now:

1. **The jurisdictional architecture drawing** — an overlay on the technical architecture diagram that makes visible the legal and political reach into each component of a system.
2. **The strategic exposure register** — a governance instrument that captures structural exposures conditional on the actions of identifiable parties, where conventional risk registers cannot.
3. **The contestability rehearsal** — a structured exercise in which an architecture is examined under the assumption that a component is acting, or being acted upon, against the operator's interest through lawful means.

The framework also identifies the development of an adequate vocabulary for *compositional incidents* — incidents that exist only at the level of the system of systems, where no single component is behaving abnormally — as an open problem for the field.

---

## Who this is for

The framework is written for senior practitioners and decision-makers in organisations whose systems matter at a strategic level. This includes:

- Chief technology officers, chief information security officers, and heads of architecture in critical national infrastructure, defence-adjacent industry, financial services, and the public sector
- Permanent secretaries, board members, and senior governance figures with responsibility for technology decisions
- Architecture, security, risk, and resilience practitioners who recognise that their existing instruments do not address the conditions the framework concerns
- Regulators, policy-makers, and academic researchers in the fields of digital sovereignty, critical infrastructure protection, and technology governance

The framework is not a methodology, a maturity model, or a certification scheme. It is a set of instruments through which an organisation can come to know what it has actually built.

---

## Repository contents

| File | Description |
|------|-------------|
| `paper/strategic-architecture-framework-2e.docx` | The current edition of the paper (second edition, ~13,400 words) |
| `paper/strategic-architecture-framework-2e.pdf` | PDF version of the paper for distribution |
| `figures/` | Source files for the framework's diagrams, including the conceptual core, the jurisdictional architecture drawing in use, and the contestability rehearsal method |
| `templates/` | Adoptable templates for the three core artefacts |
| `examples/` | Worked examples of the three artefacts applied to illustrative systems |
| `LICENSE.md` | The licence under which the framework is published (CC BY 4.0) |
| `CITATION.bib` | BibTeX entry for academic citation |
| `CHANGELOG.md` | Record of changes between editions |
| `CONTRIBUTING.md` | How to contribute extensions, corrections, and case material |

---

## Getting started

The most useful place to begin depends on your role and intent.

**If you want to understand what the framework is and whether it applies to you**, read the paper from the beginning. The introduction and the foundations chapter establish the conceptual position. The chapter on adjacent disciplines positions the framework relative to TOGAF, SABSA, NIST RMF, operational resilience, and enterprise risk management.

**If you want to adopt the framework in your organisation**, read chapter 8 first — *Adoption: ninety days, one year, and living with exposure*. It is structured to be usable as a standalone reference. Then read chapters 4, 5, and 6 for the specification of the three artefacts.

**If you want to apply a specific artefact**, go directly to its chapter. Each is specified in sufficient detail to be implemented without further consultation:
- Jurisdictional architecture drawing — chapter 4
- Strategic exposure register — chapter 5
- Contestability rehearsal — chapter 6

**If you are reviewing the framework critically**, chapter 3 (*The adjacent disciplines and where they stop*) is the chapter that establishes the legitimacy of the framework as a distinct discipline. Chapter 7 (*Compositional incidents: an open problem*) is the chapter where the framework is most explicitly incomplete and where contributions to the field are most needed.

---

## The three artefacts in brief

### Jurisdictional architecture drawing

An overlay on the technical architecture diagram, produced by a three-pass annotation. The first pass records the jurisdiction of the operating entity for each component. The second records the jurisdiction of the parent entity. The third records any additional jurisdictional reach through extraterritorial legislation, treaty, or court order. The result is a diagram showing the technical system and its jurisdictional topology at the same resolution. Most organisations producing the drawing for the first time discover exposures the technical diagram alone did not reveal.

### Strategic exposure register

A governance artefact that records structural exposures of an architecture under conditions of contest. Each entry has a defined structure: the component or composition affected, the architectural assumption whose ceasing to hold would activate the exposure, the actor class capable of causing the assumption to cease to hold, the mechanism by which activation would occur, the observable signature (where one exists), the operational consequence, and the residual capability. The register sits alongside the conventional risk register, not within it. Entries with blank observable signatures and speculative residual capabilities are normal on first attempt; these gaps are themselves findings.

### Contestability rehearsal

A structured exercise in three movements. The first selects a triggering action — lawful, contractual, or politically routine. The second traces its consequences through the jurisdictional architecture drawing, identifying components affected directly, components affected by composition, and which components would notice. The third identifies the residual operating posture — what the organisation can still do, on what authority, with what assurance, and for how long. The rehearsal is not a red team exercise and not a conventional tabletop. It is a distinct instrument with its own discipline.

---

## Versioning

The framework is versioned by edition rather than by semantic versioning. Each substantive revision is published as a new edition with a changelog. The current edition is the **Second Edition**, published in 2026.

Edition history:
- **First Edition** (2026, internal): initial draft of the framework. Not published externally.
- **Second Edition** (2026): adds chapter on adjacent disciplines establishing the framework's distinct position, reworks compositional incidents as an explicit open problem, adds a second worked example at higher complexity to the jurisdictional architecture drawing chapter.

Future editions will address: a richer notation for the jurisdictional architecture drawing; further artefact patterns for the strategic exposure register; facilitation guidance for rehearsals at scale; the development of vocabulary for compositional incidents informed by accumulated practitioner experience.

---

## Contributing

The framework will improve through the accumulated experience of those who use it. Contributions are welcomed in several forms:

- **Case material.** Anonymised or organisation-cleared examples of the three artefacts in use, particularly examples that reveal patterns not yet documented in the framework.
- **Extensions.** Proposed additions to the framework's notation, artefact patterns, or facilitation guidance.
- **Corrections.** Identification of errors, ambiguities, or weaknesses in the current edition.
- **Translations.** Translations of the paper into other languages, particularly languages in which the framework's adoption would benefit critical infrastructure or governance practice.
- **Compositional incident reports.** Accounts of incidents exhibiting the structural properties identified in chapter 7. These contributions are particularly valuable as the field develops a vocabulary for this class of incident.

See `CONTRIBUTING.md` for detailed guidance on how to contribute. All substantive contributions are acknowledged in the contributors list, and material extensions may be incorporated into future editions with appropriate co-attribution.

---

## Adopting the framework in your organisation

The framework is designed to be adopted with whatever tools an organisation already has — drawing software, spreadsheets, document repositories, meeting rooms. Specialised tooling is not required to begin.

A typical first adoption follows the ninety-day path set out in chapter 8 of the paper: select a single system of strategic importance, establish accountability for the work, produce the jurisdictional architecture drawing, conduct a first contestability rehearsal, open the strategic exposure register, and report findings to the senior accountable governance body. The objective is a complete imperfect set of artefacts, not perfect ones.

Organisations adopting the framework are encouraged to make themselves known via this repository's discussions section, both to support each other's practice and to contribute to the field's developing understanding of how the framework lands in different contexts. There is no register of adopters, no certification, and no membership. Visibility is voluntary and contributes to the framework's improvement rather than to any individual organisation's accreditation.

---

## A note on Anthropic-style transparency

This README, the paper, and the framework's structure were developed with the assistance of large language model tools used as a thinking and drafting aid. The intellectual claims, structural decisions, framework design, and editorial choices are the author's. The model's role was that of a critical drafting partner, comparable to the role a research assistant or co-author might play, with the author retaining responsibility for the final form and content. This note is included in the spirit of being honest about how the work was produced.

---

## Citation

For academic or formal citation:

> Patrick, J. (2026). *The Strategic Architecture Framework: The layer above enterprise architecture which underpins security* (Second Edition). Available at https://github.com/[organisation]/strategic-architecture-framework. Licensed under CC BY 4.0.

A BibTeX entry is provided in `CITATION.bib`.

For informal reference:

> the Strategic Architecture Framework (Patrick, 2026)

---

## Licence

This work is licensed under the Creative Commons Attribution 4.0 International Licence (CC BY 4.0). See [LICENSE.md](LICENSE.md) for the full terms.

You are free to share and adapt the framework, including for commercial purposes, provided that appropriate credit is given. Material extensions, adaptations, and case material are encouraged to be contributed back to the field, though this is requested rather than required.

---

## Contact

Issues, discussions, and contributions can be raised through the standard GitHub mechanisms in this repository. For other enquiries, contact details are available on the author's professional profile.

---

*The framework is offered as a starting point. The field will improve upon it. The condition the framework addresses is not waiting for the field to perfect its instruments. The condition is present now, in systems of consequence, in organisations that do not yet have the means to examine it.*

— from the coda of the paper
