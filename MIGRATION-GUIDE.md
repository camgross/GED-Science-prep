# GED Science Content Migration Guide

This guide documents the migration of GED Science content from the claude-skills repository to the new GED-Science-prep repository.

## Status

Due to file system permission restrictions, some bulk file operations need to be completed manually. This guide provides step-by-step instructions.

## Files Already Copied

The following files have been successfully copied to `/Users/camgross/Projects/GED-Science-prep/`:

- `docs/chapters/index.md` - GED Science chapter structure
- `docs/learning-graph/course-description.md` - GED Science course description
- `docs/learning-graph/learning-graph.csv` - GED Science concepts (200 concepts)
- `docs/learning-graph/learning-graph.json` - GED Science vis-network format
- `docs/learning-graph/list-concepts.md` - GED Science concept enumeration

## Files That Need Manual Copying

### 1. GED Science Chapters (12 directories)

Run these commands from `/Users/camgross/Projects/claude-skills`:

```bash
# Copy all 12 GED Science chapter directories
for i in {01..12}; do
  for dir in docs/chapters/$i-*; do
    if [ -d "$dir" ]; then
      cp -r "$dir" /Users/camgross/Projects/GED-Science-prep/docs/chapters/
      echo "Copied $(basename $dir)"
    fi
  done
done
```

### 2. GED Science MicroSims (6 directories)

```bash
# Copy GED Science MicroSims
for sim in ged-science-assessment-framework scientific-reasoning-process-flow scientific-method-cycle scientific-data-visualization-types quantitative-qualitative-data-collection scientific-communication-process; do
  if [ -d "docs/sims/$sim" ]; then
    cp -r "docs/sims/$sim" /Users/camgross/Projects/GED-Science-prep/docs/sims/
    echo "Copied $sim"
  fi
done
```

### 3. Assessment Guide PDF

```bash
# Copy assessment guide
if [ -f "assessment-guide-for-educators-science.pdf" ]; then
  cp assessment-guide-for-educators-science.pdf /Users/camgross/Projects/GED-Science-prep/
  echo "Copied assessment guide"
fi
```

### 4. Learning Graph Files (if modified)

Check if these files were modified for GED Science:

```bash
# Check for modifications
cd /Users/camgross/Projects/claude-skills
git diff '36c8c06d^' HEAD -- docs/learning-graph/quality-metrics.md
git diff '36c8c06d^' HEAD -- docs/learning-graph/taxonomy-distribution.md

# If modified, copy them:
# cp docs/learning-graph/quality-metrics.md /Users/camgross/Projects/GED-Science-prep/docs/learning-graph/
# cp docs/learning-graph/taxonomy-distribution.md /Users/camgross/Projects/GED-Science-prep/docs/learning-graph/
```

## Next Steps After Copying

1. **Create mkdocs.yml** for GED-Science-prep repository
2. **Create README.md** for GED-Science-prep repository
3. **Initialize git repository** in GED-Science-prep
4. **Restore original files** in claude-skills repository
5. **Update mkdocs.yml** in claude-skills to remove GED Science entries

See the plan document for complete details.
