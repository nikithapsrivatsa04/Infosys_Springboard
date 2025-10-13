🧩 Milestone 2 – Interactive Multi-Tool Application using ipywidgets
Executive Summary

This milestone extends the foundational concepts explored in Milestone 1 by developing a comprehensive, multi-functional interactive application in Python using ipywidgets.
The project demonstrates how to combine frontend interactivity with backend logic to build a polished, user-friendly environment that integrates multiple tools:

A Chatbot Interface simulating real-time conversational AI,

A File Inspector for handling and previewing user uploads, and

An Interactive Data Plotter for dynamic data visualization.

In addition, this notebook incorporates AI code benchmarking using multiple Hugging Face models such as DeepSeek-Coder, Phi-2, and Gemma, integrating metrics like Cyclomatic Complexity, Maintainability Index, and Lines of Code for comparative analysis.
Overall, Milestone 2 showcases both the interactive design capabilities of ipywidgets and the analytical depth of modern AI evaluation tools.

1. Methodology
1.1 Environment Setup

The project begins by installing essential libraries:

ipywidgets – for interactive UI elements,

transformers, torch, bitsandbytes – for AI model inference,

radon – for static code analysis,

seaborn & matplotlib – for visualization and analytics.
This ensures an integrated environment for developing, testing, and visualizing both AI and UI components.

1.2 Hugging Face Integration

Secure authentication is established via Hugging Face login, allowing access to gated models.
Predefined model configurations load and benchmark three LLMs:

deepseek-ai/deepseek-coder-1.3b-instruct

microsoft/phi-2

google/gemma-2b-it
Each model is preloaded onto the GPU for optimized inference performance.

1.3 Backend Computation Engine

Core functions include:

generate_code() – Generates Python code based on input prompts.

calculate_advanced_metrics() – Computes Cyclomatic Complexity, Maintainability Index, and Lines of Code using Radon.

clean_generated_code() – Sanitizes model output by removing unwanted text formatting.
Together, these components enable an automated, multi-model benchmarking system that evaluates both performance and code quality.

2. Interactive UI Components
   
2.1 Chatbot Interface

The Interactive Chat App forms the core of this milestone. Built using ipywidgets, it integrates:

A styled header and chat history display area.

A text input box, Send, and Clear buttons.

Simulated “Bot is typing…” feedback for realism.
The backend logic processes user input, identifies intent (e.g., greetings, programming questions), and generates appropriate responses using a rule-based system.

Key Highlights:

Dynamic message rendering within the notebook.

Support for queries about Python, AI, and coding syntax.

Clean UI layout using VBox, HBox, and HTML widgets.

2.2 File Inspector Tool

This tool allows users to upload and examine files directly from the notebook interface.
Features include:

Metadata extraction (file name, size, and type).

Real-time text preview (up to 500 characters).

Binary file handling with informative messages.

It demonstrates real-world file management, emphasizing UI responsiveness and versatility across file types.

2.3 Interactive Data Plotter

This module integrates matplotlib and ipywidgets to create interactive visualizations.
Users can select:

Plot type: Bar, Line, or Scatter.

Number of data points via a slider.
The backend generates random data dynamically and renders the chosen visualization instantly, offering an intuitive way to explore data representation concepts.

3. Multi-Model Benchmarking Dashboard

Two UIs are implemented for benchmarking:

UI #1 – Run All Models:
Executes the same prompt across all preloaded models and displays a performance summary.

UI #2 – Run Selected Models:
Provides model-specific control via checkboxes for customized benchmarking.

A final Report Generator aggregates results from all sessions, visualizing key metrics through bar charts (Generation Time, Complexity, Maintainability) using Seaborn.

4. Implementation Workflow
Step	Module	Description
1	Setup	Install and import all libraries
2	Login	Authenticate with Hugging Face
3	Backend	Define helper and metric functions
4	Load Models	Preload all selected models
5	UI #1	Benchmark across all models
6	UI #2	Run tests on selected models
7	Report	Generate visual analytics
8	Cleanup	Free GPU memory manually
5. Results & Observations

The Chatbot App successfully mimics conversational flow with a smooth and responsive interface.

The File Inspector accurately retrieves file details and previews textual content.

The Data Plotter provides flexible, real-time plotting for varied datasets.

The AI Benchmark Suite performs efficient, multi-model evaluations, generating quantifiable code metrics and comparative visual reports.

Overall, the project demonstrates a seamless blend of interactivity, analytics, and AI-driven insights.

6. Conclusion & Future Scope

This milestone solidifies practical expertise in creating multi-tab, modular applications using ipywidgets while incorporating AI benchmarking workflows.
It bridges the gap between user interface design and intelligent backend computation, exemplifying the power of interactive notebooks for real-world applications.

Future Enhancements:

Integrate LLM-based conversational models (e.g., GPT, LLaMA) for a smarter chatbot.

Extend data plotting with file-based CSV inputs.

Add a user session manager to log interaction history.

Deploy as a Streamlit or Gradio web app for accessibility beyond Jupyter.
