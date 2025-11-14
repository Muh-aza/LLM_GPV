# 📁 Project Structure

This document provides a detailed overview of the file and folder organization for the LLM-GPV repository.

---

```text
LLM_GPV/
│
├── app.py                        # Main application entrypoint
├── requirements.txt              # Python dependencies
├── environment.yml               # Conda environment file (optional)
│
├── gpv/                          # Genetic Prompt Vision (core library)
│   ├── __init__.py
│   ├── optimizer.py
│   ├── selection.py
│   ├── mutation.py
│   ├── crossover.py
│   ├── population.py
│   └── utils.py
│
├── models/                       # Multimodal LLMs & inference wrappers
│   ├── __init__.py
│   ├── llama3.py
│   ├── gpt4ov.py
│   ├── gemini.py
│   ├── claude.py
│   ├── ensemble.py               # Optional: model ensembling
│   └── configs/
│        ├── model_config.yaml
│        └── prompts/
│             ├── prompt_template_1.txt
│             └── prompt_template_2.txt
│
├── scripts/                      # Data, evaluation, automation scripts
│   ├── download_data.py
│   ├── run_benchmark.py
│   ├── export_results.py
│   └── evaluate_performance.py
│
├── data/
│   ├── raw/                      # Unprocessed source data
│   ├── processed/                # Cleaned, ready-to-use data
│   ├── annotations.csv
│   └── sample_images/
│        ├── pathway1.png
│        └── pathway2.jpg
│
├── Results/
│   ├── figures/
│   │    ├── Fig-1.jpg
│   │    └── workflow.png
│   ├── metrics/
│   │    ├── evaluation.csv
│   │    └── summary.json
│   ├── demo.gif
│   └── logs/
│        └── run_2024-05-23.log
│
├── notebooks/                    # Jupyter notebooks for exploration/reports
│   ├── demo_analysis.ipynb
│   ├── pathway_experiments.ipynb
│   └── figures_overview.ipynb
│
├── static/                       # Frontend static assets (css/js)
│   ├── style.css
│   └── script.js
│
├── templates/                    # Web app HTML templates
│   └── index.html
│
├── configs/                      # Global YAML/JSON configs, secrets, parameters
│   ├── default.yaml
│   ├── secrets.env
│   └── logging.conf
│
├── tests/                        # Automated tests
│   ├── __init__.py
│   ├── test_gpv.py
│   ├── test_models.py
│   └── test_utils.py
│
├── docs/                         # Project documentation for contributors/users
│   ├── index.md
│   ├── usage.md
│   ├── api_reference.md
│   └── architecture.md
│
├── .github/                      # GitHub workflows for CI/CD
│   ├── workflows/
│   │    └── python-app.yml
│   └── ISSUE_TEMPLATE/
│        └── bug_report.md
│
├── docker/                       # Docker build and environment files (optional)
│   ├── Dockerfile
│   └── docker-compose.yml
│
├── assets/                       # Project images, icons, branding
│   └── logo.png
│
├── LICENSE
├── README.md
├── .gitignore
├── .env.example
└── setup.py                      # For pip install as a package
