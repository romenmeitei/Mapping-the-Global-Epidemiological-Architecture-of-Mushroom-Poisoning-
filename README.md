**Mapping the Global Epidemiological Architecture of Mushroom Poisoning Research Using Transformer-Based NLP
**
This repository contains all datasets, analysis scripts, and reproducible workflows associated with the manuscript:

**"Mapping the Global Epidemiological Architecture of Mushroom Poisoning Research Using Transformer-Based Natural Language Processing"**

The study applies SciBERT-based transformer embeddings integrated with BERTopic clustering to reconstruct the thematic and geographic structure of mushroom poisoning research indexed in PubMed (2000–2025).

**📌 Study Overview**

This project:

Conducted a PRISMA-guided systematic literature review

Generated SciBERT contextual embeddings

Applied UMAP dimensionality reduction

Performed HDBSCAN clustering

Conducted BERTopic modeling

Computed inter-topic cosine similarity

Extracted geographic publication patterns

Modeled temporal trends using Poisson regression

The analysis identified three principal domains:

Clinical Hepatotoxicity

Outbreak & Epidemiology

Acute Clinical Cases

**📂 Repository Structure**
📊 Core Datasets
01_Final_Dataset_With_Topics.csv

Full dataset with document-level topic assignments (n = 1,219 initial records).

Final_Curated_Dataset_With_Topics.csv

Curated toxicology-focused corpus used for final topic modeling (n = 189).

Table_1_Topic_Summary.csv

Summary statistics of topic distribution and proportions.

**🧠 Topic Modeling Outputs**
03_Topic_Keywords_Weights.csv

Top representative keywords and c-TF-IDF weights for each topic.

04_Topic_Similarity_Matrix.csv

Cosine similarity matrix between topic embedding centroids.

05_UMAP_2D_Plot_Data.csv

Two-dimensional UMAP projection coordinates used for visualization.

06_Topic_Probabilities.csv

Document-level topic probability scores.

**🌍 Geographic Analysis**
Country_Publication_Counts.csv

Aggregated publication counts per country.

country_topic_matrix.csv

Country × Topic interaction matrix.

country_year_trend.csv

Country-specific temporal publication trends.
**
📈 Temporal Trend Analysis**
overall_year_trend.csv

Annual publication counts across the full study period.

topic_year_trend.csv

Annual publication counts stratified by topic.

**📓 Jupyter Notebooks (Reproducible Pipelines)**
Mapping the Global Epidemiological Architecture of Mushroom Poisoning.ipynb

Main end-to-end analysis pipeline:

Embedding generation (SciBERT)

UMAP reduction

HDBSCAN clustering

BERTopic modeling

Similarity matrix generation

Geographic extraction

TIME_TREND_ANALYSIS.ipynb

Poisson regression modeling and temporal trend visualization.

**⚙️ Software Environment**

Analyses were conducted using:

Python 3.x

sentence-transformers

BERTopic

UMAP-learn

HDBSCAN

scikit-learn

pandas

matplotlib

seaborn

plotly

geopandas

statsmodels

Random seeds were fixed to enhance reproducibility.
