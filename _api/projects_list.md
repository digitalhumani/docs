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

  Response will be an object, which is an array of all the projects. The projects have the following attributes:

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
  **reforestationProjectDescription_en** Description of the reforestation project in English (string<br/>
  **reforestationProjectDescription_fr** Description of the reforestation project in French (string)<br/>
  **reforestationProjectImageURL_en** Image URL of the reforestation project (in English when applicable) ( string)<br/>
  **reforestationProjectImageURL_fr** Image URL of the reforestation project (in French when applicable) ( string)<br/>
  **reforestationProjectState_en** State or province where the reforestation project is located in English ( string)<br/>
  **reforestationProjectState_fr** State or province where the reforestation project is located in French ( string)<br/>
  **reforestationProjectWebsite_en** Website address of the reforestation project in English (string)<br/>
  **reforestationProjectWebsite_fr** Website address of the reforestation project in French (string)
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
            "reforestationCompanyName_fr": "OneTreePlanted",
            "reforestationProjectImageURL_en": "https://cdn.shopify.com/1/products/California_One_Tree_Planted.png",
            "reforestationCompanyName_en": "OneTreePlanted",
            "reforestationProjectCountry_en": "United States",
            "reforestationCompanyAddress_en": "145 Pine Haven Shores Rd #1000D Shelburne, Vermont, 05482, USA",
            "created": "2018-11-17T09:06:00.725Z",
            "reforestationProjectWebsite_en": "https://onetreeplanted.org/united-states/products/california-forests",
            "name": "California OneTreePlanted",
            "reforestationProjectState_fr": "Californie",
            "reforestationProjectWebsite_fr": "https://onetreeplanted.org/united-states/products/california-forests",
            "reforestationProjectCountry_fr": "États-Unis",
            "reforestationProjectState_en": "California",
            "updated": "2019-05-19T19:19:26.180Z",
            "reforestationProjectDescription_fr": "Projet de reforestation en Californie, États-Unis",
            "reforestationProjectDescription_en": "Reforestation project in California, United States",
            "reforestationCompanyWebsite_fr": "https://onetreeplanted.org/",
            "reforestationCompanyWebsite_en": "https://onetreeplanted.org/",
            "reforestationCompanyAddress_fr": "145 Pine Haven Shores Rd #1000D Shelburne, Vermont, 05482, USA",
            "description": "California OneTreePlanted",
            "id": "91111111",
            "reforestationProjectImageURL_fr": "https://cdn.shopify.com/s/files/California_One_Tree_Planted.png"
          },
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
        ]
    title: Example response (with 2 reforestation projects included)
    language: json
---