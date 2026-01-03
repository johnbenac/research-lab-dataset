---
typeId: evaluation
fields:
  displayName: Evaluation
  pluralName: Evaluations
  icon: checklist
  bodyField: notes

  composition:
    dataset:
      typeId: dataset
      required: true
    experiment:
      typeId: experiment
      required: true

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
