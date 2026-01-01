---
id: type:evaluation
datasetId: dataset:research-lab
typeId: sys:type
createdAt: 2025-12-30T00:00:00Z
updatedAt: 2025-12-30T00:00:00Z
fields:
  recordTypeId: evaluation
  displayName: Evaluation
  pluralName: Evaluations
  icon: checklist
  bodyField: notes
  composition:
    dataset:
      recordTypeId: dataset
      min: 1
    experiment:
      recordTypeId: experiment
      min: 1
  fieldDefs:
    name:
      kind: string
      required: true
    datasetRefs:
      kind: ref[]
      ui:
        label: Datasets
        refTypeHints: [dataset]
    experimentRefs:
      kind: ref[]
      ui:
        label: Experiments
        refTypeHints: [experiment]
    notes:
      kind: string
---
