---

database-plugin: basic

---

<%%
name: Summary
description: Summary from Library
columns:
  __file__:
    key: __file__
    input: markdown
    label: File
    accessor: __file__
    isMetadata: true
    skipPersist: false
    isDragDisabled: false
    csvCandidate: true
    position: 1
    isSorted: true
    isSortedDesc: true
    config:
      enable_media_view: true
      media_width: 100
      media_height: 100
      isInline: false
      source_data: current_folder
  Author:
    input: select
    accessor: Author
    key: Author
    label: Author
    position: 3
    options:
      - { label: "Jose Moruno", backgroundColor: "hsl(54, 95%, 90%)"}
      - { label: "SniferL4bs", backgroundColor: "hsl(100, 95%, 90%)"}
      - { label: "Benito Taibo", backgroundColor: "hsl(201, 95%, 90%)"}
      - { label: "Edward Snowden", backgroundColor: "hsl(89, 95%, 90%)"}
    config:
      enable_media_view: true
      media_width: 100
      media_height: 100
      isInline: false
      source_data: current_folder
  Title:
    input: text
    accessor: Title
    key: Title
    label: Title
    position: 2
    config:
      enable_media_view: true
      media_width: 100
      media_height: 100
      isInline: false
      source_data: current_folder
  Type:
    input: select
    accessor: Type
    key: Type
    label: Type
    position: 4
    options:
      - { label: "Book", backgroundColor: "hsl(234, 95%, 90%)"}
      - { label: "✍️ Annotation", backgroundColor: "hsl(342, 95%, 90%)"}
      - { label: "🗂️ Index", backgroundColor: "hsl(53, 95%, 90%)"}
      - { label: "Video", backgroundColor: "hsl(357, 95%, 90%)"}
      - { label: "Course", backgroundColor: "hsl(102, 95%, 90%)"}
      - { label: "📝 Document", backgroundColor: "hsl(336, 95%, 90%)"}
      - { label: "💭 Quote", backgroundColor: "hsl(224, 95%, 90%)"}
      - { label: "📽️ Video", backgroundColor: "hsl(133, 95%, 90%)"}
      - { label: "🖼️ Image", backgroundColor: "hsl(93, 95%, 90%)"}
    config:
      enable_media_view: true
      media_width: 100
      media_height: 100
      isInline: false
      source_data: current_folder
  Status:
    input: select
    accessor: Status
    key: Status
    label: Status
    position: 5
    options:
      - { label: "To Read", backgroundColor: "hsl(119, 95%, 90%)"}
      - { label: "In Progress", backgroundColor: "hsl(291, 95%, 90%)"}
      - { label: "Not Started", backgroundColor: "hsl(75, 95%, 90%)"}
      - { label: "Completed", backgroundColor: "hsl(260, 95%, 90%)"}
      - { label: "Reading", backgroundColor: "hsl(312, 95%, 90%)"}
    config:
      enable_media_view: true
      media_width: 100
      media_height: 100
      isInline: false
      source_data: current_folder
  Rating:
    input: select
    accessor: Rating
    key: Rating
    label: Rating
    position: 8
    options:
      - { label: "⭐", backgroundColor: "hsl(178, 95%, 90%)"}
      - { label: "⭐⭐", backgroundColor: "hsl(156, 95%, 90%)"}
      - { label: "⭐⭐⭐", backgroundColor: "hsl(90, 95%, 90%)"}
      - { label: "⭐⭐⭐⭐", backgroundColor: "hsl(350, 95%, 90%)"}
      - { label: "⭐⭐⭐⭐⭐", backgroundColor: "hsl(19, 95%, 90%)"}
    config:
      enable_media_view: true
      media_width: 100
      media_height: 100
      isInline: false
      source_data: current_folder
  Category:
    input: select
    accessor: Category
    key: Category
    label: Category
    position: 9
    options:
      - { label: "Ficcion", backgroundColor: "hsl(189, 95%, 90%)"}
    config:
      enable_media_view: true
      media_width: 100
      media_height: 100
      isInline: false
      source_data: current_folder
  Reference:
    input: text
    accessor: Reference
    key: Reference
    label: Reference
    position: 6
    config:
      enable_media_view: true
      media_width: 100
      media_height: 100
      isInline: false
      source_data: current_folder
  Finish_Read:
    input: calendar
    accessor: Finish_Read
    key: Finish_Read
    label: Finish Read
    position: 10
    config:
      enable_media_view: true
      media_width: 100
      media_height: 100
      isInline: false
      source_data: current_folder
  Tag:
    input: select
    accessor: Tag
    key: Tag
    label: Tag
    position: 7
    options:
      - { label: "Pentesting", backgroundColor: "hsl(174, 95%, 90%)"}
      - { label: "Personal", backgroundColor: "hsl(114, 95%, 90%)"}
    config:
      enable_media_view: true
      media_width: 100
      media_height: 100
      isInline: false
      source_data: current_folder
config:
  enable_show_state: false
  group_folder_column: 
  remove_field_when_delete_column: false
  show_metadata_created: false
  show_metadata_modified: false
  source_data: current_folder
  source_form_result: root
  cell_size: normal
  sticky_first_column: false
filters:
%%>