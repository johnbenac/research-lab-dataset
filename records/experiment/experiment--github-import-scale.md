---
typeId: experiment
recordId: github-import-scale
fields:
  title: "GitHub import at scale"
  status: in_progress
  date: 2025-12-22
  lead: "[[person:vaswani]]"
  datasets:
    - "[[dataset:seed-demo]]"
  links:
    - "[[claim:md-round-trip]]"
    - "[[paper:attention-is-all-you-need]]"
---
## Protocol
1. Use GitHub tree API with `?recursive=1`
2. Filter to `.md` files
3. Fetch via `raw.githubusercontent.com`
4. Validate YAML + required fields
5. Extract `[[id]]` links

## Expected outcome
Deterministic import/export round-trip for [[dataset:seed-demo]].
