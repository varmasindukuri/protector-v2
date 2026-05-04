## Purpose
Runs all 14 agents from NB1-NB3 on your local machine in real time.
No FastAPI. Pure Jupyter + standalone tray.py.

## Features
- 14-agent multi-model fusion with weighted majority vote
- Attack family classification (BruteForce/DoS/Malware/WebAttack)
- SHAP explainability per live prediction
- NetworkX process topology graph
- Vulnerability assessment (open ports, suspicious processes)
- Static file analysis (PE headers, entropy, YARA, hash lookup)
- Groq LLM Q&A with live system context
- System tray - runs 24/7 without Jupyter open
- Email alerts for CRITICAL events

## Setup
1. Download all models from NB1, NB2, NB3, NB5 Kaggle outputs
2. Place in newml/ml/, newml/dl/, newml/advanced/ folders
3. Run merge_models() cell
4. Edit .env with your GROQ_KEY and EMAIL
5. Run Cell 9 to launch tray

   ## Tray Menu
Right-click diamond icon:
- Full Dashboard - all charts popup
- Process Graphs - NetworkX topology
- Show Status - agent verdicts
- VA Scan - open ports and suspicious procs
- Scan File - PE/hash/YARA analysis
- Ask AI (Groq) - natural language Q&A
- Quit
