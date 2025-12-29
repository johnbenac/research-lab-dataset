---
id: type:dataset
datasetId: dataset:research-lab
typeId: sys:type
createdAt: 2025-12-01T00:00:00Z
updatedAt: 2025-12-01T00:00:00Z
fields:
  recordTypeId: dataset
  displayName: Dataset Artifact
  pluralName: Dataset Artifacts
  icon: database
  bodyField: notes

  fieldDefs:
    name:
      kind: string
      required: true
      ui:
        label: Name

    kind:
      kind: enum
      options: [seed, benchmark, scraped, synthetic]
      default: seed
      ui:
        label: Kind

    links:
      kind: ref[]
      ui:
        label: Links
---
