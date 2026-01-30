# GED Science Prep

## Overview

This repository contains the complete GED Science Prep curriculum, organized into 12 chapters and aligned with the official GED Science Assessment Targets. Content addresses all 200 concepts across Life Science, Physical Science, and Earth & Space Science, and follows the eight required Science Practices.

## Course Structure

- **12 Chapters** systematically covering all 200 assessment targets
- **Learning Graph** illustrating concept dependencies and taxonomy
- **Interactive MicroSims** for hands-on, visual learning
- **Assessment Guide** reference materials for educators and learners

## Content Domains

- **Life Science (40%)**: Human body systems, energy flow, cellular organization, genetics, heredity, and evolution
- **Physical Science (40%)**: Conservation of energy, work and motion, chemical properties and reactions
- **Earth and Space Science (20%)**: Earth systems, atmospheric and oceanic processes, cosmic structures

## Science Practices

The curriculum is organized around these eight Science Practices:

1. **Comprehending Scientific Presentations**: Reading and interpreting scientific materials
2. **Designing Scientific Investigations**: Hypothesis formation, experimental design, understanding variables
3. **Reasoning from Data**: Evidence-based conclusions, data analysis, and predictions
4. **Evaluating Scientific Claims**: Critically assessing evidence, theories, and peer-reviewed sources
5. **Expressing Scientific Information**: Communicating visually, numerically, and verbally
6. **Working with Scientific Models and Theories**: Applying theories and formulas, understanding model limitations
7. **Using Probability and Statistics**: Descriptive statistics, sampling, and probability
8. **Integrating Content**: Connecting and synthesizing concepts across scientific disciplines

## Getting Started

### Prerequisites

- **Python 3.10 or newer** (for building and serving the docs locally)
- **Git** — only needed if you plan to make changes (clone, branch, pull requests). For viewing or building only, you can download the repo as a ZIP.
- Basic familiarity with Markdown

### Get the code

- **Clone (for contributors):**  
  `git clone https://github.com/camgross/GED-Science-prep.git && cd GED-Science-prep`
- **Download ZIP (view or build only):** From the repo → **Code** → **Download ZIP**, then unzip and `cd` into the folder.

### Install Dependencies

```bash
pip install -r requirements.txt
```

**Optional: use a virtual environment** (recommended if you're new to Python):

```bash
python3 -m venv .venv
source .venv/bin/activate   # On Windows: .venv\Scripts\activate
pip install -r requirements.txt
```

### Build and Serve Locally

```bash
mkdocs serve
```

Then open **http://localhost:8000** in your browser.

### Deploy

The site is deployed to **GitHub Pages** via GitHub Actions on every push to `main`. No local deploy step is required. See the [Actions](https://github.com/camgross/GED-Science-prep/actions) tab for build status.

## Repository Structure

```
GED-Science-prep/
├── docs/
│   ├── chapters/          # 12 GED Science chapter directories
│   │   ├── 01-scientific-reasoning-foundations/
│   │   ├── 02-comprehending-scientific-materials/
│   │   └── ...
│   ├── learning-graph/    # Learning graph data and analysis
│   │   ├── course-description.md
│   │   ├── learning-graph.csv
│   │   ├── learning-graph.json
│   │   └── list-concepts.md
│   └── sims/              # Interactive MicroSims
│       ├── ged-science-assessment-framework/
│       ├── scientific-reasoning-process-flow/
│       └── ...
├── assessment-guide-for-educators-science.pdf
├── mkdocs.yml
└── README.md
```

## License

This work is licensed under the [Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License](https://creativecommons.org/licenses/by-nc-sa/4.0/).

## Contact

For questions or feedback, please open an issue in this repository.
