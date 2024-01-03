---
title: /enterprise/:id/treeCount/total
position_number: 1.8
type: get
description: Count the total number of trees for an enterprise
content_markdown_method: |-
  The following method allows you to retrieve the total number of trees planted by an enterprise.
parameters:
  - name: URL_PARAM
    content: id
    values: string
content_markdown: |-
  **id** Id of your enterprise. Example of an enterprise id: 11111111  (Enterprise Ids are 8 digits long)<br/>

  Status: 200
  {: .success}

  Response will be an object that has the following attributes:

  **count** Total number of trees planted by the enterprise

left_code_blocks:
  - code_block: |-
      https://api.digitalhumani.com/enterprise/:id/treeCount/total
    title:
    language: bash
right_request_blocks:
  - code_block: |1-
     https://api.digitalhumani.com/enterprise/11111111/treeCount/total
    title: Example request
    language: bash
right_code_blocks:
  - code_block: |2-
      {
        "count": 126
      }
    title: Example response
    language: json
---
