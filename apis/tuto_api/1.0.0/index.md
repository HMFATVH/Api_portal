---
# NOTICE: Copyright 2023 Talend SA, Talend, Inc., and affiliates. All Rights Reserved. Customer’s use of the software contained herein is subject to the terms and conditions of the Agreement between Customer and Talend.
layout: "apiDefinition_1.1.0"
api-definition:
  specVersion: "4.1.0"
  info:
    name: "tuto_API"
    version: "1.0.0"
    description: "Aucune description"
  contract:
    mediaTypes:
    - "application/json"
  components: {}
api-tryin: |-
  {
    "version" : 6,
    "entities" : [ {
      "entity" : {
        "type" : "Project",
        "name" : "tuto_API 1.0.0",
        "description" : "Aucune description",
        "importedFrom" : "e9902b56-9a9c-48b8-87a9-104ab3c176d6"
      }
    } ],
    "environments" : [ {
      "name" : "tuto_API 1.0.0",
      "importedFrom" : {
        "projectId" : "e9902b56-9a9c-48b8-87a9-104ab3c176d6"
      },
      "variables" : {
        "fa4ac806-079d-4fb5-a24c-504e9b245ee9" : {
          "name" : "BaseUrl",
          "value" : "https://example.com",
          "enabled" : true,
          "private" : false
        }
      }
    } ]
  }
---
