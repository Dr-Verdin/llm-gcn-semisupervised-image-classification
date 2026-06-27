# Project Overview

This repository implements a multimodal pipeline that combines:

- Visual feature extraction (ResNet, DINOv2, ViT)
- Image captioning (BLIP)
- Ranking-based fusion of visual and textual representations
- Structured dataset generation for downstream evaluation

The pipeline is fully modular and allows swapping visual encoders without modifying downstream components.

## Pipeline

1. Image dataset loading (Corel5K)
2. Visual encoding (ResNet / DINOv2 / ViT)
3. Ranking generation
4. Caption generation (BLIP)
5. Ranking + caption fusion
6. Structured dataset creation for evaluation

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

## (Optional but recommended) Create virtual environment

```bash
python -m venv .venv
```

Activate it:

### Linux / macOS

```bash
source .venv/bin/activate
```

### Windows

```bash
.venv\Scripts\activate
```

## Install dependencies

```bash
pip install -r requirements.txt
```

## Reproducibility

To reproduce the experiments:

1. Install dependencies
2. Download datasets from Zenodo
3. Place files in `data/`
4. Run notebooks in order:

   - 01_generate_blip_captions.ipynb
   - 02_preprocess_and_consolidate_outputs.ipynb