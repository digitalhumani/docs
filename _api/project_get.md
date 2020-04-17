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
  **id** Id of the reforestation project for which you want to get the details. Example of an id: 93333333  (Project Ids are 8 digits long). The complete list of available projects is listed in the Appendix&nbsp;1.

  Status: 200
  {: .success}

  Response will be an object that has the following attributes:
  
  **created** Creation date of the project in the RaaS database (ISO 8601 Date and Time format)<br/>
  **updated** Date of the last modification of the project information (ISO 8601 Date and Time format)<br/>
  **id** Unique identifier of the project (string)<br/>
  **name** Short name of the project, in English (deprecated) (string)<br/>
  **description** Short Description of the project, in English (deprecated) (string)<br/>
  **reforestationCompanyName_en** Name of the reforestation company in English (string)<br/>
  **reforestationCompanyName_fr** Name of the reforestation company in French (string)<br/>
  **reforestationCompanyAddress_en** Physical address of the reforestation company in English (string)<br/>
  **reforestationCompanyAddress_fr** Physical address of the reforestation company in French (string)<br/>
  **reforestationCompanyWebsite_en** Website address of the reforestation company in English (string)<br/>
  **reforestationCompanyWebsite_fr** Website address of the reforestation company in French (string)<br/>
  **reforestationProjectCountry_en** Country of the reforestation project in English (string)<br/>
  **reforestationProjectCountry_fr** Country of the reforestation project in French (string)<br/>
  **reforestationProjectDescription_en** Description of the reforestation project in English (string)<br/>
  **reforestationProjectDescription_fr** Description of the reforestation project in French (string)<br/>
  **reforestationProjectImageURL_en** Image URL of the reforestation project (in English when applicable) ( string)<br/>
  **reforestationProjectImageURL_fr** Image URL of the reforestation project (in French when applicable) ( string)<br/>
  **reforestationProjectState_en** State or province where the reforestation project is located in English ( string)<br/>
  **reforestationProjectState_fr** State or province where the reforestation project is located in French ( string)<br/>
  **reforestationProjectWebsite_en** Website address of the reforestation project in English (string)<br/>
  **reforestationProjectWebsite_fr** Website address of the reforestation project in French (string)
left_code_blocks:
  - code_block: |-
     https://api.digitalhumani.com/project/:id
    title:
    language: bash
right_request_blocks:
  - code_block: |1-
     https://api.digitalhumani.com/project/96666666
    title: Example request
    language: bash
right_code_blocks:
  - code_block: |2-
      {
        "reforestationCompanyName_fr": "WeForest",
        "reforestationProjectImageURL_en": "https://www.weforest.org/sites/IMG_20190423_132725_0.jpg",
        "reforestationCompanyName_en": "WeForest",
        "reforestationProjectCountry_en": "India",
        "reforestationCompanyAddress_en": "Ogentroostlaan 15, 3090 Overijse, Belgium",
        "created": "2018-12-12T09:05:00.725Z",
        "reforestationProjectWebsite_en": "https://www.weforest.org/project/india-khasi-hills",
        "name": "Khasi Hills in India, WeForest",
        "reforestationProjectWebsite_fr": "https://www.weforest.org/project/india-khasi-hills",
        "reforestationProjectCountry_fr": "Inde",
        "updated": "2019-05-19T19:24:10.761Z",
        "reforestationProjectDescription_fr": "Projet de reforestation aux Khasi Hills en Inde",
        "reforestationProjectDescription_en": "Reforestation project in the Khasi Hills in India",
        "reforestationCompanyWebsite_fr": "https://www.weforest.org/",
        "reforestationCompanyWebsite_en": "https://www.weforest.org/",
        "reforestationCompanyAddress_fr": "Ogentroostlaan 15, 3090 Overijse, Belgique",
        "description": "Khasi Hills in India, WeForest",
        "id": "96666666",
        "reforestationProjectImageURL_fr": "https://www.weforest.org/sites/default/IMG_20190423_132725_0.jpg"
      }
    title: Example response
    language: json
---