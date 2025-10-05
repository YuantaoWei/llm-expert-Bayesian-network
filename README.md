📚 Bayesian Network Library

A curated library of Bayesian Networks (BNs) for research and education.  
This repository collects well-known benchmark networks and datasets, making it easier to evaluate **causal discovery, parameter learning, and inference algorithms**.

---

Classic Discrete Bayesian Networks

Small Networks (<20 nodes)

| Name | Nodes | Arcs | Parameters | Description |
|------|-------:|------:|------------:|-------------|
| [ASIA](networks/asia.json) | 8 | 8 | 18 | A small medical diagnosis network relating travel and respiratory diseases. |
| [CANCER](networks/cancer.json) | 5 | 4 | 10 | Simple cancer diagnostic model showing probabilistic influence of tests and disease. |
| [EARTHQUAKE](networks/earthquake.json) | 5 | 4 | 10 | Classic alarm example modeling earthquake and burglary events. |
| [SACHS](networks/sachs.json) | 11 | 17 | 178 | Protein-signaling network from Sachs et al. (2005). |
| [SURVEY](networks/survey.json) | 6 | 6 | 21 | Illustrative model for opinion polling with latent factors. |

---

Medium Networks (20–50 nodes)

| Name | Nodes | Arcs | Parameters | Description |
|------|-------:|------:|------------:|-------------|
| [ALARM](networks/alarm.json) | 37 | 46 | 509 | An ICU patient monitoring model for early detection of emergencies. |
| [BARLEY](networks/barley.json) | 48 | 84 | 114005 | Agricultural yield prediction network based on environmental variables. |
| [CHILD](networks/child.json) | 20 | 25 | 230 | Pediatric diagnosis network used for teaching medical reasoning. |
| [INSURANCE](networks/insurance.json) | 27 | 52 | 1008 | Insurance risk assessment model for policy decisions. |
| [MILDEW](networks/mildew.json) | 35 | 46 | 540150 | Crop disease network modeling mildew propagation under humidity. |
| [WATER](networks/water.json) | 32 | 66 | 10083 | Water treatment plant control model for fault diagnosis. |

---

Large Networks (50–100 nodes)

| Name | Nodes | Arcs | Parameters | Description |
|------|-------:|------:|------------:|-------------|
| [HAILFINDER](networks/hailfinder.json) | 56 | 66 | 2656 | Weather forecasting network for hail prediction. |
| [HEPAR2](networks/hepar2.json) | 70 | 123 | 1453 | Expert-designed medical BN for liver disorder diagnosis. |
| [WIN95PTS](networks/win95pts.json) | 76 | 112 | 574 | Windows 95 printer troubleshooting network. |

---

Very Large Networks (100–1000 nodes)

| Name | Nodes | Arcs | Parameters | Description |
|------|-------:|------:|------------:|-------------|
| [ANDES](networks/andes.json) | 223 | 338 | 1157 | Intelligent tutoring system modeling student knowledge in physics. |
| [DIABETES](networks/diabetes.json) | 413 | 602 | 429409 | Diabetes patient health progression model from clinical data. |
| [LINK](networks/link.json) | 724 | 1125 | 14211 | Telecommunication reliability and link-failure model. |
| [MUNIN (subnetwork #1)](networks/munin1.json) | 186 | 273 | 15622 | Medical diagnosis subnetwork from the MUNIN expert system. |
| [PATHFINDER](networks/pathfinder.json) | 109 | 195 | 72079 | Expert pathology BN for lymph node disease classification. |
| [PIGS](networks/pigs.json) | 441 | 592 | 5618 | Economic model for swine production management. |

---

Massive Networks (>1000 nodes)

| Name | Nodes | Arcs | Parameters | Description |
|------|-------:|------:|------------:|-------------|
| [MUNIN (full network)](networks/munin_full.json) | 1041 | 1397 | 80592 | Complete MUNIN expert system for neuromuscular diagnosis. |
| [MUNIN (subnetwork #2)](networks/munin2.json) | 1003 | 1244 | 69431 | Subnetwork derived from the full MUNIN medical expert system. |
| [MUNIN (subnetwork #3)](networks/munin3.json) | 1041 | 1306 | 71059 | Alternative diagnostic module of the MUNIN network. |
| [MUNIN (subnetwork #4)](networks/munin4.json) | 1038 | 1388 | 80352 | Fourth subnetwork for hierarchical medical reasoning. |

---

Gaussian Bayesian Networks

Medium Networks (20–50 nodes)

| Name | Nodes | Arcs | Parameters | Description |
|------|-------:|------:|------------:|-------------|
| [ECOLI70](networks/ecoli70.json) | 46 | 70 | 162 | Gene expression regulatory model for E. coli under stress. |
| [MAGIC-NIAB](networks/magic_niab.json) | 44 | 66 | 154 | Crop genetic trait network from NIAB MAGIC population data. |

Large Networks (50–100 nodes)

| Name | Nodes | Arcs | Parameters | Description |
|------|-------:|------:|------------:|-------------|
| [MAGIC-IRRI](networks/magic_irri.json) | 64 | 102 | 230 | Rice yield and environmental factor network from IRRI datasets. |

Very Large Networks (101–1000 nodes)

| Name | Nodes | Arcs | Parameters | Description |
|------|-------:|------:|------------:|-------------|
| [ARTH150](networks/arth150.json) | 107 | 150 | 364 | Arthritis-related gene and symptom interaction model. |

---

Conditional Linear Gaussian Bayesian Networks

Small Networks (<20 nodes)

| Name | Nodes | Arcs | Parameters | Description |
|------|-------:|------:|------------:|-------------|
| [HEALTHCARE](networks/healthcare.json) | 7 | 9 | 42 | Healthcare process simulation network linking quality and cost. |
| [SANGIOVESE](networks/sangiovese.json) | 15 | 55 | 259 | Winemaking quality model based on Sangiovese fermentation data. |

Medium Networks (20–50 nodes)

| Name | Nodes | Arcs | Parameters | Description |
|------|-------:|------:|------------:|-------------|
| [MEHRA](networks/mehra.json) | 24 | 71 | 324423 | CLG network describing sensor-driven industrial process control. |

---

Repository Structure


