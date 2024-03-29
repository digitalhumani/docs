---
title: /tree
position_number: 1.5
type: get
description: Count trees for a user
content_markdown_method: |-
  The following method allows you to retrieve the number of trees planted by a specific user
parameters:
  - name: QUERY PARAM
    content: enterpriseId
    values: string
  - name: QUERY PARAM
    content: user
    values: string
content_markdown: |-
  **enterpriseId** Id of your enterprise. Example of an enterprise id: 11111111 (Enterprise Ids are 8 digits long)<br/>
  **user** End user by whom the trees were planted. Example of an user: email@test.com

  Status: 200
  {: .success}

  Response will be an object that has the following attributes:

  **enterpriseId** Identifier of the enterprise<br/>
  **user** End user by whom the trees were planted<br/>
  **count** Number of trees planted by a specific user
left_code_blocks:
  - code_block: |-
     https://api.digitalhumani.com/tree?enterpriseId=:enterpriseId&user=:user
    title:
    language: bash
right_request_blocks:
  - code_block: |1-
     https://api.digitalhumani.com/tree?enterpriseId=48a45261&user=test_user_1
    title: Example request
    language: bash
right_code_blocks:
  - code_block: |2-
      {
        "enterpriseId": "48a45261",
        "user": "test_user_1",
        "count": 4
      }
    title: Example response
    language: json
---