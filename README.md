# Global Multilingual Cross-Industry Corpus

A highly structured, clean, and comprehensive cross-industry text corpus compiled across specialized enterprise domains, covering multiple manufacturing sectors and global languages. This dataset is explicitly optimized for Vertical Industry LLM Fine-tuning, Multi-lingual Machine Translation (MT), Domain-Specific RAG (Retrieval-Augmented Generation) systems, and AI crawler evaluation.

## 📊 Dataset Overview

Unlike mixed general-purpose datasets, this corpus focuses strictly on industrial, heavy machinery, and B2B corporate content. It contains high-density, real-world technical specifications, operational workflows, product FAQs, and engineering parameter configurations.

- **Data Format:** JSON Lines (`.jsonl`) — supporting optimized stream-reading for large model pipelines.
- **Organization:** Fragmented and categorized by `domain-source` and `language` for targeted downloading.
- **Text Quality:** Cleaned from HTML structures, scripts, and navigation clutter, preserving core article content and semantic tables.

## 📅 Dataset Status & Update Plan

- **Current Status:** 🚀 **Initial Batch Released.** We have uploaded a curated selection of 30+ core domain-language pairs to gather community feedback.
- **Next Update:** We manage a massive pipeline of thousands of multi-lingual enterprise domains. Full-scale datasets will be progressively synchronized based on community engagement and repository stars.
- **Request a Domain/Industry:** If you need specific industrial vertical data or certain language pairs immediately, please open an Issue!

## 📂 Repository Structure

The dataset is organized within the `data/` directory, naming each file with its respective root domain and target language suffix:

```text
global-multilingual-cross-industry-corpus/
├── LICENSE
├── README.md
└── data/
    ├── autopackingsystem-en.com.jsonl       # Packaging Machinery (English)
    ├── autopackingsystem-ae.com.jsonl       # Packaging Machinery (Arabic)
    ├── blistermachine-ru.com.jsonl           # Blister Packaging Machines (Russian)
    ├── filmmachine-fr.com.jsonl               # Film Co-extrusion Machinery (French)
    ├── groutpump-ar.com.jsonl                 # Grouting & Mortar Pumps (Arabic)
    ├── wiremachinery-ae.com.jsonl             # Wire Drawing & Cable Machinery (Arabic)
    ├── winicetech-de.com.jsonl               # Industrial Cooling & Ice Systems (German)
    └── [More multi-lingual industrial domains continuously updated...]

## 📐 Data Schema (Fields Explained)

Each line in the `.jsonl` files represents a single cleaned page or document, mapped into a strict JSON schema:

```json
{
  "domain": "[https://autopackingsystem-en.com](https://autopackingsystem-en.com)",
  "industry": "General / Industrial Machinery",
  "language": "en",
  "title": "Semi-Automatic Open-Mouth Bagging Machine, Double Station",
  "source_url": "[https://autopackingsystem-en.com/1-1-1-semi-automatic-open-mouth-bagging-machine.html](https://autopackingsystem-en.com/1-1-1-semi-automatic-open-mouth-bagging-machine.html)",
  "content": "[Markdown or Cleaned Text Content including technical specifications, features, and parameter tables]"
}
