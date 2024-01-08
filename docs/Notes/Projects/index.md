---
tags:
  - navigation
  - project
database-plugin: basic
share: true
---


```yaml:dbfolder
name: Projects
description: Projects
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
    config:
      enable_media_view: true
      link_alias_enabled: true
      media_width: 100
      media_height: 100
      isInline: true
      task_hide_completed: true
      footer_type: none
      persist_changes: false
  parent:
    input: relation
    accessorKey: parent
    key: parent
    id: parent
    label: Parent
    position: 4
    skipPersist: false
    isHidden: false
    sortIndex: -1
    width: 252
    config:
      enable_media_view: true
      link_alias_enabled: true
      media_width: 100
      media_height: 100
      isInline: true
      task_hide_completed: true
      footer_type: none
      persist_changes: false
      related_note_path: Notes/Projects/Projects.md
      bidirectional_relation: false
      relation_color: hsl(0,0%,0%)
  due:
    input: calendar
    accessorKey: due
    key: due
    id: due
    label: Due
    position: 2
    skipPersist: false
    isHidden: false
    sortIndex: -1
    config:
      enable_media_view: true
      link_alias_enabled: true
      media_width: 100
      media_height: 100
      isInline: true
      task_hide_completed: true
      footer_type: none
      persist_changes: false
  priority:
    input: select
    accessorKey: priority
    key: priority
    id: priority
    label: Priority
    position: 3
    skipPersist: false
    isHidden: false
    sortIndex: -1
    options:
      - { label: "[,medium]", value: "[,medium]", color: "hsl(36, 95%, 90%)"}
      - { label: "[,,medium]", value: "[,,medium]", color: "hsl(332, 95%, 90%)"}
      - { label: "medium", value: "medium", color: "hsl(320, 95%, 90%)"}
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
  sticky_first_column: true
  group_folder_column: 
  remove_empty_folders: true
  automatically_group_files: true
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
```