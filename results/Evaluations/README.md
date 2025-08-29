# Evaluation

This folder contains raw evaluation data generated during the testing of **PromptForge**.  
Each file captures prompts, responses, tasks, and timestamps for different evaluation runs.

## Files

- **evaluation_data.jsonl**  
  Raw logs of model interactions with simple QA and summarization prompts.

- **prompt_eval_data.jsonl**  
  Logs of evaluations with predefined prompt templates (e.g., roleplay, structured QA, summarization).

## File Format

- Files use **JSON Lines (.jsonl)** format.  
- Each line represents one evaluation record with fields such as:
  - `timestamp` → when the interaction occurred  
  - `task` → type of task (`qa`, `summarization`, `roleplay`, etc.)  
  - `prompt` → input provided to the model  
  - `response` → model’s output  

## Purpose

- Serves as the **ground truth data source** for generating reports in the `reports/` folder.  
- Enables reproducibility and transparency by keeping all raw logs intact.  
- Provides data for custom metrics or future re-analysis.

---

📌 These logs are not edited. Reports in `/reports` are generated from this data.
