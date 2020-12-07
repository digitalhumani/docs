---
title: /tree/:uuid
position_number: 1.4
type: get
description: Get details of a single request to plant one or many trees
content_markdown_method: |-
  The following method allows you to retrieve the details of a single request request to plant trees.
parameters:
  - name: URL_PARAM
    content: uuid
    values: string
content_markdown: |-
  **uuid** uuid of the trees for which you want to get the details. Example of an uuid: eef9f369-9ae0-45b8-ab07-10650f53a71e (uuids are 36 digits long)

  Status: 200
  {: .success}

  Response will be an object that has the following attributes:

  **uuid** Universally Unique Identifier generated (string)<br/>
  **created** Creation date of the trees in the RaaS database (ISO 8601 Date and Time format)<br/>
  **treeCount** Number of trees requested to plant (integer)<br/>
  **enterpriseId** identifier of the enterprise (string)<br/>
  **projectId** identifier of the project (string)<br/>
  **user** End user by whom the trees were planted (string)
left_code_blocks:
  - code_block: |-
     https://api.digitalhumani.com/tree/:uuid-of-tree-planted
    title:
    language: bash
right_request_blocks:
  - code_block: |1-
     https://api.digitalhumani.com/tree/bcd35c97-d66c-412e-89ae-ecbac0f629ac
    title: Example request
    language: bash
right_code_blocks:
  - code_block: |2-
      {
        "projectId": "81818182",
        "created": "2020-04-11T18:01:40.441Z",
        "uuid": "bcd35c97-d66c-412e-89ae-ecbac0f629ac",
        "user": "1",
        "treeCount": 1,
        "enterpriseId": "33333333"
      }
    title: Example response
    language: json
---

