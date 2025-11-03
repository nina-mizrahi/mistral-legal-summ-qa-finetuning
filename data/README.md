# Data Overview

This folder documents the datasets used for fine-tuning **Mistral-7B** on legal summarization and question answering.

---

### CaseSumm (ChicagoHAI/CaseSumm)
- **Source:** [Hugging Face Dataset](https://huggingface.co/datasets/ChicagoHAI/CaseSumm)
- **Task:** Legal summarization  
- **Description:** Contains U.S. Supreme Court opinions and concise human-written summaries.  
- **License:** CC-BY-4.0 — requires attribution.  
- **Load:**
  ```python
  from datasets import load_dataset
  ds_sum = load_dataset("ChicagoHAI/CaseSumm")
---

### CaseHOLD (LexGLUE subset)
- **Source:** [Hugging Face Dataset]((https://huggingface.co/lex_glue/datasets))
- **Task:** Legal question answering
- **Description:** Multiple-choice questions derived from U.S. legal opinions.  
- **License:** CC-BY-NC-SA-4.0 — research only.
- **Load:**
  ```python
  from datasets import load_dataset
  ds_qa = load_dataset("lex_glue", "case_hold")
