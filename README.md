# GED Science Prep

A comprehensive GED Science preparation resource covering all 200 assessment targets across Life Science, Physical Science, and Earth and Space Science.

## Overview

This repository contains a complete 12-chapter GED Science curriculum designed to prepare adult learners for the GED Science Test. The content is structured around the eight Science Practices and three content domains specified in the GED Assessment Targets.

## Course Structure

- **12 Chapters** covering all 200 concepts
- **Learning Graph** with concept dependencies and taxonomy
- **Interactive MicroSims** for visual learning
- **Assessment Guide** reference materials

## Content Domains

- **Life Science (40%)** - Human body systems, energy flow, cellular organization, genetics, heredity, and evolution
- **Physical Science (40%)** - Energy conservation, work and motion, chemical properties and reactions
- **Earth and Space Science (20%)** - Earth systems, atmospheric and oceanic characteristics, cosmic structures

## Science Practices

The curriculum is organized around eight core Science Practices:

1. **Comprehending Scientific Presentations** - Reading and interpreting scientific materials
2. **Designing Scientific Investigations** - Hypothesis formation, experimental design, variables
3. **Reasoning from Data** - Evidence-based conclusions, data analysis, predictions
4. **Evaluating Scientific Claims** - Assessing evidence, theory evaluation, peer review
5. **Expressing Scientific Information** - Visual, numerical, and verbal communication
6. **Working with Scientific Models and Theories** - Theory application, formula use, model limitations
7. **Using Probability and Statistics** - Descriptive statistics, sampling, probability
8. **Integrating Content** - Connecting concepts across scientific disciplines

## Getting Started

### Prerequisites

- Python 3.8 or higher
- Git
- Basic familiarity with markdown

### Install Dependencies

```bash
pip install mkdocs
pip install mkdocs-material
pip install pymdown-extensions
```

### Build and Serve Locally

```bash
mkdocs serve
# Opens at http://localhost:8000
```

### Deploy to GitHub Pages

```bash
mkdocs gh-deploy
```

## Repository Structure

```
GED-Science-prep/
├── docs/
│   ├── chapters/          # 12 GED Science chapters
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

For questions or feedback, please open an issue on GitHub.
