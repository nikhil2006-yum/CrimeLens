# CrimeLens Architecture

## Workflow

```text
User Query
      │
      ▼
Question Classifier
      │
      ▼
Knowledge Retrieval
      │
      ▼
Variable Aggregator
      │
      ▼
Gemini LLM
      │
      ▼
Answer
```

## Components

### Question Classifier

Identifies the intent of the police officer.

Possible Categories

- Crime Database
- Crime Laws
- Police SOP
- Crime Intelligence

---

### Knowledge Retrieval

Retrieves relevant documents from the selected knowledge base using Hybrid Search.

---

### Variable Aggregator

Aggregates retrieved information before passing it to the LLM.

---

### Gemini

Generates accurate responses using retrieved context only.

---

### Output

Displays a concise answer to the officer.
