# myinvois-sdk-llm

This repository contains a **knowledge package** extracted from the MyInvois SDK documentation (`https://sdk.myinvois.hasil.gov.my/`) in a format suitable for **LLM ingestion**.

---

## Folder Structure

knowledge_package/
├─ markdown/ # Individual Markdown files per page
├─ apis/ # Detected OpenAPI/Swagger JSON/YAML files
├─ combined_markdown.md # All pages concatenated
├─ summary.md # Short extracts per page
├─ chunks.jsonl # LLM embedding-ready chunks (JSONL)
├─ api_summaries.md # List of discovered API files
└─ metadata.json # Page metadata (URL, MD5 hash, updated)

---

## Usage

1. **Browse the Markdown**  
   Each file in `markdown/` corresponds to a page in the MyInvois SDK documentation.

2. **LLM ingestion**

    - Use `chunks.jsonl` to generate embeddings for vector search.
    - `combined_markdown.md` can be used directly for context or QA tasks.
    - `summary.md` provides short summaries for quick reference.

3. **API schemas**
    - Stored in `apis/`.
    - `api_summaries.md` lists each detected API schema along with its source URL.
