---
title: /enterprise/:id
position_number: 1.0
type: get
description: Get Enterprise by ID
content_markdown_method: |-
  The following method allows you to retrieve the details of your enterprise.
parameters:
  - name: URL_PARAM
    content: id
    values: string
content_markdown: |-
  **id** Id of the enterprise for which you want to get the details. Example of an id: 11111111  (Enterprise Ids are 8 digits long)

  Status: 200
  {: .success}

  Response will be an object containing the details of an Enterprise, with the following attributes:

  **created** Creation date of the enterprise in the RaaS database (ISO 8601 Date and Time format)<br/>
  **updated** Date of the last modification of the enterprise information (ISO 8601 Date and Time format)<br/>
  **id** Unique identifier of the enterprise (string)<br/>
  **name** Name of the enterprise (string)<br/>
  **contact name** Name of the contact in the enterprise (string)<br/>

left_code_blocks:
  - code_block: |-
      !API_URL!/enterprise/:id
    title:
    language: bash
right_request_blocks:
  - code_block: |1-
     !API_URL!/enterprise/11111111
    title: Example request
    language: bash
right_code_blocks:
  - code_block: |2-
      {
        "created": "2018-12-12T09:07:00.725Z",
        "updated": "2019-03-30T15:03:42.095Z",
        "id": "11111111",
        "name": "Test - Cable Company ABC",
        "contact": {
          "name": "Jane Doe"
        }
      }
    title: Example response
    language: json
---


