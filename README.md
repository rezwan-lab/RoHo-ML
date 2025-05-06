# RoHo-ML: Predicting Evolutionary Fitness of Viral Mutations for Early Detection of High-Risk Variants

## Background

RNA viruses such as SARS-CoV-2 mutate quickly, often acquiring changes that increase transmissibility or reduce vaccine effectiveness. Most current monitoring systems focus on frequency or case counts, which are reactive and often delayed. 

The **RoHo score** (Ratio of Homoplasic Offspring) is a phylogeny-based measure that captures how frequently a mutation arises independently and how successfully it spreads—highlighting signals of positive selection and convergent evolution.

Despite its value, RoHo has rarely been applied in predictive modeling. This project aims to combine RoHo scoring with machine learning and biological annotation to forecast high-risk mutations before they become widespread.

---

## Objectives

- Generate RoHo scores from mutation-annotated trees (e.g., UShER for SARS-CoV-2).
- Train ML models (XGBoost, CatBoost) to predict high-RoHo mutations using genomic features.
- Enrich predictions with biological context using LLMs and mutation databases (e.g., IEDB, GISAID).
- Build a mutation monitoring tool or dashboard for real-time prioritization.

---

## Methodology

- **Data**: Use `matUtils` to generate RoHo scores from UShER MATs.
- **Features**: Include mutation position, gene, mutation type, domain (e.g., RBD), recurrence, VOC status.
- **Modeling**: Train and evaluate models with AUC and SHAP for interpretability.
- **Enrichment**: Integrate LLMs (e.g., BioGPT) and structured databases for mutation impact context.
- **Output**: Ranked mutation table and dashboard-ready pipeline.

---

## Expected Outcomes

- A predictive framework for identifying mutations under positive selection.
- A mutation ranking system for use by public health or research labs.
- A working notebook or tool for genomic surveillance.
- Potential publications in computational biology, virology, or AI in genomics.

---

## Applications

- Real-time tracking of emerging viral mutations.
- Input for vaccine design and epitope mapping.
- Integration with platforms like Nextstrain or outbreak dashboards.

---

## Significance

This work combines phylogenetic insight, machine learning, and biological knowledge to prioritize viral mutations in advance—supporting early intervention and better pandemic response.

## Author
Rezwanuzzaman Laskar
