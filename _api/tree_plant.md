---
title: /tree
position_number: 1.3
type: post
description: Plant one or many trees
content_markdown_method: |-
  The following  method sends the request to plant one or many trees.
parameters:
  - name: Body Parameter
    content: enterpriseId
    values: string
  - name: Body Parameter
    content: projectId
    values: string
  - name: Body Parameter
    content: user
    values: string
  - name: Body Parameter
    content: treeCount
    values: integer
content_markdown: |-
  The request is encoded in [JSON](https://en.wikipedia.org/wiki/JSON) and the parameters need to be passed in the body of the request.

  In the header, “Content-Type” requires to have a value of “application/json”
  {: .warning}

  **enterpriseId**  Id of your enterprise. Example of an enterprise id: 11111111  (Enterprise Ids are 8 digits long)<br/>
  **projectId** Id of the reforestation project for where you want the trees to be planted. Example of an id: 93333333  (Project Ids are 8 digits long)<br/>
  **user** End user by whom the trees were planted. Example of an user: email@test.com<br/>
  **treeCount** Number of trees requested to plant. Example: 1<br/>

  Status: 200
  {: .success}

  Response will be an object that has the following attributes:

  **uuid** Universally Unique Identifier generated (string)<br/>
  **created** Creation date of the trees in the RaaS database (ISO 8601 Date and Time format)<br/>
  **treeCount** Number of trees requested to plant (integer)<br/>
  **enterpriseId** Identifier of the enterprise (string)<br/>
  **projectId** Identifier of the project (string)<br/>
  **user** End user by whom the trees were planted (string)


left_code_blocks:
  - code_block: |-
     !API_URL!/tree + Body Parameters described below
    title:
    language: bash
right_request_blocks:
  - code_block: |1-
     !API_URL!/tree
     Body parameters
     {
       "treeCount": 1,
       "enterpriseId": "1234abcd",
       "projectId": "93322249",
       "user": "test_user_1"
     }
    title: Example request
    language: bash
right_code_blocks:
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