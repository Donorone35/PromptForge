## **Prompt-Forage**

This repository contains an **LLM-powered framework** for **prompt engineering, multi-task evaluation, and automated report generation**.  
It leverages **IBM Granite LLM** via **WatsonX.ai** and **LangChain** to handle tasks like **question answering, summarization, classification, roleplay, and code generation** with reproducible evaluation and visualization support.

## **Key Features**
- **Multi-Task LLM:** Supports QA, summarization, roleplay, classification, and code generation.
- **Granite LLM Integration:** Uses `ibm/granite-3-2-8b-instruct` from WatsonX.ai.
- **Parameter Tuning:** Control `temperature`, `top_p`, `top_k`, `max_new_tokens`, and more per task.
- **LangChain Orchestration:** Modular prompts, chains, and templates for structured LLM interactions.
- **Structured Logging:** JSONL logs of every request with timestamp and metadata.
- **Automated Reports:** Markdown, CSV summaries, and visualization charts for evaluation.
- **Task-Specific Defaults:** Presets optimized for decoding strategies per task (greedy vs sampling).

## **Technology Used**
### **Languages & Libraries**
- **Python 3.10+**
- **LangChain** (templates, chains, parsing)
- **ibm_watsonx_ai** (Granite LLM API)
- **Pandas & CSV** (data handling)
- **Matplotlib** (visualizations)
- **JSON / JSONL** (logging & reporting)

### **Model & Parameters**
- **Model:** `ibm/granite-3-2-8b-instruct`
- **Provider:** IBM WatsonX.ai
- **Task Presets:**  
  - QA: sample decoding, max 256 tokens, temperature 0.4  
  - Summarization: sample decoding, max 200 tokens, temperature 0.3  
  - Classification: greedy decoding, max 50 tokens, temperature 0.2  
  - Code: sample decoding, max 300 tokens, temperature 0.3, top_k 20  
  - Roleplay: sample decoding, max 256 tokens, temperature 0.8, top_p 0.9

## **Project Structure**
```
Prompt-Forage/
│── prompts/ # Task-specific prompt templates
│── results/ # Stores output files
│ │── Evaluations/ # JSONL / CSV evaluation data
│ │ │── prompt_evaluation_responses.jsonl # Structured evaluation responses
│ │ │── llm_raw_responses.jsonl # Raw LLM outputs
│ │── Reports/ # Markdown summaries and visualizations
│ │ │── metrics_summary.csv # CSV summary of metrics
│ │ │── graphs.png # Visualizations of results
│ │ │── evaluation_report.md # Markdown report
│ │── README.md # Result folder documentation
│── PromptForge.ipynb # Main Jupyter notebook with code
│── requirements.txt # Python dependencies
│── README.md # Project documentation
│── LICENSE # MIT License
```

## **Installation & Usage**
### **Installation**
1. **Clone the Repository**
   ```bash
   git clone https://github.com/Donorone35/Prompt-Forage.git
   cd Prompt-Forage

## **Contact**
- **Author:** Trayambak Rai
- **GitHub:** [Donorone35](https://github.com/Donorone35)
- **LinkedIn:** [Trayambak Rai](https://www.linkedin.com/in/trayambak-rai-314606278/)
