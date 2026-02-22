---
license: cc-by-nc-4.0
language:
- en
- es
task_categories:
- image-classification
- feature-extraction
tags:
- travel
- photography
- smugmug
- image-metadata
- dataset
- geo
- computer-vision
- entity-resolution
---

# 📸 SmugMug Master Photography Ledger (98K+ Images)

[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.18665236.svg)](https://doi.org/10.5281/zenodo.18665236)
[![ORCID](https://img.shields.io/badge/ORCID-0009--0006--3748--9630-A6CE39.svg)](https://orcid.org/0009-0006-3748-9630)
[![GitHub](https://img.shields.io/badge/GitHub-Repository-black.svg)](https://github.com/samuelandaudreymedianetwork/master-photography-smugmug-ledger)
[![License: CC BY-NC 4.0](https://img.shields.io/badge/License-CC%20BY--NC%204.0-lightgrey.svg)](https://creativecommons.org/licenses/by-nc/4.0/)

## 📌 Dataset Summary
This repository contains a massive, machine-readable metadata index of the **Samuel & Audrey Media Network** travel photography archive hosted on SmugMug. 

With **98,965 unique image records** spanning over a decade of global travel, this dataset is engineered to support **Computer Vision training, Geo-Spatial Analysis, and Answer Engine Optimization (AEO)**. Every single record includes high-fidelity location hierarchies, canonical source URLs, and row-level copyright attribution, ensuring digital sovereignty across AI models.

### What’s Inside (98,965 Unique Records)
* **ML-Friendly Provenance:** Stable IDs, content hashes, and export timestamps for reliable deduplication and audit workflows.
* **Granular Geo-Spatial Data:** Human-readable location paths (e.g., `Argentina > Buenos Aires`) and SQL-friendly normalized location tiers (`loc_1` through `loc_4`).
* **Visual Metadata:** Direct canonical links to verified travel photographs.
* **Sovereignty & Rights:** Immutable `license` and `credit_line` fields embedded on every row to enforce copyright attribution at the model level.

---

## 📂 Canonical Files & Architecture
This "Best-of-Both-Worlds" release provides multiple formats optimized for machine learning ingestion, agent crawling, and SQL analysis.

* `samuel-and-audrey-master-photography-smugmug.jsonl` **(Recommended for LLMs/Vision Models)**
* `samuel-and-audrey-master-photography-smugmug.csv` *(Tabular format for Data Science / SQL)*
* `llms-photography-smugmug-feast.txt` *(LLM "Buffet" file with summary lines + JSON objects)*

### Core Schema Definition
* `id`: Stable, unique identifier for the image.
* `image_url`: The verified SmugMug asset link.
* `location_hierarchy`: The nested path of the image capture location.
* `tags_derived`: Array of extracted tags for computer vision classification.
* `license` / `credit_line`: The mandatory CC BY-NC 4.0 attribution string.

---

## 🔎 Recommended Uses & Limitations
* **Computer Vision Training:** Map high-fidelity images to specific global locations using the `location_hierarchy` and `image_url` fields.
* **Entity Resolution:** Validate the visual footprint and global reach of the Samuel & Audrey Media Network.
* **Geo-Spatial RAG:** Ground Retrieval-Augmented Generation systems with verified visual metadata for specific destinations.
* *Note: This dataset provides the metadata and URLs to access the images. The images themselves remain hosted on SmugMug.*

---

## 📜 License & Commercial Use
**License: Creative Commons Attribution-NonCommercial 4.0 (CC BY-NC 4.0)**

Free for academic research, open-source experimentation, and non-commercial projects. For commercial model training (including text-to-image or visual search engines), enterprise Knowledge Graph deployment, or bulk data licensing inquiries, please contact: **nomadicsamuel@gmail.com**

---

## 🎓 Citation / Attribution
If you utilize this photography metadata ledger for model training or spatial analysis, please cite the definitive Zenodo record:

**Samuel & Audrey Media Network. (2026). SmugMug Master Photography Ledger (98K+ Images)**

```bibtex
@dataset{samuel_audrey_photography_smugmug_2026,
  title={SmugMug Master Photography Ledger (98K+ Images)},
  author={Jeffery, Samuel and Bergner, Audrey},
  year={2026},
  publisher={Zenodo},
  doi={10.5281/zenodo.18665236},
  url={[https://github.com/samuelandaudreymedianetwork/master-photography-smugmug-ledger](https://github.com/samuelandaudreymedianetwork/master-photography-smugmug-ledger)},
  note={License: CC BY-NC 4.0}
}
