
🔹 Milestone 2 – Interactive Multi-Tool Application using ipywidgets

Executive Summary

Milestone 2 enhances the initial pipeline by creating a modular, interactive Jupyter application that integrates frontend interactivity with backend analytics. Built using ipywidgets, it delivers an intuitive, user-centric environment combining conversational AI, file utilities, visual analytics, and AI benchmarking.

Core Modules:

Chatbot Interface: Simulates real-time conversations with intent recognition for Python and AI topics.

File Inspector: Enables secure uploads, metadata extraction, and live previews.

Interactive Data Plotter: Generates dynamic charts with user-controlled options.

AI Code Benchmarking Suite: Compares Hugging Face models (DeepSeek-Coder, Phi-2, Gemma) on code quality and performance metrics.

**Methodology**

Environment Setup:

| Library                           | Purpose                                    |
| --------------------------------- | ------------------------------------------ |
| ipywidgets                        | Interactive frontend components            |
| transformers, torch, bitsandbytes | AI/LLM inference                           |
| radon                             | Static code analysis (complexity, metrics) |
| seaborn, matplotlib               | Visualization and analytics tools          |


Hugging Face Model Integration:

| Model               | Provider/Path                            | Use Case        |
| ------------------- | ---------------------------------------- | --------------- |
| DeepSeek-Coder 1.3B | deepseek-ai/deepseek-coder-1.3b-instruct | Code generation |
| Phi-2               | microsoft/phi-2                          | Code generation |
| Gemma 2B IT         | google/gemma-2b-it                       | Code generation |


All models are authenticated and GPU-optimized for efficient inference.

Backend Logic

| Function                       | Purpose                                     |
| ------------------------------ | ------------------------------------------- |
| `generate_code()`              | Produces Python code from natural prompts   |
| `calculate_advanced_metrics()` | Computes complexity, maintainability, LOC   |
| `clean_generated_code()`       | Removes formatting/artifacts from AI output |


**Interactive UI Features**

1. Chatbot Interface:
   
Real-time dialogue simulation with “Bot is typing…” feedback.

Intent recognition for Python/AI queries.

Send and Clear buttons for easy interaction.

2. File Inspector:
   
Displays file metadata, previews text up to 500 characters, and handles non-text binaries gracefully.

| Feature          | Description                                  |
| ---------------- | -------------------------------------------- |
| Upload support   | Handles multiple file types                  |
| Metadata display | Shows name, type, size                       |
| Text preview     | Displays up to 500 characters for text files |
| Binary handling  | Displays clear message for non-text files    |


3. Interactive Data Plotter:
   
Users select chart type (Bar, Line, Scatter) and data size via sliders; plots update instantly for visual exploration.

4. Model Benchmarking Dashboard:
   
| UI Type             | Description                                                           |
| ------------------- | --------------------------------------------------------------------- |
| Run All Models      | Executes prompt on all models, shows summary                          |
| Run Selected Models | User selects models to benchmark & compare                            |
| Report Generator    | Aggregates metrics: Generation time, Complexity, Maintainability, LOC |


Sample Benchmark (Illustrative):
| Model    | Gen. Time (s) | Complexity | Maintainability | LOC |
| -------- | ------------- | ---------- | --------------- | --- |
| DeepSeek | 2.1           | 8          | 78              | 54  |
| Phi-2    | 2.3           | 7          | 75              | 51  |
| Gemma    | 1.9           | 9          | 73              | 56  |

5. Hugging Face Model Comparison and Best Model Selection

This project includes a benchmarking module that compares multiple Hugging Face models—DeepSeek-Coder-1.3B, Phi-2-2.7B, and Gemma-2B-IT—on code generation tasks. Key performance metrics evaluated are:

| Metric                    | Description                                             |
| ------------------------- | ------------------------------------------------------- |
| **Generation Time (s)**   | Time taken by the model to generate code from a prompt. |
| **Cyclomatic Complexity** | Measures code complexity; lower is simpler.             |
| **Maintainability Index** | Indicates ease of maintenance; higher is better.        |
| **Lines of Code (LOC)**   | Number of lines generated.                              |


A visual dashboard presents these metrics using interactive bar plots for easy comparison. Based on the analysis, DeepSeek-Coder-1.3B emerges as the best-performing model across key metrics, offering a balance of speed, maintainability, and complexity.

**Results & Insights**

The Chatbot effectively simulates conversational interactions.

The File Inspector accurately previews and summarizes uploads.

The Plotter enables real-time, user-driven analytics.

The Benchmark Suite offers valuable insights into model performance and code quality.

**Conclusion & Future Scope**

This milestone demonstrates how ipywidgets can unify interactive UI and analytical workflows within a single Jupyter environment—bridging intuitive design with analytical depth for real-world data science tasks.
