# File Restoration Status

## Successfully Restored ✅

1. **course-description.md** - Restored from commit 36c8c06d to `/Users/camgross/Projects/GED-Science-prep/docs/learning-graph/course-description.md`
2. **list-concepts.md** - Restored from commit 36c8c06d to `/Users/camgross/Projects/GED-Science-prep/docs/learning-graph/list-concepts.md`

## Cannot Restore (Not in Git History) ❌

1. **12 GED Science Chapter directories** - These were never committed to git, only existed in working directory
2. **6 GED Science MicroSim directories** - These were never committed to git:
   - ged-science-assessment-framework
   - scientific-reasoning-process-flow
   - scientific-method-cycle
   - scientific-data-visualization-types
   - quantitative-qualitative-data-collection
   - scientific-communication-process

## Manual Steps Required

### Assessment Guide PDF

The PDF exists in commit 36c8c06d but cannot be restored automatically due to file system permissions. To restore manually:

```bash
cd /Users/camgross/Projects/claude-skills
git show 36c8c06d:assessment-guide-for-educators-science.pdf > /Users/camgross/Projects/GED-Science-prep/assessment-guide-for-educators-science.pdf
```

### Chapters and MicroSims

These need to be regenerated:
- **Chapters**: Use the `chapter-content-generator` skill to regenerate all 12 chapters
- **MicroSims**: Use the `microsim-generator` skill to regenerate the 6 MicroSims

See `CHAPTER-GENERATION-NEEDED.md` for details on regenerating chapters.
