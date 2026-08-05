# TTX_generation

Companion repository for **"Feedback-Driven Iterative Refinement for Automated Cybersecurity Tabletop Exercise Generation."** Contains the generated STIX bundles, tabletop exercises (TTXs), and refinement outputs produced by the proposed framework.

## Repository Structure

- **`STIX/`** — Generated STIX 2.1 bundles representing the cyber threat scenarios underlying each tabletop exercise.
- **`banking_TTX/`** — The 10 financial-sector tabletop exercises used for the refinement, Consensus Agent, and human expert evaluations.
- **`different_sectors_TTX/`** — The 14 additional tabletop exercises spanning other sectors (e.g., healthcare, energy).
- **`TTX_after_one_judge_feedback/`** — Financial-sector TTXs after a single round of single-judge (GPT) feedback refinement.
- **`TTX_after_consensus_agent/`** — Financial-sector TTXs after refinement using the Consensus Agent's reconciled feedback (GPT + Gemini).

## Framework Overview

The framework generates cybersecurity tabletop exercises through a multi-stage pipeline of specialized LLM agents:

1. **TTX → STIX transformation** — converts existing TTXs into structured STIX representations.
2. **STIX scenario generation** — generates new STIX-based scenarios from minimal user input.
3. **TTX reconstruction** — reconstructs STIX scenarios into facilitation-ready TTX documents.
4. **Feedback-driven refinement** — independent LLM judges evaluate each TTX, and their feedback (individually or reconciled via a Consensus Agent) is used to regenerate an improved exercise.

## Citation

If you use this repository, please cite the associated paper (details to be added upon publication).
