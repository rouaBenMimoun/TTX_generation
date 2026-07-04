- **`stix/`** — Generated STIX 2.1 bundles produced by the Scenario Generation GPT (LLM₂), representing the structured cyber threat intelligence underlying each tabletop exercise (threat actors, malware, attack patterns, infrastructure, incidents, and relationships).
  - `financial_sector/` — STIX bundles for the 10 exercises targeting the financial sector.
  - `other_sectors/` — STIX bundles for the remaining 14 exercises, spanning healthcare, energy, and other sectors.
- **`ttx/`** — Complete, facilitation-ready tabletop exercises produced by the TTX Reconstruction GPT (LLM₃) from the corresponding STIX scenarios. Each document follows the standardized structure described in the paper (Preparation, Scenario, Response, Analysis).
  - `financial_sector/` — TTX documents for the 10 financial sector exercises.
  - `other_sectors/` — TTX documents for the remaining 14 exercises.



## Contents Overview

A total of 24 generated tabletop exercises are included. The **financial sector** subset (10 exercises) addresses ransomware, business email compromise, insider threats, cloud misconfigurations, DDoS, third-party/supply-chain compromise, payment fraud, social engineering, and data integrity attacks, targeting operational domains such as payment systems, digital banking, SWIFT infrastructure, and regulatory compliance. The **other sectors** subset (14 exercises) covers healthcare, energy, and additional industries.

## Format Notes

- STIX files are provided as valid STIX 2.1 JSON bundles and can be validated or visualized using standard STIX tooling (e.g., OASIS `stix2` Python library, OpenCTI, MISP).
- TTX documents are provided in PDF format, following the hierarchical structure: Preparation → Scenario → Response → Analysis, including MITRE ATT&CK mappings and STIX-to-scenario traceability notes.

## Citation

If you use these artifacts in your research, please cite:

> Ben Mimoun, R., Saint-Hilaire, K. A., Ben Salem, R., Cuppens, F., Boulahia-Cuppens, N. *Automated Generation of Cybersecurity Tabletop Exercises using custom LLMs.*

## License

This repository is released for academic and research purposes only. Some source tabletop exercises used to build the underlying knowledge base were provided by industrial partners under confidentiality arrangements; accordingly, redistribution or commercial use of the generated artifacts is not permitted without prior authorization. Please contact the authors for licensing inquiries.

## Contact

Roua Ben Mimoun — roua-2.ben-mimoun@etud.polymtl.ca# TTX_generation
