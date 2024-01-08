---
tags:
  - navigation
  - recipe
database-plugin: basic
share: true
---


```yaml:dbfolder
name: Recipes
description: Family Recipes
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
  recipe_meal:
    input: select
    accessorKey: recipe_meal
    key: recipe_meal
    id: recipe_meal
    label: Meal
    position: 2
    skipPersist: false
    isHidden: false
    sortIndex: -1
    options:
      - { label: "Snack", value: "Snack", color: "hsl(107,96%,90%)"}
      - { label: "Dinner", value: "Dinner", color: "hsl(0,96%,90%)"}
      - { label: "Dessert", value: "Dessert", color: "hsl(276,96%,90%)"}
    config:
      enable_media_view: true
      link_alias_enabled: true
      media_width: 100
      media_height: 100
      isInline: true
      task_hide_completed: true
      footer_type: none
      persist_changes: false
      option_source: manual
  recipe_type:
    input: select
    accessorKey: recipe_type
    key: recipe_type
    id: recipe_type
    label: Type
    position: 3
    skipPersist: false
    isHidden: false
    sortIndex: -1
    options:
      - { label: "炸", value: "炸", color: "hsl(50,96%,90%)"}
      - { label: "拌", value: "拌", color: "hsl(165,96%,90%)"}
      - { label: "炒", value: "炒", color: "hsl(18, 95%, 90%)"}
      - { label: "炖", value: "炖", color: "hsl(214,96%,90%)"}
      - { label: "蒸", value: "蒸", color: "hsl(271,96%,90%)"}
    config:
      enable_media_view: true
      link_alias_enabled: true
      media_width: 100
      media_height: 100
      isInline: true
      task_hide_completed: true
      footer_type: none
      persist_changes: false
      option_source: manual
  share:
    input: checkbox
    accessorKey: share
    key: share
    id: share
    label: Share
    position: 4
    skipPersist: false
    isHidden: false
    sortIndex: -1
    width: 41
    config:
      enable_media_view: true
      link_alias_enabled: true
      media_width: 100
      media_height: 100
      isInline: true
      task_hide_completed: true
      footer_type: none
      persist_changes: false
  recipe_detail:
    input: text
    accessorKey: recipe_detail
    key: recipe_detail
    id: recipe_instruction
    label: Detail
    position: 5
    skipPersist: false
    isHidden: false
    sortIndex: -1
    width: 670
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
  sticky_first_column: true
  group_folder_column: recipe_type
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