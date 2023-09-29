---
# NOTICE: Copyright 2023 Talend SA, Talend, Inc., and affiliates. All Rights Reserved. Customer’s use of the software contained herein is subject to the terms and conditions of the Agreement between Customer and Talend.
layout: "apiDefinition_1.1.0"
api-definition:
  specVersion: "4.1.0"
  info:
    name: "FrenchCodePostal"
    version: "1.0.0"
    description: "Aucune description"
    license: {}
    contact: {}
  contract:
    baseUrls:
    - url: "http://COSTAL01TSTP.tvhconsulting.local:8040/services/codePostal"
      isPublished: true
    mediaTypes:
    - "application/json"
    unsortedElementOrder:
    - "#/contract/resources/b2995f7f-0749-4910-82d4-d555e60b044f"
    - "#/contract/resources/19372d87-15a1-44bc-add7-d3fd9f4abc5e"
    - "#/contract/resources/f310d509-e6dc-4e58-a8d4-a805a75ee58a"
    - "#/contract/resources/93ad35cd-fcf1-4336-9122-09fe81f8a17e"
    resources:
      b2995f7f-0749-4910-82d4-d555e60b044f:
        path: "/getAll"
        operations:
          "6fba9a84-d3a0-4130-a9b1-5919fd954e33":
            name: "getAll"
            method: "GET"
      "19372d87-15a1-44bc-add7-d3fd9f4abc5e":
        path: "/getDepartement"
        operations:
          "77af4589-aa2a-412b-a7c5-d0e1d160ca78":
            name: "getDepartement"
            method: "GET"
      f310d509-e6dc-4e58-a8d4-a805a75ee58a:
        path: "/test"
        operations:
          abd9aa8c-e7a4-485a-99d1-7a1e822d4d9c:
            name: "test"
            method: "GET"
      "93ad35cd-fcf1-4336-9122-09fe81f8a17e":
        path: "/getVilleByCodePostal"
        operations:
          "4801f68d-43f6-4b22-9e70-7ac8c328e9b5":
            name: "getVileByCodePostal"
            method: "GET"
            queryParameters:
            - name: "CodePostal"
              type: "STRING"
              required: true
              examples:
              - value: "13010"
  components: {}
api-tryin: |-
  {
    "version" : 6,
    "entities" : [ {
      "entity" : {
        "type" : "Project",
        "name" : "FrenchCodePostal 1.0.0",
        "description" : "Aucune description",
        "importedFrom" : "03ca3caa-0415-43bf-9f61-c2c4c10f6058"
      },
      "children" : [ {
        "entity" : {
          "type" : "Request",
          "id" : "6fba9a84-d3a0-4130-a9b1-5919fd954e33",
          "name" : "getAll",
          "uri" : {
            "host" : "${\"BaseUrl\"}",
            "path" : "/getAll"
          },
          "method" : {
            "link" : "",
            "name" : "GET"
          },
          "headers" : [ ],
          "headersType" : "Form"
        }
      }, {
        "entity" : {
          "type" : "Request",
          "id" : "77af4589-aa2a-412b-a7c5-d0e1d160ca78",
          "name" : "getDepartement",
          "uri" : {
            "host" : "${\"BaseUrl\"}",
            "path" : "/getDepartement"
          },
          "method" : {
            "link" : "",
            "name" : "GET"
          },
          "headers" : [ ],
          "headersType" : "Form"
        }
      }, {
        "entity" : {
          "type" : "Request",
          "id" : "abd9aa8c-e7a4-485a-99d1-7a1e822d4d9c",
          "name" : "test",
          "uri" : {
            "host" : "${\"BaseUrl\"}",
            "path" : "/test"
          },
          "method" : {
            "link" : "",
            "name" : "GET"
          },
          "headers" : [ ],
          "headersType" : "Form"
        }
      }, {
        "entity" : {
          "type" : "Request",
          "id" : "4801f68d-43f6-4b22-9e70-7ac8c328e9b5",
          "name" : "getVileByCodePostal",
          "uri" : {
            "host" : "${\"BaseUrl\"}",
            "path" : "/getVilleByCodePostal",
            "query" : {
              "delimiter" : "&",
              "items" : [ {
                "name" : "CodePostal",
                "value" : "13010",
                "enabled" : true
              } ]
            }
          },
          "method" : {
            "link" : "",
            "name" : "GET"
          },
          "headers" : [ ],
          "headersType" : "Form",
          "uriEditor" : true
        }
      } ]
    } ],
    "environments" : [ {
      "name" : "FrenchCodePostal 1.0.0",
      "importedFrom" : {
        "projectId" : "03ca3caa-0415-43bf-9f61-c2c4c10f6058"
      },
      "variables" : {
        "12499d4b-9130-4429-a6ba-a84ecfeaa0c8" : {
          "name" : "BaseUrl",
          "value" : "http://COSTAL01TSTP.tvhconsulting.local:8040/services/codePostal",
          "enabled" : true,
          "private" : false
        }
      }
    } ]
  }
---
