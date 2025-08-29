# Results

This folder contains the **final outputs** of the evaluation process for **PromptForge**.  
While `/evaluation` stores the raw logs, this folder summarizes findings into human-readable reports, metrics, and visualizations.

## Files

- **evaluation_report.md**  
  A detailed written summary of model performance, strengths, weaknesses, and error analysis.

- **metrics_summary.csv**  
  Tabular performance metrics (accuracy, precision, recall, F1-score, etc.) computed from the evaluation data.

- **graphs.png**  
  Visual representation of key results (e.g., task-wise accuracy, response length distribution, or comparison across prompt styles).

## Purpose

- Provides a **clear snapshot** of how the model performs across tasks.  
- Helps compare runs over time by tracking metrics.  
- Facilitates communication of results with stakeholders or collaborators.

## Workflow

1. Raw logs are collected in `/evaluation`.  
2. Scripts aggregate and analyze the data.  
3. Final results are exported here as reports, tables, and graphs.  

---

📊 These outputs should always be regenerated if `/evaluation` logs are updated.
