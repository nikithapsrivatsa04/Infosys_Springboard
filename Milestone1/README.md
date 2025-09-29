# Milestone 1 - Infosys Springboard Project

## 📌 Objective
The goal of Milestone 1 is to build a **Code Explainer Pipeline** that can analyze Python programs by combining:
- Transformer-based embeddings
- Abstract Syntax Tree (AST) parsing
- Visualization approaches  

This pipeline provides structural and semantic understanding of Python code snippets.

---

## 🛠️ Methodology

1. **Data Preparation**
   - Created 10 Python code samples demonstrating various programming constructs:
     - Imports
     - Loops
     - Recursion
     - Functions
     - Classes
     - File I/O
     - Exception Handling
     - etc.

2. **AST Parsing**
   - Used Python's `ast` library to extract:
     - Functions
     - Classes
     - Imports
   - Helps identify structure and flow of code.

3. **Transformer-based Embeddings**
   - Used pretrained embeddings (e.g., from HuggingFace models) to generate semantic vector representations of code snippets.
   - Enables natural language explanations.

4. **Visualization**
   - Generated flow representations and summaries.
   - Illustrated the code structure for better interpretability.

5. **Notebook Implementation**
   - Final implementation is in `milestone1_final.ipynb`.

---

## 📊 Observations
- **AST parsing** was effective for structural elements but lacked semantic richness.
- **Embeddings** helped in generating human-like explanations.
- Combining both approaches provided a **balanced understanding** of code.
- Visualization made explanations more intuitive.

---

## 📂 Folder Structure
