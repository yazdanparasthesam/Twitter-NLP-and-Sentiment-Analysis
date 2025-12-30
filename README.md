Social Narrative Intelligence: SNA & Transformer-Based Sentiment Analysis
Hybrid Narrative Extraction | Graph Theory | MLOps
📌 Overview
This repository contains a production-grade pipeline for analyzing large-scale social data. The project bridges the gap between Network Science and Natural Language Processing to identify how ideologies spread through social clusters. It goes beyond simple sentiment analysis by mapping sentiment to specific community structures (Social Tribes).

🚀 Key Features
Community Detection: Uses the Louvain Algorithm to identify hidden social clusters within millions of interaction edges.

Narrative Extraction: Implements LDA (Latent Dirichlet Allocation) for automated topic discovery within specific communities.

Advanced NLP: A multi-stage pipeline utilizing Transformers (BERT) and VADER/TextBlob for high-accuracy sentiment and polarity scoring.

SNA Metrics: Calculated Betweenness Centrality and PageRank to identify high-impact influencers and "bridge nodes" that link different narrative bubbles.

🛠️ Tech Stack
Machine Learning: Scikit-learn, BERT (HuggingFace), XGBoost.

Graph & SNA: NetworkX, Louvain-Community.

MLOps & Tracking: MLflow for experiment tracking and Kubeflow for workflow orchestration.

Data Engineering: Pandas, NumPy, SQL.

Visualization: Pyvis (for interactive graph HTMLs), Matplotlib, Seaborn.

📂 Project Structure
Bash

├── Analysis_Notebook.ipynb   # Main end-to-end ML pipeline
├── data/                     # Raw & Processed datasets
├── src/                      # Production scripts
│   ├── graph_engine.py       # SNA & Community detection logic
│   ├── nlp_processor.py      # Sentiment & Topic modeling
│   └── serving.py            # API logic for real-time analysis
├── mlflow_logs/              # Model versioning & metadata
└── requirements.txt          # Environment dependencies
📊 Methodology
Network Construction: Interaction data is transformed into a directed graph where nodes represent users and edges represent information flow.

Cluster Segmentation: The Louvain algorithm identifies dense communities.

Sentiment Mapping: Sentiment scores are aggregated at the cluster level to identify "Ideological Hotspots."

Influence Ranking: Users are ranked by their ability to control information flow (Centrality metrics).

⚙️ MLOps Integration
This project is designed for Reproducible AI:

MLflow: Used to log hyperparameters (Learning Rate, Community Resolution) and store model artifacts.

Kubeflow: The pipeline is modularized for deployment as a Kubeflow Pipeline (KFP) on Kubernetes.

📈 Performance
Narrative Classification: Achieved a 92% F1-score on theme detection.

Scalability: Optimized for high-throughput processing of social streams via efficient vectorization.

🤝 Contact
Hesam Yazdanparast Machine Learning Engineer | Data Scientist

LinkedIn | GitHub
