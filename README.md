<h1 align="center">Dhruvkumar Patel</h1>

<p align="center">
  Data Scientist @ Myntra · M.Tech CSE, IIIT Delhi · BlackboxNLP @ EMNLP 2026
</p>

<p align="center">
  <a href="https://www.stackdhruv.com">stackdhruv.com</a> ·
  <a href="https://www.linkedin.com/in/stack-dhruv">LinkedIn</a> ·
  <a href="https://scholar.google.com/citations?user=RZULQawAAAAJ&hl=en">Google Scholar</a> ·
  <a href="mailto:hello@stackdhruv.com">hello@stackdhruv.com</a>
</p>

---

I build production ML systems — ranking models, multimodal pipelines, and computer vision applications. Currently at **Myntra** on the Homepage Merchandising / Ads Ranking team, and a graduate researcher at the **MIDAS Lab, IIIT Delhi**, where my thesis work on separating perception failures from reasoning failures in multimodal LLMs is published at BlackboxNLP (EMNLP 2026).

---

## Experience

| Period | Role | Where |
|--------|------|--------|
| Jul 2026 – Present | Data Scientist | Myntra, Bengaluru |
| Jan 2026 – Jul 2026 | Data Scientist Intern | Myntra, Bengaluru |
| Jan 2025 – Present | Graduate Researcher (Thesis) | MIDAS Lab, IIIT Delhi |
| Jan – Jun 2024 | Jr. SDE Intern | Ishitva Robotic Systems |

**Myntra — Ads Ranking**
- Shipped a replacement ads-ranking model that delivered a statistically significant CTR lift in a live A/B test, after improving offline NDCG over both the incumbent production ranker and a heuristic baseline
- Extended the ranking objective from CTR alone to funnel-depth (CVR) metrics using deep multi-task ranking architectures
- Selected the production configuration through controlled ablations on loss function (pointwise binary-logistic → pairwise), boosting rounds, and auxiliary scalar features
- Built resumable, idempotent Databricks / PySpark pipelines for user and ad embedding generation, then migrated the entire embedding stack after diagnosing quality anomalies through EDA
- Authored the modular training-to-production codebase, MLflow-tracked experimentation through Triton runtime plan-file conversion

*Production metrics for this work are covered by an employment confidentiality agreement and are deliberately omitted.*

**MIDAS Lab — M.Tech Thesis** (M.Tech CGPA 8.08/10)
- Built a five-condition diagnostic framework that attributes multimodal LLM failures to perception, to reasoning, or to their interaction, holding the reasoning prompt fixed and varying only the visual grounding
- Ran ~140 inference runs across 6 multimodal LLMs and 5 physics/geometry benchmarks on a thread-pooled OpenRouter backbone with sliding-window rate limiting and idempotent checkpointing, so 8–12 hour jobs resume without recomputation
- Found that adding the diagram breaks up to **46.1%** of problems the model already solves from text alone; LLM-judge evaluation validated against a four-annotator majority vote at Cohen's κ 0.74–0.84
- Separately, fine-tuned Qwen-2.5-VL-72B-Instruct on 5× H100-SXM for annotation-anomaly detection, served through a GPU-backed FastAPI + Celery async batch backend — 100+ req/s, 35% lower end-to-end latency

---

## Selected Projects

| Project | Highlights |
|---------|------------|
| [**Mental Health Meme Classification**](https://github.com/stack-dhruv/mental-health-meme-classification) | Extends the M3H architecture with visual feature maps and Qwen-2.5-VL-7B semantic triplet extraction over OCR text; fine-tuned MentalBART · 65% / 63% Macro F1 on anxiety and depression · `PyTorch` `Transformers` `Streamlit` |
| [**Advanced ANPR & Face Recognition**](https://github.com/coding-brigade/advanced-anpr-fr) | YOLOv8-nano plate detection + fine-tuned ResNet-18 classifier (92% precision, 91% recall) with a Siamese few-shot face-recognition path for low illumination · **National Finalist, KAVACH-2023** · `YOLOv8` `ResNet` `FastAPI` `React Native` |
| [**Student Dropout Analysis**](https://github.com/ssip-hack/student-dropout-analysis) | Government dashboard turning UDISE+ data into ML dropout-risk forecasts · R² 0.9976 on the EduDropX dataset · **SSIP 2022 State Winner** · Published IEEE I2CT 2024 · `scikit-learn` `React` `MySQL` |
| [**Microservices Benchmarking**](https://github.com/stack-dhruv/DeathStarBench) | DeathStarBench social network across a local Docker Swarm cluster and GKE, benchmarking three replica/node configurations with two-tier observability — Pixie eBPF for real-time tracing, Prometheus for fine-grained metrics · `Kubernetes` `Docker Swarm` `Pixie` |

---

## Publications

- **Lost in Perception: Isolating Perceptual and Reasoning Failures in Multimodal Physics and Geometry Reasoning** · *BlackboxNLP Workshop, co-located with EMNLP 2026* · Budapest, Oct 2026
- **Unlocking Enigmatic Pathways: Empowering Student Dropout Analysis with ML** · *IEEE I2CT 2024* · [IEEE Xplore](https://ieeexplore.ieee.org/document/10543438/)

---

## Certifications

<p>
  <img src="images/certifications/aws-machine-learning-associate-mla-c01-600x600.png" width="80" alt="AWS ML Engineer Associate"/>
  &nbsp;
  <img src="images/certifications/azure-data-scientist-associate-600x600.png" width="80" alt="Azure Data Scientist Associate"/>
</p>

**AWS Certified Machine Learning Engineer – Associate** · issued Jul 2025
**Microsoft Certified: Azure Data Scientist Associate** · issued Jun 2024

---

## Stack

**ML / AI** · PyTorch · scikit-learn · Hugging Face · vLLM · OpenCV
**Infra** · FastAPI · Celery · Docker · Kubernetes · Databricks · PySpark · Triton
**Cloud** · AWS · Azure · GCP
**Languages** · Python · C++ · JavaScript · SQL
