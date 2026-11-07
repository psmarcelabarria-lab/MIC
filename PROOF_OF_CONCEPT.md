# Proof of concept — Diagnóstico MIC para Plataformas

**External demonstration:** https://iaysaludmental.com/diagnostico_plataformas_mic.html  
**Owner / author:** Marcela Barría Cárdenas  
**Classification:** Exploratory self-report prototype; **not** a validated instrument, independent audit or certification.

## Purpose
Demonstrate a possible translation of the MIC's three public-facing domains—Soberanía, Secreto and Profundidad—into a structured, browser-based reflection workflow for AI platforms operating near psychology or mental health.

## Features observed in the prototype
- A questionnaire organized around the three domains.
- Separate framing for professional-facing and patient-facing uses, plus a combined-use option.
- Five questions per domain in the selected questionnaire path, with structured responses.
- Domain-level numerical summaries and explanatory feedback.
- Client-side PDF report generation.
- A research-consent checkbox displayed in the interface.

**Important:** These are implementation characteristics, not evidence of measurement validity or legal compliance.

## Known methodological and technical limitations
1. **Combined-use path:** the mixed modality currently reuses professional-facing questions, so it cannot support conclusions about both audiences without revision.
2. **Unknown answers:** an “I don't know” response is excluded from the sum while the denominator stays fixed; this can misrepresent missing knowledge as a low score.
3. **Thresholds:** numerical ranges and equal weights are heuristic; there is no demonstrated empirical basis for classification or cut-offs.
4. **Non-compensatory conditions:** potentially critical safeguards may need explicit alerts rather than compensation by other positive answers.
5. **Research consent:** access to PDF output should not be conditioned on optional research participation.
6. **Data capture:** the reviewed prototype did not implement a research-submission backend. Checking consent does not itself create a research dataset.
7. **Scope:** a platform's self-report cannot verify its actual privacy practices, clinical safety, regulatory compliance or real-world behavior.

## What the prototype establishes
It establishes the feasibility of a simple user experience that organizes questions and returns structured feedback. It **does not** establish psychometric reliability, validity, external audit findings or safe deployment for clinical decision-making.

## Proposed next iteration
- Document construct-to-question mapping, without publishing protected items.
- Correct combined-use routing and missing-data handling.
- Separate educational feedback from evaluative classifications.
- Introduce transparent uncertainty and safety-critical criteria.
- Decouple research consent from report download.
- Design data collection, security and governance only after approval of a research protocol.
- Conduct expert review and usability testing using synthetic scenarios.

## Intellectual-property boundary
This document describes the external demonstration. It does **not** release its underlying code, proprietary items, scoring logic or branding under an open-source license. Future open components will be specified and licensed separately.
