🔹 Milestone 2 – Interactive Multi-Tool Application using ipywidgets

Milestone 2 enhances the initial pipeline by creating a modular, interactive Jupyter application that integrates frontend interactivity with backend analytics. Built using ipywidgets, it delivers an intuitive, user-centric environment combining conversational AI, file utilities, visual analytics, and AI benchmarking.

**Core Modules**

Chatbot Interface – Simulates real-time conversations with intent recognition for Python and AI topics.

File Inspector – Enables secure uploads, metadata extraction, and live previews.

Interactive Data Plotter – Generates dynamic charts with user-controlled options.

AI Code Benchmarking Suite – Compares Hugging Face models (DeepSeek-Coder, Phi-2, Gemma) on code quality and performance metrics.

<img width="617" height="619" alt="Screenshot (135)" src="https://github.com/user-attachments/assets/5041c8ef-c3fc-497e-8f52-39292131f3bd" />


**Chatbot Interface (Detailed Overview)**

The Chatbot Interface serves as the conversational entry point of the Interactive Multi-Tool Application. Built entirely with ipywidgets, it provides a seamless and responsive dialogue experience inside the Jupyter environment.


Key Features

| Feature                   | Description                                                                                          |
| ------------------------- | ---------------------------------------------------------------------------------------------------- |
| **Real-Time Interaction** | Users can chat with the bot using a clean text area and intuitive “Send” and “Clear” buttons.        |
| **Typing Simulation**     | Displays a “Bot is typing…” animation to mimic real-time conversation flow.                          |
| **Intent Recognition**    | Detects keywords and phrases related to Python, AI, Machine Learning, and coding concepts.           |
| **Dynamic Responses**     | Generates context-aware replies about Python syntax, loops, data structures, and AI/ML fundamentals. |
| **Error Handling**        | Default responses guide the user to rephrase or explore supported topics.                            |
| **Scrollable History**    | The conversation area automatically updates without freezing, maintaining all previous messages.     |
| **Fully Styled Layout**   | Utilizes `VBox`, `HBox`, and `HTML` widgets for header, borders, color themes, and spacing.          |

**UI Design**

Header: A stylized title banner using HTML for a clean interface.

Chat Window: Scrollable Output widget to display user and bot messages with alternating background colors.

Input Bar: Combines a Textarea, “Send” button, and “Clear” button horizontally using HBox.

Layout Styling: Controlled through widgets.Layout properties for consistent sizing, padding, and borders.

**Backend Logic**

get_bot_reply() and get_bot_response() handle input processing and keyword-based reply generation.

Event handlers (on_send_button_clicked, on_clear_button_clicked) manage user actions and chat updates.

Built-in delay (time.sleep(1)) creates natural “typing” feedback for smoother interaction.

Example Queries

| User Input             | Bot Response                                                   |
| ---------------------- | -------------------------------------------------------------- |
| “Hello”                | “Hello there! How can I help you today?”                       |
| “Explain Python loops” | “Loops repeat actions. Example: `for i in range(5): print(i)`” |
| “Tell me about AI”     | “AI is the simulation of human intelligence by machines...”    |

<img width="1757" height="538" alt="Screenshot (134)" src="https://github.com/user-attachments/assets/0ac65836-b50f-44e4-ae53-782b7aad20f1" />


**Extensibility**

Can be integrated with real NLP or LLM APIs (OpenAI, Hugging Face) for intelligent conversation.

Supports adding new intents or command patterns for extended functionality.

**Methodology**

Environment Setup

| Library                           | Purpose                                    |
| --------------------------------- | ------------------------------------------ |
| ipywidgets                        | Interactive frontend components            |
| transformers, torch, bitsandbytes | AI/LLM inference                           |
| radon                             | Static code analysis (complexity, metrics) |
| seaborn, matplotlib               | Visualization and analytics tools          |


**Hugging Face Model Integration**

| Model               | Provider/Path                            | Use Case        |
| ------------------- | ---------------------------------------- | --------------- |
| DeepSeek-Coder 1.3B | deepseek-ai/deepseek-coder-1.3b-instruct | Code generation |
| Phi-2               | microsoft/phi-2                          | Code generation |
| Gemma 2B IT         | google/gemma-2b-it                       | Code generation |

<img width="1984" height="571" alt="image" src="https://github.com/user-attachments/assets/e6b78994-631f-44f5-8587-1e9b62315133" />


All models are authenticated and GPU-optimized for efficient inference.

**Backend Logic Functions**

| Function                       | Purpose                                     |
| ------------------------------ | ------------------------------------------- |
| `generate_code()`              | Produces Python code from natural prompts   |
| `calculate_advanced_metrics()` | Computes complexity, maintainability, LOC   |
| `clean_generated_code()`       | Removes formatting/artifacts from AI output |

Real-time dialogue simulation with “Bot is typing…” feedback.

Intent recognition for Python/AI queries.

Send and Clear buttons for easy interaction.

**File Inspector**

| Feature          | Description                                  |
| ---------------- | -------------------------------------------- |
| Upload support   | Handles multiple file types                  |
| Metadata display | Shows name, type, size                       |
| Text preview     | Displays up to 500 characters for text files |
| Binary handling  | Displays clear message for non-text files    |

Users select chart type (Bar, Line, Scatter) and data size via sliders.

Plots update instantly for visual exploration.

**AI Model Benchmarking Dashboard**

| UI Type             | Description                                                           |
| ------------------- | --------------------------------------------------------------------- |
| Run All Models      | Executes prompt on all models and shows summary                       |
| Run Selected Models | User selects models to benchmark & compare                            |
| Report Generator    | Aggregates metrics: Generation time, Complexity, Maintainability, LOC |

Sample Benchmark (Illustrative)

| Model    | Gen. Time (s) | Complexity | Maintainability | LOC |
| -------- | ------------- | ---------- | --------------- | --- |
| DeepSeek | 2.1           | 8          | 78              | 54  |
| Phi-2    | 2.3           | 7          | 75              | 51  |
| Gemma    | 1.9           | 9          | 73              | 56  |

<img width="1984" height="571" alt="image" src="https://github.com/user-attachments/assets/a693ea51-dbb8-4c39-aba3-e847e0ff361d" />


Insight: DeepSeek-Coder-1.3B offers the best balance of speed, maintainability, and complexity.

**Results & Insights**

Chatbot effectively simulates conversational interactions.

File Inspector accurately previews and summarizes uploads.

Plotter enables real-time, user-driven analytics.

Benchmark Suite offers valuable insights into model performance and code quality.

**Conclusion & Future Scope**

This milestone demonstrates how ipywidgets can unify interactive UI and analytical workflows within a single Jupyter environment—bridging intuitive design with analytical depth for real-world data science tasks.

**Future Enhancements:**

Integrate real-time LLM APIs for smarter conversational AI.

Add more advanced data visualization types and filtering options.

Extend the benchmarking suite with additional models and metrics.
