---
title: /tree
position_number: 1.5
type: get
description: Count trees for a user
content_markdown_method: |-
  The following method allows you to retrieve the number of trees   planted by a specific user
parameters:
  - name: QUERY PARAM
    content: enterpriseId
    values: string
  - name: QUERY PARAM
    content: user
    values: string
content_markdown: |-
  **enterpriseId** Id of your enterprise. Example of an enterprise id: 11111111 (Enterprise Ids are 8 digits long)<br/>
  **user** End user by whom the tree was planted. Example of an user: email@test.com

  Status: 200
  {: .success}

  Response will be an object that has the following attributes:

  **enterpriseId** Identifier of the enterprise<br/>
  **user** End user by whom the tree was planted<br/>
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
        "uuid": "eef9f369-9ae0-45b8-ab07-10650f53a71e",
        "created": "2019-05-17T00:36:25.797Z",
        "treeCount": 2,
        "enterpriseId": "11111111",
        "projectId": "93333333",
        "user": "email@test.com"
      }
    title: Example response
    language: json
---