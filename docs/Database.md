---
tags:
  - navigation
database-plugin: basic
share: true
---


```yaml:dbfolder
name: Database
description: Database
columns:
  __file__:
    key: __file__
    id: __file__
    input: markdown
    label: File
    accessorKey: __file__
    isMetadata: true
    skipPersist: false
    isDragDisabled: false
    csvCandidate: true
    position: 0
    isHidden: false
    sortIndex: -1
    width: 95
    config:
      enable_media_view: true
      link_alias_enabled: true
      media_width: 100
      media_height: 100
      isInline: true
      task_hide_completed: true
      footer_type: none
      persist_changes: false
config:
  remove_field_when_delete_column: false
  cell_size: normal
  sticky_first_column: false
  group_folder_column: 
  remove_empty_folders: false
  automatically_group_files: false
  hoist_files_with_empty_attributes: true
  show_metadata_created: false
  show_metadata_modified: false
  show_metadata_tasks: false
  show_metadata_inlinks: false
  show_metadata_outlinks: false
  show_metadata_tags: false
  source_data: current_folder
  source_form_result: 
  source_destination_path: /
  row_templates_folder: /
  current_row_template: 
  pagination_size: 20
  font_size: 16
  enable_js_formulas: false
  formula_folder_path: /
  inline_default: false
  inline_new_position: last_field
  date_format: yyyy-MM-dd
  datetime_format: "yyyy-MM-dd HH:mm:ss"
  metadata_date_format: "yyyy-MM-dd HH:mm:ss"
  enable_footer: false
  implementation: default
filters:
  enabled: true
  conditions:
      - condition: OR
        disabled: false
        label: "📁"
        color: "hsl(0,0%,77%)"
        filters:
        - field: database-plugin
          operator: IS_NOT_EMPTY
          value: ""
          type: text
        - field: tags
          operator: CONTAINS
          value: "navigation"
          type: text
      - condition: AND
        disabled: true
        label: "🍱"
        color: "hsl(305,100%,86%)"
        filters:
        - field: tags
          operator: CONTAINS
          value: "recipe"
          type: text
        - field: file.name
          operator: NOT_CONTAINS
          value: "Template"
          type: text
        - field: database-plugin
          operator: IS_EMPTY
          value: ""
          type: text
      - condition: AND
        disabled: true
        label: "🗃"
        color: "hsl(217,96%,90%)"
        filters:
        - field: tags
          operator: CONTAINS
          value: "project"
          type: text
        - field: file.name
          operator: NOT_CONTAINS
          value: "Template"
          type: text
        - field: database-plugin
          operator: IS_EMPTY
          value: ""
          type: text
      - condition: AND
        disabled: true
        label: "🧑"
        color: "hsl(50,96%,90%)"
        filters:
        - field: tags
          operator: CONTAINS
          value: "people"
          type: text
        - field: file.name
          operator: NOT_CONTAINS
          value: "Template"
          type: text
        - field: database-plugin
          operator: IS_EMPTY
          value: ""
          type: text
      - condition: AND
        disabled: true
        label: "🏫"
        color: "hsl(121,96%,90%)"
        filters:
        - field: tags
          operator: CONTAINS
          value: "course"
          type: text
        - field: file.name
          operator: NOT_CONTAINS
          value: "Template"
          type: text
        - field: database-plugin
          operator: IS_EMPTY
          value: ""
          type: text
```