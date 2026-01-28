# GED Science Chapters - Generation Required

## Status

The GED Science chapter directories (01-12) were **never committed to git** and have been deleted from the working directory. They need to be regenerated.

## What Exists

✅ **Chapter structure defined** - `/Users/camgross/Projects/GED-Science-prep/docs/chapters/index.md` contains the complete 12-chapter structure with descriptions

✅ **Learning graph** - All 200 GED Science concepts are defined in:
- `docs/learning-graph/learning-graph.csv`
- `docs/learning-graph/learning-graph.json`
- `docs/learning-graph/list-concepts.md`

✅ **Chapter 1 placeholder** - Directory exists but needs content generation

## What Needs to Be Done

### Regenerate All 12 Chapters

Use the `chapter-content-generator` skill to generate content for each chapter:

1. **Chapter 1: Scientific Reasoning Foundations** (15 concepts)
   - Concepts: Scientific Reasoning, Assessment Targets, Career and College Readiness Standards, Science Practices, Content Topics, Depth of Knowledge (DOK), Test Item Alignment, Scientific Method, Evidence-Based Reasoning, Data Interpretation, Scientific Literacy, Textual Scientific Presentations, Non-Textual Scientific Presentations, Visual Data Representation, Scientific Communication

2. **Chapter 2: Comprehending Scientific Materials** (18 concepts)
   - See `docs/learning-graph/list-concepts.md` for full concept list

3. **Chapters 3-12** - Follow the same process

### Process

For each chapter:

1. Identify the concepts from the learning graph (see `docs/chapters/index.md` for concept counts)
2. Use the `chapter-content-generator` skill with:
   - Chapter number and title
   - List of concepts for that chapter
   - Reading level: "Senior High" (for GED Science)
3. The skill will generate the full chapter content including:
   - YAML frontmatter
   - Educational content
   - Worked examples
   - Practice exercises
   - Interactive element specifications

### Reference

- Chapter structure: `docs/chapters/index.md`
- Concept list: `docs/learning-graph/list-concepts.md`
- Learning graph: `docs/learning-graph/learning-graph.json`

## Note

The dans-archive directories are empty placeholders. The actual chapter content was never committed to git and was lost when the working directory was cleaned up.
