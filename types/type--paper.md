---
typeId: paper
fields:
  displayName: Paper
  pluralName: Papers
  icon: book
  bodyField: notes

  fieldDefs:
    title:
      kind: string
      required: true
      ui:
        label: Title

    year:
      kind: number
      constraints:
        min: 1600
        max: 2100
      ui:
        label: Year

    authors:
      kind: ref[]
      ui:
        label: Authors
        refTypeHints: [person]

    url:
      kind: url
      ui:
        label: URL

    doi:
      kind: string
      ui:
        label: DOI

    concepts:
      kind: ref[]
      ui:
        label: Concepts
        refTypeHints: [concept]

    cites:
      kind: ref[]
      ui:
        label: Cites
        refTypeHints: [paper]

    links:
      kind: ref[]
      ui:
        label: Links
---
