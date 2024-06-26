---
title: /project/:id
position_number: 1.2
type: get
description: Get Project by ID
content_markdown_method: |-
  The following method allows you to retrieve the details of a single reforestation project.
parameters:
  - name: URL_PARAM
    content: id
    values: string
content_markdown: |-
  **id** Id of the reforestation project for which you want to get the details. Example of an id: 44116666  (Project Ids are 8 digits long). You can find a [complete list of available projects](#appendixlist-of-projects) listed in the Appendix.

  Status: 200
  {: .success}

  Response will be an object that has the following attributes:

  - **created** - Creation date of the project in the RaaS database (ISO 8601 Date and Time format)<br/>
  - **updated** - Date of the last modification of the project information (ISO 8601 Date and Time format)<br/>
  - **id** - Unique identifier of the project (string)<br/>
  - **name** - Short name of the project, in English (deprecated) (string)<br/>
  - **active** - Indicator of project's active/inactive status (boolean)<br/>
  - **description** - Short Description of the project, in English (deprecated) (string)<br/>
  - **reforestationCompanyName_en** - Name of the reforestation company in English (string)<br/>
  - **reforestationCompanyName_fr** - Name of the reforestation company in French (string)<br/>
  - **reforestationCompanyAddress_en** - Physical address of the reforestation company in English (string)<br/>
  - **reforestationCompanyAddress_fr** - Physical address of the reforestation company in French (string)<br/>
  - **reforestationCompanyWebsite_en** - Website address of the reforestation company in English (string)<br/>
  - **reforestationCompanyWebsite_fr** - Website address of the reforestation company in French (string)<br/>
  - **reforestationProjectCountry_en** - Country of the reforestation project in English (string)<br/>
  - **reforestationProjectCountry_fr** - Country of the reforestation project in French (string)<br/>
  - **reforestationProjectDescription_en** - Description of the reforestation project in English (string)<br/>
  - **reforestationProjectDescription_fr** - Description of the reforestation project in French (string)<br/>
  - **reforestationProjectImageURL_en** - Image URL of the reforestation project (in English when applicable) (string)<br/>
  - **reforestationProjectImageURL_fr** - Image URL of the reforestation project (in French when applicable) (string)<br/>
  - **reforestationProjectState_en** - State or province where the reforestation project is located in English (string)<br/>
  - **reforestationProjectState_fr** - State or province where the reforestation project is located in French (string)<br/>
  - **reforestationProjectWebsite_en** - Website address of the reforestation project in English (string)<br/>
  - **reforestationProjectWebsite_fr** - Website address of the reforestation project in French (string)

left_code_blocks:
  - code_block: |-
      https://api.digitalhumani.com/project/:id
    title:
    language: bash
right_request_blocks:
  - code_block: |1-
     https://api.digitalhumani.com/project/44116666
    title: Example request
    language: bash
right_code_blocks:
  - code_block: |2-
      {
          "id": "44116666",
          "name": "Africa OneTreePlanted",
          "active": true,
          "description": "Africa OneTreePlanted",
          "reforestationCompanyName_fr": "OneTreePlanted",
          "reforestationProjectImageURL_en": "",
          "reforestationCompanyName_en": "OneTreePlanted",
          "reforestationProjectCountry_en": "Africa",
          "reforestationCompanyAddress_en": "145 Pine Haven Shores Rd #1000D Shelburne, Vermont, 05482, USA",
          "created": "2024-05-23T09:05:00.725Z",
          "reforestationProjectWebsite_en": "https://onetreeplanted.org/collections/africa",
          "reforestationProjectWebsite_fr": "https://onetreeplanted.org/collections/africa",
          "reforestationProjectCountry_fr": "Afrique",
          "location_en": "Africa",
          "updated": "2024-05-23T19:21:44.646Z",
          "reforestationProjectDescription_fr": "Projets de reforestation en Afrique",
          "reforestationProjectDescription_en": "Reforestation projects in Africa",
          "reforestationCompanyWebsite_fr": "https://onetreeplanted.org/",
          "reforestationCompanyWebsite_en": "https://onetreeplanted.org/",
          "reforestationCompanyAddress_fr": "145 Pine Haven Shores Rd #1000D Shelburne, Vermont, 05482, USA",
          "reforestationProjectImageURL_fr": ""
      }
    title: Example Response
    language: json
---
