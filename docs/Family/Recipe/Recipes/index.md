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
    input: relation
    accessorKey: recipe_meal
    key: recipe_meal
    id: recipe_meal
    label: Meal
    position: 3
    skipPersist: false
    isHidden: false
    sortIndex: -1
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
      related_note_path: Family/Recipe/Recipe Meals/Recipe Meals.md
      relation_color: hsl(0,0%,0%)
  recipe_type:
    input: relation
    accessorKey: recipe_type
    key: recipe_type
    id: recipe_type
    label: Type
    position: 2
    skipPersist: false
    isHidden: false
    sortIndex: -1
    isSorted: false
    isSortedDesc: false
    width: 156
    config:
      enable_media_view: true
      link_alias_enabled: true
      media_width: 100
      media_height: 100
      isInline: false
      task_hide_completed: true
      footer_type: none
      persist_changes: false
      related_note_path: Family/Recipe/Recipe Types/Recipe Types.md
      relation_color: hsl(0,0%,0%)
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
      isInline: false
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
  source_data: query
  source_form_result: "from \"Family/Recipe/Recipes\""
  source_destination_path: Family/Recipe/Recipes
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