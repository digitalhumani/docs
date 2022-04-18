---
title: /user/whoami
position_number: 0.9
type: get
description: Get Authenticated User
content_markdown_method: |-
  The following method allows you to retrieve the details of your authenticated user.
content_markdown: |-
  Status: 200
  {: .success}

  Response will be an object containing the details of your authenicated user, including internal user ID, user name and email, and ID of user's associated enterprise (`enterpriseId`).

left_code_blocks:
  - code_block: |-
      https://api.digitalhumani.com/user/whoami
    title:
    language: bash
right_request_blocks:
  - code_block: |1-
     https://api.digitalhumani.com/user/whoami
    title: Example request
    language: bash
right_code_blocks:
  - code_block: |2-
      {
          "id": "abcd1234",
          "email": "test@test.com",
          "firstName": "Test",
          "lastName": "User",
          "enterpriseId": "1111111"
      }
    title: Example response
    language: json
---
