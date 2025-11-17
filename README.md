# Quantitative-Mapping-of-Conceptual-Hierarchies-and-Data-Driven-Taxonomies-of-Japanese-Architectural
Paper materials
This repository contains the supplementary materials, analysis scripts, configuration files, and complete results for the paper, "Quantitative-Mapping-of-Conceptual-Hierarchies-and-Data-Driven-Taxonomies-of-Japanese-Architectural."

The project uses Natural Language Processing (NLP) techniques (including BERT and Word2Vec) to perform a data-driven clustering analysis and quantitative mapping of conceptual hierarchies within Japanese architectural discourse.

📚 Data Source
The pre-processed data used for fine-tuning the models in this study is available in the repository of the preceding paper. You can access and download it from the following link:

[Reproducibility-and-Validation-of-a-Computational-Framework-for-Architectural-Semantics](https://github.com/ArchiScrub/Reproducibility-and-Validation-of-a-Computational-Framework-for-Architectural-Semantics)

🗂️ Repository Structure
This repository is organized into directories based on the experimental parameters and random seeds used to ensure reproducibility.

Config_yalm...: YAML configuration files detailing the parameters for the conceptual alignment and exploratory ARI (Adjusted Rand Index) experiments.

Script...: The main scripts used to run the conceptual alignment and exploratory analyses.

seeds_from_grouping: Contains logs and data related to the seed-finding process for clustering.

Ma = 1/Results & Results/Ma = 0: These directories contain the full experimental results, separated by the paper's main parameter (Ma, likely "Conceptual Alignment" on or off).

No Pin: Contains results for experiments run without a "pinning" or "seeding" constraint.

Within the results directories, you will find sub-folders for each experimental run, categorized by their random seed:

run_seed_42/

run_seed_527/

run_seed_777/

📄 Key Files & Outputs
Each run_seed_... folder contains a comprehensive set of output files from the analysis. Key files include:

Figures/: Contains CSV files with aggregated data used to generate the figures in the paper.

paper2_clusters_clean_... & paper2_clusters_full_...: CSV files detailing the assigned cluster for each term, for both "clean" (pre-processed) and "full" datasets, using different models (BERT, W2V, etc.).

paper2_cluster_exemplars_...: Text files showing the most representative terms (exemplars) for each cluster, which helps in qualitatively interpreting the clusters.

paper2_confirmatory_parity_...: CSV files containing the results of the confirmatory parity analysis.

paper2_exploratory_ari_summary.csv: A summary file of the Adjusted Rand Index (ARI) scores, a key metric for evaluating the clustering results.

Final run report exploratory ARI...: A final text report summarizing the results for a given experimental configuration.

paper2_env.json: A JSON file capturing the environment and parameters for a specific run.



### Third-party libraries

The scripts in this repository depend on external libraries
(e.g. `transformers`, `scikit-learn`, and other Python packages).
Those libraries are **not** covered by the licences in this
repository. They keep their own original licences as distributed
upstream.
