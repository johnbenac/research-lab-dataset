---
typeId: experiment
fields:
  displayName: Experiment
  pluralName: Experiments
  icon: flask
  bodyField: protocol

  fieldDefs:
    title:
      kind: string
      required: true
      ui:
        label: Title

    status:
      kind: enum
      options: [planned, in_progress, done]
      default: planned
      ui:
        label: Status

    date:
      kind: date
      ui:
        label: Date

    lead:
      kind: ref
      ui:
        label: Lead
        refTypeHints: [person]

    datasets:
      kind: ref[]
      ui:
        label: Datasets
        refTypeHints: [dataset]

    links:
      kind: ref[]
      ui:
        label: Links
---
