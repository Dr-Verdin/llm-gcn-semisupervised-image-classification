# Project Setup

## Prerequisites

- Python 3.10+
- Git
- 7-Zip (or p7zip)

### Ubuntu/Debian

```bash
sudo apt update
sudo apt install p7zip-full
```

### macOS

```bash
brew install p7zip
```

### Windows

Download and install from:
https://www.7-zip.org/


---

## Installation

```bash
git clone https://github.com/<username>/llm-gcn-semisupervised-image-classification.git
cd llm-gcn-semisupervised-image-classification
```

## Optional but recommended) Create virtual environment

```bash
python -m venv .venv
```

Activate it:

# Linux / macOS
source .venv/bin/activate

# Windows
.venv\Scripts\activate

## Install dependencies

```bash
pip install -r requirements.txt
```

```markdown
## Reproducibility

This repository was used to generate the results reported in the paper.  
All experiments assume the dataset is downloaded from Zenodo and placed in the `data/` directory.
```