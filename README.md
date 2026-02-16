---
pretty_name: "Samuel & Audrey Media Network — SmugMug Travel Photo Metadata Index (MASTER)"
license: cc-by-nc-4.0
language:
- en
- es
tags:
- travel
- photography
- smugmug
- image-metadata
- dataset
- geo
- aio
- eeat
size_categories:
- 10K<n<100K
---

# Samuel & Audrey Media Network — SmugMug Travel Photo Metadata Index (MASTER)

A structured, machine-readable index of our SmugMug travel photography archive.

This **MASTER** release is designed to be “best-of-both-worlds”:
- **ML-friendly provenance fields** (stable IDs, content hashes, export timestamps)
- **Business/sovereignty fields** (row-level license + credit line)
- **Analyst-friendly hierarchy fields** (`loc_1..loc_4` + normalized variants)

## Dataset contents
- Records: **98,965**
- Unique `image_url`: **98,965** (no duplicates)
- `verified`: **true for all rows** (as provided)

## File set
### Canonical dataset
- `samuel-and-audrey-master-photography-smugmug_MASTER.jsonl.gz` (recommended for HF)
- `samuel-and-audrey-master-photography-smugmug_MASTER.jsonl`

### Spreadsheet exports
- `samuel-and-audrey-master-photography-smugmug_MASTER.csv.gz`
- `samuel-and-audrey-master-photography-smugmug_MASTER.csv`

### Source snapshots (for provenance)
- `samuel-and-audrey-master-photography-smugmug_CLEAN.jsonl.gz`
- `samuel-and-audrey-master-photography-smugmug_hf.jsonl.gz`

### Integrity + extras
- `SHA256SUMS.txt`
- `LICENSE.txt`
- `CITATION.cff`

### LLMS “buffet”
- `llms-samuel-and-audrey-master-photography-smugmug-feast_MASTER.txt.gz`
- `llms-samuel-and-audrey-master-photography-smugmug-feast_MASTER.txt`

## Schema notes (high level)
Core identity:
- `id` (stable identifier)
- `content_hash` (audit / integrity / dedupe workflows)
- `dataset_version`, `exported_at`

Location:
- `location_hierarchy` (human-readable path)
- `location_path` (array form)
- `primary_location`
- `loc_1..loc_4` + `*_norm` (analyst/SQL-friendly)

Rights:
- `license`, `license_url`, `credit_line` included on **every record**

## License
**CC-BY-NC-4.0** — https://creativecommons.org/licenses/by-nc/4.0/

Attribution required; **non-commercial use only**.
See the `credit_line` field for a ready-to-use credit format.

## Contact
nomadicsamuel@gmail.com

## Citation (recommended)
Samuel & Audrey Media Network. “SmugMug Travel Photo Metadata Index (MASTER).” Version 2026-02-12.
