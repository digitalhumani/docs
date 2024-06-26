---
title: /project
position_number: 1.1
type: get
description: Get list of all Projects
content_markdown_method: |-
  The following method retrieves all the reforestation projects available.  The complete list of available projects is listed in the Appendix&nbsp;1.
parameters:
  - name:
    content:
content_markdown: |-
  Status: 200
  {: .success}

  Response will be an array of objects representing each project. The projects have the following attributes:

  - **id** - Unique identifier of the project (string)<br/>
  - **name** - Short name of the project (string)<br/>
  - **active** - Indicator of project's active/inactive status (boolean)<br/>
  - **reforestationProjectDescription_en** - Description of the reforestation project (string)<br/>
  - **reforestationProjectState_en** - State or province where the reforestation project is located (string)<br/>
  - **reforestationProjectCountry_en** - Country of the reforestation project (string)<br/>
  - **reforestationProjectWebsite_en** - Website address of the reforestation project (string)<br/>
  - **reforestationCompanyName_en** - Name of the reforestation organization managing the project (string)<br/>

  If you are looking for more information on each project, please see [`GET /project/:id`](#apiproject_get). Note that `_en` indicates the English language version of the attributes

left_code_blocks:
  - code_block: |-
      https://api.digitalhumani.com/project
    title:
    language: bash
right_request_blocks:
  - code_block: |1-
     https://api.digitalhumani.com/project
    title: Example request
    language: bash
right_code_blocks:
  - code_block: |2-
      [
        { 
          "id": "44116666",
          "name": "Africa OneTreePlanted",
          "active": true,
          "reforestationProjectDescription_en": "Reforestation projects in Africa",
          "reforestationProjectCountry_en": "Africa",
          "reforestationProjectWebsite_en": "https://onetreeplanted.org/collections/africa",
          "reforestationCompanyName_en": "OneTreePlanted",
          
        },
        {
          "id": "52223885",
          "name": "Belize SustainableHarvest",
          "active": true,
          "reforestationProjectDescription_en": "Reforestation project in Belize",
          "reforestationProjectCountry_en": "Belize",
          "reforestationProjectWebsite_en": "https://www.sustainableharvest.org/programs",
          "reforestationCompanyName_en": "Sustainable Harvest International",
        }
      ]
    title: Example response (with 2 reforestation projects included)
    language: json
---
