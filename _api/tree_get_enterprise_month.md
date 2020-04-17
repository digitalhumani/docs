---
title: /enterprise/:id/treeCount/:month
position_number: 1.6
type: get
description: Count trees for an enterprise by month
content_markdown_method: |-
    The following method allows you to retrieve the number of trees planted by an enterprise for a specific month
parameters:
  - name: URL_PARAM
    content: id
    values: string
  - name: URL_PARAM
    content: month
    values: string
content_markdown: |-
  **id** Id of your enterprise. Example of an enterprise id: 11111111  (Enterprise Ids are 8 digits long)<br/>
  **month** Month for which you want to count the number of trees planted. Example of a month: 2020-02
 
  Status: 200
  {: .success}

  Response will be an object that has the following attributes:

  **count** Number of trees planted by the enterprise for a specific month
left_code_blocks:
  - code_block: |-
     https://api.digitalhumani.com/enterprise/:id/treeCount/YYYY-MM
    title:
    language: bash
right_request_blocks:
  - code_block: |1-
     https://api.digitalhumani.com/enterprise/11111111/treeCount/2020-02
    title: Example request
    language: bash
right_code_blocks:
  - code_block: |2-
      {
        "count": 17
      }
    title: Example response
    language: json
---