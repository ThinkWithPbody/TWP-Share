---
tags:
  - navigation
  - course
database-plugin: basic
share: true
---


```yaml:dbfolder
name: Courses
description: Courses
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
    position: 1
    isHidden: false
    sortIndex: -1
    width: 217
    config:
      enable_media_view: true
      link_alias_enabled: true
      media_width: 100
      media_height: 100
      isInline: true
      task_hide_completed: true
      footer_type: none
      persist_changes: false
      wrap_content: true
  year:
    input: number
    accessorKey: year
    key: year
    id: year
    label: Year
    position: 2
    skipPersist: false
    isHidden: false
    sortIndex: -1
    config:
      enable_media_view: true
      link_alias_enabled: true
      media_width: 100
      media_height: 100
      isInline: false
      task_hide_completed: true
      footer_type: none
      persist_changes: false
  quarter:
    input: select
    accessorKey: quarter
    key: quarter
    id: quarter
    label: Quarter
    position: 3
    skipPersist: false
    isHidden: false
    sortIndex: -1
    options:
      - { label: "Winter", value: "1", color: "hsl(217, 95%, 90%)"}
      - { label: "Spring", value: "2", color: "hsl(132,96%,90%)"}
      - { label: "Summer", value: "3", color: "hsl(36,96%,90%)"}
      - { label: "Fall", value: "4", color: "hsl(320,96%,90%)"}
    config:
      enable_media_view: true
      link_alias_enabled: true
      media_width: 100
      media_height: 100
      isInline: false
      task_hide_completed: true
      footer_type: none
      persist_changes: false
      option_source: manual
  Time:
    input: text
    accessorKey: Time
    key: Time
    id: Time
    label: Time
    position: 4
    skipPersist: false
    isHidden: false
    sortIndex: -1
    width: 128
    isSorted: false
    isSortedDesc: false
    config:
      enable_media_view: true
      link_alias_enabled: true
      media_width: 100
      media_height: 100
      isInline: false
      task_hide_completed: true
      footer_type: none
      persist_changes: false
  Location:
    input: select
    accessorKey: Location
    key: Location
    id: Location
    label: Location
    position: 5
    skipPersist: false
    isHidden: false
    sortIndex: -1
    options:
      - { label: "TBA", value: "TBA", color: "hsl(320, 95%, 90%)"}
      - { label: "DA 200", value: "DA 200", color: "hsl(58, 95%, 90%)"}
    config:
      enable_media_view: true
      link_alias_enabled: true
      media_width: 100
      media_height: 100
      isInline: false
      task_hide_completed: true
      footer_type: none
      persist_changes: false
config:
  remove_field_when_delete_column: false
  cell_size: normal
  sticky_first_column: false
  group_folder_column: 
  remove_empty_folders: true
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
  inline_default: true
  inline_new_position: last_field
  date_format: yyyy-MM-dd
  datetime_format: "yyyy-MM-dd HH:mm:ss"
  metadata_date_format: "yyyy-MM-dd HH:mm:ss"
  enable_footer: false
  implementation: default
filters:
  enabled: false
  conditions:
      - condition: AND
        disabled: false
        label: "2024 Winter"
        color: "hsl(248, 95%, 90%)"
        filters:
        - field: year
          operator: CONTAINS
          value: "2024"
          type: number
      - field: quarter
        operator: EQUAL
        value: "1"
        type: select
```