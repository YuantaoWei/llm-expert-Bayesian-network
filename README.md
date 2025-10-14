BN-Bench: A Unified Library for Expert-Elicited and Synthetic Bayesian Networks

A curated and extensible library of **Bayesian Networks (BNs)** designed for **causal discovery**, **parameter learning**, and **algorithm benchmarking**.  
BN-Bench integrates both *canonical benchmark networks* (e.g., Asia, Student, Insurance) and *new expert-elicited datasets* derived from human judgments, enabling systematic evaluation of structure learning and inference methods under uncertainty.

---

Motivation

While existing repositories such as the [Bayesian Network Repository](https://www.bnlearn.com/bnrepository/) focus on classical, simulation-based networks, they lack *human-elicited* data that reflect subjective causal beliefs.  
BN-Bench bridges this gap by providing:

- **Expert-elicited BN data** collected from real human judgments  
- **Synthetic data generators** with tunable noise levels for robustness testing  
- **Evaluation pipelines** for structure learning and causal inference algorithms  
- **Standardized metrics** (Kendall’s τ, SHD, SID, F1) for fair benchmarking  

The goal is to promote **data sharing**, **method comparison**, and **transparent evaluation** across causal learning studies.

---

Repository Structure

| Folder | Description |
|:--|:--|
| `networks/` | Canonical Bayesian networks (Asia, Student, Insurance, Alarm, etc.) |
| `experts_data/` | Expert-elicited pairwise preference data and meta-information |
| `simulation/` | Synthetic data generation scripts for controlled experiments |
| `evaluation/` | Metric implementations and benchmark reports |
| `notebooks/` | Interactive notebooks for data loading, visualization, and evaluation |
| `docs/` | Dataset cards and collection documentation |

---

Included Networks

Classic Discrete Bayesian Networks

| Name | Nodes | Arcs | Parameters | Description |
|:------|:------:|:------:|:-------------:|:-------------|
| **ASIA** | 8 | 8 | 18 | Medical diagnosis network relating travel, tuberculosis, and respiratory diseases. |
| **STUDENT** | 5 | 5 | 10 | Student performance network linking intelligence, grades, and recommendations. |
| **INSURANCE** | 27 | 52 | 1008 | Policy risk assessment model for insurance decisions. |
| **ALARM** | 37 | 46 | 509 | ICU patient monitoring model for early detection of emergencies. |
| **CHILD** | 20 | 25 | 230 | Pediatric diagnosis model used for reasoning and teaching. |

---

Expert-Elicited Networks

| Dataset | Experts | Ratings | Noise Levels σ | Description |
|:--|:--:|:--:|:--:|:--|
| **ASIA-Human** | 20 | 28 pairs × 20 experts | {0, 1, 2, 5, 10} | Human-elicited causal judgments on the Asia network. |
| **STUDENT-Survey** | 15 | 28 pairs | {0, 2, 5} | Student survey data capturing causal understanding between academic factors. |
| **HIP-FRACTURE** | 12 clinicians | 45 pairs | {0, 1, 2, 5} | Medical expert data on causal pathways in geriatric fracture outcomes. |

---

Example Usage

python
from bnbench import load_network, load_expert_data
from bnbench.metrics import evaluate_structure

# Load a canonical BN
asia = load_network("asia")
print("Nodes:", asia.nodes)
print("Edges:", asia.edges)

# Load expert-elicited pairwise data
ratings = load_expert_data("asia_human")
print(ratings.head())

# Evaluate predicted structure
score = evaluate_structure(predicted_dag, ground_truth=asia)
print(score)


