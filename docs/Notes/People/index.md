---
tags:
  - navigation
  - people
database-plugin: basic
share: true
---


```yaml:dbfolder
name: People
description: People
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
    width: -824
    config:
      enable_media_view: true
      link_alias_enabled: true
      media_width: 100
      media_height: 100
      isInline: true
      task_hide_completed: true
      footer_type: none
      persist_changes: false
  people_firstname:
    input: text
    accessorKey: people_firstname
    key: people_firstname
    id: people_firstname
    label: Firstname
    position: 2
    skipPersist: false
    isHidden: true
    sortIndex: -1
    width: 114
    config:
      enable_media_view: true
      link_alias_enabled: true
      media_width: 100
      media_height: 100
      isInline: true
      task_hide_completed: true
      footer_type: none
      persist_changes: false
  people_lastname:
    input: text
    accessorKey: people_lastname
    key: people_lastname
    id: people_lastname
    label: Lastname
    position: 4
    skipPersist: false
    isHidden: true
    sortIndex: -1
    width: 100
    config:
      enable_media_view: true
      link_alias_enabled: true
      media_width: 100
      media_height: 100
      isInline: true
      task_hide_completed: true
      footer_type: none
      persist_changes: false
  people_organization:
    input: text
    accessorKey: people_organization
    key: people_organization
    id: people_organization
    label: Organization
    position: 5
    skipPersist: false
    isHidden: false
    sortIndex: -1
    width: 80
    config:
      enable_media_view: true
      link_alias_enabled: true
      media_width: 100
      media_height: 100
      isInline: true
      task_hide_completed: true
      footer_type: none
      persist_changes: false
  people_department:
    input: text
    accessorKey: people_department
    key: people_department
    id: people_department
    label: Department
    position: 6
    skipPersist: false
    isHidden: false
    sortIndex: -1
    width: -35
    config:
      enable_media_view: true
      link_alias_enabled: true
      media_width: 100
      media_height: 100
      isInline: true
      task_hide_completed: true
      footer_type: none
      persist_changes: false
  people_title:
    input: text
    accessorKey: people_title
    key: people_title
    id: people_title
    label: Title
    position: 7
    skipPersist: false
    isHidden: false
    sortIndex: -1
    width: -68
    config:
      enable_media_view: true
      link_alias_enabled: true
      media_width: 100
      media_height: 100
      isInline: true
      task_hide_completed: true
      footer_type: none
      persist_changes: false
  people_email:
    input: text
    accessorKey: people_email
    key: people_email
    id: people_email
    label: Email
    position: 8
    skipPersist: false
    isHidden: false
    sortIndex: -1
    width: -41
    config:
      enable_media_view: true
      link_alias_enabled: true
      media_width: 100
      media_height: 100
      isInline: true
      task_hide_completed: true
      footer_type: none
      persist_changes: false
  people_phone:
    input: text
    accessorKey: people_phone
    key: people_phone
    id: people_phone
    label: Phone
    position: 9
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
  people_year:
    input: text
    accessorKey: people_year
    key: people_year
    id: people_year
    label: Year
    position: 10
    skipPersist: false
    isHidden: false
    sortIndex: -1
    width: 35
    config:
      enable_media_view: true
      link_alias_enabled: true
      media_width: 100
      media_height: 100
      isInline: true
      task_hide_completed: true
      footer_type: none
      persist_changes: false
  people_birthyear:
    input: text
    accessorKey: people_birthyear
    key: people_birthyear
    id: people_birthyear
    label: Birthyear
    position: 11
    skipPersist: false
    isHidden: false
    sortIndex: -1
    width: -85
    config:
      enable_media_view: true
      link_alias_enabled: true
      media_width: 100
      media_height: 100
      isInline: true
      task_hide_completed: true
      footer_type: none
      persist_changes: false
  people_birthday:
    input: text
    accessorKey: people_birthday
    key: people_birthday
    id: people_birthday
    label: Birthday
    position: 12
    skipPersist: false
    isHidden: false
    sortIndex: -1
    width: 42
    config:
      enable_media_view: true
      link_alias_enabled: true
      media_width: 100
      media_height: 100
      isInline: true
      task_hide_completed: true
      footer_type: none
      persist_changes: false
  people_deathdate:
    input: text
    accessorKey: people_deathdate
    key: people_deathdate
    id: people_deathdate
    label: Deathdate
    position: 13
    skipPersist: false
    isHidden: false
    sortIndex: -1
    width: 37
    config:
      enable_media_view: true
      link_alias_enabled: true
      media_width: 100
      media_height: 100
      isInline: true
      task_hide_completed: true
      footer_type: none
      persist_changes: false
  note:
    input: text
    accessorKey: note
    key: note
    id: note
    label: Note
    position: 14
    skipPersist: false
    isHidden: false
    sortIndex: -1
    width: 70
    config:
      enable_media_view: true
      link_alias_enabled: true
      media_width: 100
      media_height: 100
      isInline: true
      task_hide_completed: true
      footer_type: none
      persist_changes: false
  people_middlename:
    input: text
    accessorKey: people_middlename
    key: people_middlename
    id: people_middlename
    label: Middlename
    position: 3
    skipPersist: false
    isHidden: true
    sortIndex: -1
    width: 26
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
  pagination_size: 10
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