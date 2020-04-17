---
title: /enterprise/:id/treeCount
position_number: 1.7
type: get
description: Count trees for an enterprise for any range of date
content_markdown_method: |-
  The following method allows you to retrieve the number of trees planted by an enterprise for any range of date.
parameters:
  - name: URL_PARAM
    content: id
    values: string
  - name: QUERY PARAM
    content: startDate
    values: date (YYYY-MM-DD)
  - name: QUERY PARAM
    content: endDate
    values: date (YYYY-MM-DD)
content_markdown: |-
  **id** Id of your enterprise. Example of an enterprise id: 11111111  (Enterprise Ids are 8 digits long)<br/>
  **startDate** Start Date of the range to specify (start-date will be included in the results). Date format is as follow: (YYYY-MM-DD)<br/>
  **endDate** End Date of the range to specify (end-date will be included in the results). Date format is as follow: (YYYY-MM-DD)

  Status: 200
  {: .success}

  Response will be an object that has the following attributes:

  **count** Number of trees planted by the enterprise for the specified range

left_code_blocks:
  - code_block: |-
     https://api.digitalhumani.com/enterprise/:id/treeCount?startDate=YYYY-MM-DD&endDate=YYYY-MM-DD
    title:
    language: bash
right_request_blocks:
  - code_block: |1-
     https://api.digitalhumani.com/enterprise/11111111/treeCount?startDate=2010-03-01&endDate=2030-01-01
    title: Example request
    language: bash
right_code_blocks:
  - code_block: |2-
      {
        "count": 57
      }
    title: Example response
    language: json
---


