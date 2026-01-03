---
typeId: dataset
fields:
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

    description:
      kind: string
      ui:
        label: Description

    links:
      kind: ref[]
      ui:
        label: Links
---
