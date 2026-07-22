# Processing Notes — RDHEI using GNN with Thumbnail-Preserving Encryption (Bharathidasan 2025)

- **Paper:** S. Bharathidasan, V. Tamil Selvi, V. Sathiya, Francis H. Shajin, Signal, Image and Video Processing, vol. 19, 2025
- **Reproduction tier:** C
- **Status:** Completed (literature review + partial demo)

## Reproduction scope
**Reproduced:** the ESTPE thumbnail-preserving cipher (block-mean preserved exactly, detail scrambled). **Not reproduced:** the similarity-navigated GNN predictor (no trained weights, dataset, or GPU pipeline in this workspace).

## Why full reproduction is not feasible here
The core novelty depends on a trained graph neural network; training it faithfully needs the paper's dataset and hardware. We therefore reproduce the encryption component and review the rest.

## Honesty note
Demo numbers are from the included code; all capacity/robustness figures attributed to the paper are NOT independently reproduced.
