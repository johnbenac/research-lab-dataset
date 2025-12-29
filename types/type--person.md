---
id: type:person
datasetId: dataset:research-lab
typeId: sys:type
createdAt: 2025-12-01T00:00:00Z
updatedAt: 2025-12-01T00:00:00Z
fields:
  recordTypeId: person
  displayName: Person
  pluralName: People
  icon: user
  bodyField: bio

  fieldDefs:
    name:
      kind: string
      required: true
      ui:
        label: Name

    affiliation:
      kind: string
      ui:
        label: Affiliation
---
