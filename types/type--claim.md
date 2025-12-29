---
id: type:claim
datasetId: dataset:research-lab
typeId: sys:type
createdAt: 2025-12-01T00:00:00Z
updatedAt: 2025-12-01T00:00:00Z
fields:
  recordTypeId: claim
  displayName: Claim
  pluralName: Claims
  icon: link
  bodyField: rationale

  fieldDefs:
    statement:
      kind: string
      required: true
      ui:
        label: Statement

    confidence:
      kind: number
      constraints:
        min: 0
        max: 1
      ui:
        label: Confidence (0–1)

    supports:
      kind: ref[]
      ui:
        label: Supported by

    contradicts:
      kind: ref[]
      ui:
        label: Contradicted by

    links:
      kind: ref[]
      ui:
        label: Links
---
