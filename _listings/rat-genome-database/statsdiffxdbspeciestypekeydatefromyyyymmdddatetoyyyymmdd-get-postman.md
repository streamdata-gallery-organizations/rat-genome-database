{
  "info": {
    "name": "Rat Genome Database Count difference of external database ids, for specified species and date range",
    "_postman_id": "65cd8df5-2836-416c-b469-2de72782570a",
    "description": "",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "id": "11d2363e-e263-4833-885b-e064ad22b113",
      "name": "getTermAccIdsUsingGET",
      "request": {
        "url": {
          "protocol": "http",
          "host": "rest.rgd.mcw.edu",
          "path": [
            "rgdws",
            "annotations/accId/:rgdId"
          ],
          "variable": [
            {
              "id": "rgdId",
              "value": "{}",
              "type": "string"
            }
          ]
        },
        "method": "GET",
        "header": [
          {
            "key": "Accept",
            "value": "*/*",
            "disabled": false
          }
        ],
        "body": {
          "mode": "raw"
        },
        "description": "Returns a list ontology term accession IDs annotated to an rgd object"
      },
      "response": [
        {
          "status": "OK",
          "code": 200,
          "name": "Response_200",
          "id": "24d0c871-f415-4dd9-888f-42ebb410521c"
        }
      ]
    },
    {
      "id": "046536f5-e689-46d5-aad7-8ee6144b6d34",
      "name": "getAnnotationCountByAccIdUsingGET",
      "request": {
        "url": {
          "protocol": "http",
          "host": "rest.rgd.mcw.edu",
          "path": [
            "rgdws",
            "annotations/count/:accId/:includeChildren"
          ],
          "variable": [
            {
              "id": "accId",
              "value": "{}",
              "type": "string"
            },
            {
              "id": "includeChildren",
              "value": "{}",
              "type": "string"
            }
          ]
        },
        "method": "GET",
        "header": [
          {
            "key": "Accept",
            "value": "*/*",
            "disabled": false
          }
        ],
        "body": {
          "mode": "raw"
        },
        "description": "Returns annotation count for ontology accession ID"
      },
      "response": [
        {
          "status": "OK",
          "code": 200,
          "name": "Response_200",
          "id": "3723c526-6213-4d30-97ac-f92f9cf6b0ea"
        }
      ]
    },
    {
      "id": "31f6d826-0bde-4706-b236-6f1bed512744",
      "name": "getAnnotationCountByAccIdAndSpeciesUsingGET",
      "request": {
        "url": {
          "protocol": "http",
          "host": "rest.rgd.mcw.edu",
          "path": [
            "rgdws",
            "annotations/count/:accId/:speciesTypeKey/:includeChildren"
          ],
          "variable": [
            {
              "id": "accId",
              "value": "{}",
              "type": "string"
            },
            {
              "id": "includeChildren",
              "value": "{}",
              "type": "string"
            },
            {
              "id": "speciesTypeKey",
              "value": "{}",
              "type": "string"
            }
          ]
        },
        "method": "GET",
        "header": [
          {
            "key": "Accept",
            "value": "*/*",
            "disabled": false
          }
        ],
        "body": {
          "mode": "raw"
        },
        "description": "Returns annotation count for ontology accession ID and speicies"
      },
      "response": [
        {
          "status": "OK",
          "code": 200,
          "name": "Response_200",
          "id": "2dff09c9-1067-4739-962d-0dea9228e78a"
        }
      ]
    },
    {
      "id": "5ae0a143-70e5-40a9-8f91-86a99ac68248",
      "name": "getAnnotationCountByAccIdAndObjectTypeUsingGET",
      "request": {
        "url": {
          "protocol": "http",
          "host": "rest.rgd.mcw.edu",
          "path": [
            "rgdws",
            "annotations/count/:accId/:speciesTypeKey/:includeChildren/:objectType"
          ],
          "variable": [
            {
              "id": "accId",
              "value": "{}",
              "type": "string"
            },
            {
              "id": "includeChildren",
              "value": "{}",
              "type": "string"
            },
            {
              "id": "objectType",
              "value": "{}",
              "type": "string"
            },
            {
              "id": "speciesTypeKey",
              "value": "{}",
              "type": "string"
            }
          ]
        },
        "method": "GET",
        "header": [
          {
            "key": "Accept",
            "value": "*/*",
            "disabled": false
          }
        ],
        "body": {
          "mode": "raw"
        },
        "description": "Returns annotation count for ontology accession ID and object type"
      },
      "response": [
        {
          "status": "OK",
          "code": 200,
          "name": "Response_200",
          "id": "49df6a94-0d6a-47b2-9cec-38bae194414c"
        }
      ]
    },
    {
      "id": "e0a8796c-94b8-4cc3-a8d5-d03990ab9c7a",
      "name": "getAnnotsByRefrerenceUsingGET",
      "request": {
        "url": {
          "protocol": "http",
          "host": "rest.rgd.mcw.edu",
          "path": [
            "rgdws",
            "annotations/reference/:refRgdId"
          ],
          "variable": [
            {
              "id": "refRgdId",
              "value": "{}",
              "type": "string"
            }
          ]
        },
        "method": "GET",
        "header": [
          {
            "key": "Accept",
            "value": "*/*",
            "disabled": false
          }
        ],
        "body": {
          "mode": "raw"
        },
        "description": "Returns a list of annotations for a reference"
      },
      "response": [
        {
          "status": "OK",
          "code": 200,
          "name": "Response_200",
          "id": "39e234a0-73e3-47ea-8dfa-bd68467a52a9"
        }
      ]
    },
    {
      "id": "c8f5cf9f-cb47-4f9a-83ef-e1e2a1f1a5b1",
      "name": "getAnnotationsByRgdIdUsingGET",
      "request": {
        "url": {
          "protocol": "http",
          "host": "rest.rgd.mcw.edu",
          "path": [
            "rgdws",
            "annotations/rgdId/:rgdId"
          ],
          "variable": [
            {
              "id": "rgdId",
              "value": "{}",
              "type": "string"
            }
          ]
        },
        "method": "GET",
        "header": [
          {
            "key": "Accept",
            "value": "*/*",
            "disabled": false
          }
        ],
        "body": {
          "mode": "raw"
        },
        "description": "Returns a list of annotations by RGD ID"
      },
      "response": [
        {
          "status": "OK",
          "code": 200,
          "name": "Response_200",
          "id": "4bdb1ed1-eeeb-4afd-a47b-3ebe6ad1289d"
        }
      ]
    },
    {
      "id": "bb554e78-f526-4730-b2d1-f0d6f53af403",
      "name": "getAnnotationsByRgdIdAndOntologyUsingGET",
      "request": {
        "url": {
          "protocol": "http",
          "host": "rest.rgd.mcw.edu",
          "path": [
            "rgdws",
            "annotations/rgdId/:rgdId/:ontologyPrefix"
          ],
          "variable": [
            {
              "id": "ontologyPrefix",
              "value": "{}",
              "type": "string"
            },
            {
              "id": "rgdId",
              "value": "{}",
              "type": "string"
            }
          ]
        },
        "method": "GET",
        "header": [
          {
            "key": "Accept",
            "value": "*/*",
            "disabled": false
          }
        ],
        "body": {
          "mode": "raw"
        },
        "description": "Returns a list of annotations by RGD ID and ontology prefix"
      },
      "response": [
        {
          "status": "OK",
          "code": 200,
          "name": "Response_200",
          "id": "cbc7f889-cc11-4305-b262-31909599bd1b"
        }
      ]
    },
    {
      "id": "56ee5e27-9b3c-428d-9c9d-8b150fd30a3c",
      "name": "getAnnotationsByAccIdAndRgdIdUsingGET",
      "request": {
        "url": {
          "protocol": "http",
          "host": "rest.rgd.mcw.edu",
          "path": [
            "rgdws",
            "annotations/:accId/:rgdId"
          ],
          "variable": [
            {
              "id": "accId",
              "value": "{}",
              "type": "string"
            },
            {
              "id": "rgdId",
              "value": "{}",
              "type": "string"
            }
          ]
        },
        "method": "GET",
        "header": [
          {
            "key": "Accept",
            "value": "*/*",
            "disabled": false
          }
        ],
        "body": {
          "mode": "raw"
        },
        "description": "Returns a list of annotations by RGD ID and ontology term accession ID"
      },
      "response": [
        {
          "status": "OK",
          "code": 200,
          "name": "Response_200",
          "id": "01006859-fc1a-44c3-bd11-cd400d8a3336"
        }
      ]
    },
    {
      "id": "a1d406fc-3a6b-4934-94d2-17f38f0193ef",
      "name": "getAnnotationsUsingGET",
      "request": {
        "url": {
          "protocol": "http",
          "host": "rest.rgd.mcw.edu",
          "path": [
            "rgdws",
            "annotations/:accId/:speciesTypeKey/:includeChildren"
          ],
          "variable": [
            {
              "id": "accId",
              "value": "{}",
              "type": "string"
            },
            {
              "id": "includeChildren",
              "value": "{}",
              "type": "string"
            },
            {
              "id": "speciesTypeKey",
              "value": "{}",
              "type": "string"
            }
          ]
        },
        "method": "GET",
        "header": [
          {
            "key": "Accept",
            "value": "*/*",
            "disabled": false
          }
        ],
        "body": {
          "mode": "raw"
        },
        "description": "Returns a list annotations for an ontology term or a term and it's children"
      },
      "response": [
        {
          "status": "OK",
          "code": 200,
          "name": "Response_200",
          "id": "2e11ade8-c171-4b41-b36e-1a199cd528a0"
        }
      ]
    },
    {
      "id": "5f7e9e1d-db6a-4087-b879-0049f294db84",
      "name": "getGenesByAffyIdUsingGET",
      "request": {
        "url": {
          "protocol": "http",
          "host": "rest.rgd.mcw.edu",
          "path": [
            "rgdws",
            "genes/affyId/:affyId/:speciesTypeKey"
          ],
          "variable": [
            {
              "id": "affyId",
              "value": "{}",
              "type": "string"
            },
            {
              "id": "speciesTypeKey",
              "value": "{}",
              "type": "string"
            }
          ]
        },
        "method": "GET",
        "header": [
          {
            "key": "Accept",
            "value": "*/*",
            "disabled": false
          }
        ],
        "body": {
          "mode": "raw"
        },
        "description": "Return a list of genes for an affymetrix ID"
      },
      "response": [
        {
          "status": "OK",
          "code": 200,
          "name": "Response_200",
          "id": "fc6f63f1-2175-4ec3-bf7c-51b0cf2ae262"
        }
      ]
    },
    {
      "id": "2f3364b7-015c-4d58-beb3-6ced8fb8d69a",
      "name": "getGenesByAliasSymbolUsingGET",
      "request": {
        "url": {
          "protocol": "http",
          "host": "rest.rgd.mcw.edu",
          "path": [
            "rgdws",
            "genes/alias/:aliasSymbol/:speciesTypeKey"
          ],
          "variable": [
            {
              "id": "aliasSymbol",
              "value": "{}",
              "type": "string"
            },
            {
              "id": "speciesTypeKey",
              "value": "{}",
              "type": "string"
            }
          ]
        },
        "method": "GET",
        "header": [
          {
            "key": "Accept",
            "value": "*/*",
            "disabled": false
          }
        ],
        "body": {
          "mode": "raw"
        },
        "description": "Return a list of genes for an alias and species"
      },
      "response": [
        {
          "status": "OK",
          "code": 200,
          "name": "Response_200",
          "id": "b7fe0605-5a78-473a-9f62-16aff8d16e85"
        }
      ]
    },
    {
      "id": "99ce74ac-738d-4ae1-9dcd-f50d3e8d9fcc",
      "name": "getGeneAllelesUsingGET",
      "request": {
        "url": {
          "protocol": "http",
          "host": "rest.rgd.mcw.edu",
          "path": [
            "rgdws",
            "genes/allele/:rgdId"
          ],
          "variable": [
            {
              "id": "rgdId",
              "value": "{}",
              "type": "string"
            }
          ]
        },
        "method": "GET",
        "header": [
          {
            "key": "Accept",
            "value": "*/*",
            "disabled": false
          }
        ],
        "body": {
          "mode": "raw"
        },
        "description": "Return a list of gene alleles"
      },
      "response": [
        {
          "status": "OK",
          "code": 200,
          "name": "Response_200",
          "id": "c64910c2-8a2c-40b3-9e9a-2af34654333c"
        }
      ]
    },
    {
      "id": "496fe502-169d-484d-8868-b952ec953d37",
      "name": "getGenesAnnotatedUsingGET",
      "request": {
        "url": {
          "protocol": "http",
          "host": "rest.rgd.mcw.edu",
          "path": [
            "rgdws",
            "genes/annotation/:accId/:speciesTypeKey"
          ],
          "variable": [
            {
              "id": "accId",
              "value": "{}",
              "type": "string"
            },
            {
              "id": "speciesTypeKey",
              "value": "{}",
              "type": "string"
            }
          ]
        },
        "method": "GET",
        "header": [
          {
            "key": "Accept",
            "value": "*/*",
            "disabled": false
          }
        ],
        "body": {
          "mode": "raw"
        },
        "description": "Return a list of genes annotated to an ontology term"
      },
      "response": [
        {
          "status": "OK",
          "code": 200,
          "name": "Response_200",
          "id": "662eaa3e-2d47-45fa-aacb-fc91bf55aa18"
        }
      ]
    },
    {
      "id": "24a9ba1a-5efa-4d63-a3fe-27667c880b5c",
      "name": "getGenesByKeywordUsingGET",
      "request": {
        "url": {
          "protocol": "http",
          "host": "rest.rgd.mcw.edu",
          "path": [
            "rgdws",
            "genes/keyword/:keyword/:speciesTypeKey"
          ],
          "variable": [
            {
              "id": "keyword",
              "value": "{}",
              "type": "string"
            },
            {
              "id": "speciesTypeKey",
              "value": "{}",
              "type": "string"
            }
          ]
        },
        "method": "GET",
        "header": [
          {
            "key": "Accept",
            "value": "*/*",
            "disabled": false
          }
        ],
        "body": {
          "mode": "raw"
        },
        "description": "Return a list of genes by keyword and species type key"
      },
      "response": [
        {
          "status": "OK",
          "code": 200,
          "name": "Response_200",
          "id": "1aa76322-4989-4347-b421-1f92f1f15417"
        }
      ]
    },
    {
      "id": "3d160109-bf7a-4438-afbd-bc3a3d45fc63",
      "name": "getGeneByMapKeyUsingGET",
      "request": {
        "url": {
          "protocol": "http",
          "host": "rest.rgd.mcw.edu",
          "path": [
            "rgdws",
            "genes/map/:mapKey"
          ],
          "variable": [
            {
              "id": "mapKey",
              "value": "{}",
              "type": "string"
            }
          ]
        },
        "method": "GET",
        "header": [
          {
            "key": "Accept",
            "value": "*/*",
            "disabled": false
          }
        ],
        "body": {
          "mode": "raw"
        },
        "description": "Return a list of all genes with position information for an assembly"
      },
      "response": [
        {
          "status": "OK",
          "code": 200,
          "name": "Response_200",
          "id": "14c09cf1-b2cf-469b-a604-867d3cc5963f"
        }
      ]
    },
    {
      "id": "558495e2-e780-42a1-999d-adc6dc68087b",
      "name": "getGeneOrthologsUsingGET",
      "request": {
        "url": {
          "protocol": "http",
          "host": "rest.rgd.mcw.edu",
          "path": [
            "rgdws",
            "genes/ortholog/:rgdId"
          ],
          "variable": [
            {
              "id": "rgdId",
              "value": "{}",
              "type": "string"
            }
          ]
        },
        "method": "GET",
        "header": [
          {
            "key": "Accept",
            "value": "*/*",
            "disabled": false
          }
        ],
        "body": {
          "mode": "raw"
        },
        "description": "Return a list of gene orthologs"
      },
      "response": [
        {
          "status": "OK",
          "code": 200,
          "name": "Response_200",
          "id": "b5b4fa3c-b623-41d0-87ac-591a287632cd"
        }
      ]
    },
    {
      "id": "12fbcc2b-7d9c-4f74-b496-3d6e8ea69daf",
      "name": "getGenesBySpeciesUsingGET",
      "request": {
        "url": {
          "protocol": "http",
          "host": "rest.rgd.mcw.edu",
          "path": [
            "rgdws",
            "genes/species/:speciesTypeKey"
          ],
          "variable": [
            {
              "id": "speciesTypeKey",
              "value": "{}",
              "type": "string"
            }
          ]
        },
        "method": "GET",
        "header": [
          {
            "key": "Accept",
            "value": "*/*",
            "disabled": false
          }
        ],
        "body": {
          "mode": "raw"
        },
        "description": "Return a list of all genes for a species in RGD"
      },
      "response": [
        {
          "status": "OK",
          "code": 200,
          "name": "Response_200",
          "id": "7865ea2f-e6ed-4801-b64e-8f0088890b28"
        }
      ]
    },
    {
      "id": "5b06fb61-8512-4ab3-8fb6-f0fbe52e491d",
      "name": "getGenesByPositionUsingGET",
      "request": {
        "url": {
          "protocol": "http",
          "host": "rest.rgd.mcw.edu",
          "path": [
            "rgdws",
            "genes/:chr/:start/:stop/:mapKey"
          ],
          "variable": [
            {
              "id": "chr",
              "value": "{}",
              "type": "string"
            },
            {
              "id": "mapKey",
              "value": "{}",
              "type": "string"
            },
            {
              "id": "start",
              "value": "{}",
              "type": "string"
            },
            {
              "id": "stop",
              "value": "{}",
              "type": "string"
            }
          ]
        },
        "method": "GET",
        "header": [
          {
            "key": "Accept",
            "value": "*/*",
            "disabled": false
          }
        ],
        "body": {
          "mode": "raw"
        },
        "description": "Return a list of genes position and map key"
      },
      "response": [
        {
          "status": "OK",
          "code": 200,
          "name": "Response_200",
          "id": "3343f0aa-eb78-4219-99ea-f3f4def03e41"
        }
      ]
    },
    {
      "id": "e6dcd635-1b7a-4e11-bc53-f375563155ec",
      "name": "getGeneByRgdIdUsingGET",
      "request": {
        "url": {
          "protocol": "http",
          "host": "rest.rgd.mcw.edu",
          "path": [
            "rgdws",
            "genes/:rgdId"
          ],
          "variable": [
            {
              "id": "rgdId",
              "value": "{}",
              "type": "string"
            }
          ]
        },
        "method": "GET",
        "header": [
          {
            "key": "Accept",
            "value": "*/*",
            "disabled": false
          }
        ],
        "body": {
          "mode": "raw"
        },
        "description": "Get a gene record by RGD ID"
      },
      "response": [
        {
          "status": "OK",
          "code": 200,
          "name": "Response_200",
          "id": "fa69855b-b9ea-4421-ab8d-e0aa9a672846"
        }
      ]
    },
    {
      "id": "cf7c923b-8577-4752-8080-1370703e2f42",
      "name": "getGeneBySymbolUsingGET",
      "request": {
        "url": {
          "protocol": "http",
          "host": "rest.rgd.mcw.edu",
          "path": [
            "rgdws",
            "genes/:symbol/:speciesTypeKey"
          ],
          "variable": [
            {
              "id": "speciesTypeKey",
              "value": "{}",
              "type": "string"
            },
            {
              "id": "symbol",
              "value": "{}",
              "type": "string"
            }
          ]
        },
        "method": "GET",
        "header": [
          {
            "key": "Accept",
            "value": "*/*",
            "disabled": false
          }
        ],
        "body": {
          "mode": "raw"
        },
        "description": "Get a gene record by symbol and species type key"
      },
      "response": [
        {
          "status": "OK",
          "code": 200,
          "name": "Response_200",
          "id": "5f3cde0a-d839-49c3-a9ed-ca85496cfb40"
        }
      ]
    },
    {
      "id": "aa478800-4c40-410f-b733-734df14444c6",
      "name": "getGeneTypesUsingGET",
      "request": {
        "url": "http://rest.rgd.mcw.edu/rgdws/lookup/geneTypes",
        "method": "GET",
        "header": [
          {
            "key": "Accept",
            "value": "*/*",
            "disabled": false
          }
        ],
        "body": {
          "mode": "raw"
        },
        "description": "Returns a list of gene types avialable in RGD"
      },
      "response": [
        {
          "status": "OK",
          "code": 200,
          "name": "Response_200",
          "id": "4449c8b0-7eb0-4e5c-b84f-f407ad44880a"
        }
      ]
    },
    {
      "id": "630a518b-ab15-403e-9d52-2f1984b73c72",
      "name": "getMapsUsingGET",
      "request": {
        "url": {
          "protocol": "http",
          "host": "rest.rgd.mcw.edu",
          "path": [
            "rgdws",
            "lookup/maps/:speciesTypeKey"
          ],
          "variable": [
            {
              "id": "speciesTypeKey",
              "value": "{}",
              "type": "string"
            }
          ]
        },
        "method": "GET",
        "header": [
          {
            "key": "Accept",
            "value": "*/*",
            "disabled": false
          }
        ],
        "body": {
          "mode": "raw"
        },
        "description": "Return a list assembly maps for a species"
      },
      "response": [
        {
          "status": "OK",
          "code": 200,
          "name": "Response_200",
          "id": "e7960302-f2fe-4bf5-80ce-42c308a4ae3b"
        }
      ]
    },
    {
      "id": "ccfc373d-3690-4a3d-8c6f-84575e001cd9",
      "name": "getSpeciesTypesUsingGET",
      "request": {
        "url": "http://rest.rgd.mcw.edu/rgdws/lookup/speciesTypeKeys",
        "method": "GET",
        "header": [
          {
            "key": "Accept",
            "value": "*/*",
            "disabled": false
          }
        ],
        "body": {
          "mode": "raw"
        },
        "description": "Return a Map of species type keys available in RGD"
      },
      "response": [
        {
          "status": "OK",
          "code": 200,
          "name": "Response_200",
          "id": "3ea40350-42e1-4cc3-83f6-b89d0a1977f2"
        }
      ]
    },
    {
      "id": "e3d6b098-c43a-4d2c-931f-b8b18415ac60",
      "name": "searchPathwaysUsingGET",
      "request": {
        "url": {
          "protocol": "http",
          "host": "rest.rgd.mcw.edu",
          "path": [
            "rgdws",
            "pathways/diagrams/search/:searchString"
          ],
          "variable": [
            {
              "id": "searchString",
              "value": "{}",
              "type": "string"
            }
          ]
        },
        "method": "GET",
        "header": [
          {
            "key": "Accept",
            "value": "*/*",
            "disabled": false
          }
        ],
        "body": {
          "mode": "raw"
        },
        "description": "Return a list of pathways based on search term"
      },
      "response": [
        {
          "status": "OK",
          "code": 200,
          "name": "Response_200",
          "id": "297d2e5f-6615-46ed-88e1-5c1b61fdda7e"
        }
      ]
    },
    {
      "id": "20efae37-f1ce-49ef-a62a-3e87d9bf8596",
      "name": "getPathwaysWithDiagramsForCategoryUsingGET",
      "request": {
        "url": {
          "protocol": "http",
          "host": "rest.rgd.mcw.edu",
          "path": [
            "rgdws",
            "pathways/diagramsForCategory/:category"
          ],
          "variable": [
            {
              "id": "category",
              "value": "{}",
              "type": "string"
            }
          ]
        },
        "method": "GET",
        "header": [
          {
            "key": "Accept",
            "value": "*/*",
            "disabled": false
          }
        ],
        "body": {
          "mode": "raw"
        },
        "description": "Return a list of pathways based on category provided"
      },
      "response": [
        {
          "status": "OK",
          "code": 200,
          "name": "Response_200",
          "id": "3cf77f5b-8e7d-426e-ac81-451ece6400ad"
        }
      ]
    },
    {
      "id": "b558c072-6268-4f89-be50-b57388ea517a",
      "name": "getChartInfoUsingGET",
      "request": {
        "url": {
          "protocol": "http",
          "host": "rest.rgd.mcw.edu",
          "path": [
            "rgdws",
            "phenotype/phenominer/chart/:speciesTypeKey/:termString"
          ],
          "variable": [
            {
              "id": "speciesTypeKey",
              "value": "{}",
              "type": "string"
            },
            {
              "id": "termString",
              "value": "{}",
              "type": "string"
            }
          ]
        },
        "method": "GET",
        "header": [
          {
            "key": "Accept",
            "value": "*/*",
            "disabled": false
          }
        ],
        "body": {
          "mode": "raw"
        },
        "description": "Return a list of pathways based on search term and species type.  3=rat 4=chinchilla"
      },
      "response": [
        {
          "status": "OK",
          "code": 200,
          "name": "Response_200",
          "id": "97702d35-2df6-461d-940f-f02cee3fce50"
        }
      ]
    },
    {
      "id": "13738fab-e350-4e3d-84b9-547dca71ae94",
      "name": "getQtlListByPositionUsingGET",
      "request": {
        "url": {
          "protocol": "http",
          "host": "rest.rgd.mcw.edu",
          "path": [
            "rgdws",
            "qtls/:chr/:start/:stop/:mapKey"
          ],
          "variable": [
            {
              "id": "chr",
              "value": "{}",
              "type": "string"
            },
            {
              "id": "mapKey",
              "value": "{}",
              "type": "string"
            },
            {
              "id": "start",
              "value": "{}",
              "type": "string"
            },
            {
              "id": "stop",
              "value": "{}",
              "type": "string"
            }
          ]
        },
        "method": "GET",
        "header": [
          {
            "key": "Accept",
            "value": "*/*",
            "disabled": false
          }
        ],
        "body": {
          "mode": "raw"
        },
        "description": "Returns a list QTL for given position and assembly map"
      },
      "response": [
        {
          "status": "OK",
          "code": 200,
          "name": "Response_200",
          "id": "1b1030e1-c9ab-49a7-8c33-000f36e09881"
        }
      ]
    },
    {
      "id": "6fdfd87b-a009-41cb-aa4c-ab7549940ea5",
      "name": "getQTLByRgdIdUsingGET",
      "request": {
        "url": {
          "protocol": "http",
          "host": "rest.rgd.mcw.edu",
          "path": [
            "rgdws",
            "qtls/:rgdId"
          ],
          "variable": [
            {
              "id": "rgdId",
              "value": "{}",
              "type": "string"
            }
          ]
        },
        "method": "GET",
        "header": [
          {
            "key": "Accept",
            "value": "*/*",
            "disabled": false
          }
        ],
        "body": {
          "mode": "raw"
        },
        "description": "Return a QTL for provided RGD ID"
      },
      "response": [
        {
          "status": "OK",
          "code": 200,
          "name": "Response_200",
          "id": "49859ee7-919a-441e-8b51-d0cfefe783c0"
        }
      ]
    },
    {
      "id": "0dfe292d-d033-4813-92d9-c3f4ef507908",
      "name": "getActiveObjectCountUsingGET",
      "request": {
        "url": {
          "protocol": "http",
          "host": "rest.rgd.mcw.edu",
          "path": [
            "rgdws",
            "stats/count/activeObject/:speciesTypeKey/:dateYYYYMMDD"
          ],
          "variable": [
            {
              "id": "dateYYYYMMDD",
              "value": "{}",
              "type": "string"
            },
            {
              "id": "speciesTypeKey",
              "value": "{}",
              "type": "string"
            }
          ]
        },
        "method": "GET",
        "header": [
          {
            "key": "Accept",
            "value": "*/*",
            "disabled": false
          }
        ],
        "body": {
          "mode": "raw"
        },
        "description": "Count of active objects by type, for specified species and date"
      },
      "response": [
        {
          "status": "OK",
          "code": 200,
          "name": "Response_200",
          "id": "0eedc9e7-b8ad-41a7-9684-5a97509c775a"
        }
      ]
    },
    {
      "id": "9ab1ee5e-d553-4aeb-93dc-2bd5c6e559ac",
      "name": "getGeneTypeCountUsingGET",
      "request": {
        "url": {
          "protocol": "http",
          "host": "rest.rgd.mcw.edu",
          "path": [
            "rgdws",
            "stats/count/geneType/:speciesTypeKey/:dateYYYYMMDD"
          ],
          "variable": [
            {
              "id": "dateYYYYMMDD",
              "value": "{}",
              "type": "string"
            },
            {
              "id": "speciesTypeKey",
              "value": "{}",
              "type": "string"
            }
          ]
        },
        "method": "GET",
        "header": [
          {
            "key": "Accept",
            "value": "*/*",
            "disabled": false
          }
        ],
        "body": {
          "mode": "raw"
        },
        "description": "Count of gene types, for specified species and date"
      },
      "response": [
        {
          "status": "OK",
          "code": 200,
          "name": "Response_200",
          "id": "a9203ae0-319d-4752-b3ab-a9128ab85386"
        }
      ]
    },
    {
      "id": "a5014959-25d3-40dd-9449-8d29a4a3b0c6",
      "name": "getObjectStatusCountUsingGET",
      "request": {
        "url": {
          "protocol": "http",
          "host": "rest.rgd.mcw.edu",
          "path": [
            "rgdws",
            "stats/count/objectStatus/:speciesTypeKey/:dateYYYYMMDD"
          ],
          "variable": [
            {
              "id": "dateYYYYMMDD",
              "value": "{}",
              "type": "string"
            },
            {
              "id": "speciesTypeKey",
              "value": "{}",
              "type": "string"
            }
          ]
        },
        "method": "GET",
        "header": [
          {
            "key": "Accept",
            "value": "*/*",
            "disabled": false
          }
        ],
        "body": {
          "mode": "raw"
        },
        "description": "Count of objects with given status, for specified species and date"
      },
      "response": [
        {
          "status": "OK",
          "code": 200,
          "name": "Response_200",
          "id": "2bfd48ad-c4e7-4c37-8f93-a563c9d4b27a"
        }
      ]
    },
    {
      "id": "af9f7f33-e969-440c-a773-de3111fe2111",
      "name": "getObjectsWithRefSeqCountUsingGET",
      "request": {
        "url": {
          "protocol": "http",
          "host": "rest.rgd.mcw.edu",
          "path": [
            "rgdws",
            "stats/count/objectWithRefSeq/:speciesTypeKey/:dateYYYYMMDD"
          ],
          "variable": [
            {
              "id": "dateYYYYMMDD",
              "value": "{}",
              "type": "string"
            },
            {
              "id": "speciesTypeKey",
              "value": "{}",
              "type": "string"
            }
          ]
        },
        "method": "GET",
        "header": [
          {
            "key": "Accept",
            "value": "*/*",
            "disabled": false
          }
        ],
        "body": {
          "mode": "raw"
        },
        "description": "Count of objects with reference sequence(s), by object type, for specified species and date"
      },
      "response": [
        {
          "status": "OK",
          "code": 200,
          "name": "Response_200",
          "id": "a1e25f84-9504-4a97-8f4b-7eb53b2770bd"
        }
      ]
    },
    {
      "id": "115f2e3d-c6d7-4b7f-81a8-1570534de46c",
      "name": "getObjectsWithReferenceCountUsingGET",
      "request": {
        "url": {
          "protocol": "http",
          "host": "rest.rgd.mcw.edu",
          "path": [
            "rgdws",
            "stats/count/objectWithReference/:speciesTypeKey/:dateYYYYMMDD"
          ],
          "variable": [
            {
              "id": "dateYYYYMMDD",
              "value": "{}",
              "type": "string"
            },
            {
              "id": "speciesTypeKey",
              "value": "{}",
              "type": "string"
            }
          ]
        },
        "method": "GET",
        "header": [
          {
            "key": "Accept",
            "value": "*/*",
            "disabled": false
          }
        ],
        "body": {
          "mode": "raw"
        },
        "description": "Count of objects with reference, by object type, for specified species and date"
      },
      "response": [
        {
          "status": "OK",
          "code": 200,
          "name": "Response_200",
          "id": "42518ad0-d29a-42b8-8e58-cd976c04105f"
        }
      ]
    },
    {
      "id": "a3bcc48c-e52d-437a-b7f5-4c4f439da993",
      "name": "getObjectsWithXDBsCountUsingGET",
      "request": {
        "url": {
          "protocol": "http",
          "host": "rest.rgd.mcw.edu",
          "path": [
            "rgdws",
            "stats/count/objectWithXdb/:speciesTypeKey/:objectKey/:dateYYYYMMDD"
          ],
          "variable": [
            {
              "id": "dateYYYYMMDD",
              "value": "{}",
              "type": "string"
            },
            {
              "id": "objectKey",
              "value": "{}",
              "type": "string"
            },
            {
              "id": "speciesTypeKey",
              "value": "{}",
              "type": "string"
            }
          ]
        },
        "method": "GET",
        "header": [
          {
            "key": "Accept",
            "value": "*/*",
            "disabled": false
          }
        ],
        "body": {
          "mode": "raw"
        },
        "description": "Count of objects with external database ids, by database id, for specified species, object type and date"
      },
      "response": [
        {
          "status": "OK",
          "code": 200,
          "name": "Response_200",
          "id": "fe7e1da8-2c8b-4e09-bbe3-7779fb443aa9"
        }
      ]
    },
    {
      "id": "1672ac77-65a4-4b4b-9aa4-0cd8f5b1ae43",
      "name": "getProteinInteractionCountUsingGET",
      "request": {
        "url": {
          "protocol": "http",
          "host": "rest.rgd.mcw.edu",
          "path": [
            "rgdws",
            "stats/count/proteinInteraction/:speciesTypeKey/:dateYYYYMMDD"
          ],
          "variable": [
            {
              "id": "dateYYYYMMDD",
              "value": "{}",
              "type": "string"
            },
            {
              "id": "speciesTypeKey",
              "value": "{}",
              "type": "string"
            }
          ]
        },
        "method": "GET",
        "header": [
          {
            "key": "Accept",
            "value": "*/*",
            "disabled": false
          }
        ],
        "body": {
          "mode": "raw"
        },
        "description": "Count of protein interactions, for specified species and date"
      },
      "response": [
        {
          "status": "OK",
          "code": 200,
          "name": "Response_200",
          "id": "e363ea8a-1bc8-4cf3-8717-2d2fde9b33c9"
        }
      ]
    },
    {
      "id": "4f396c21-69f8-4e17-ab6a-615e5ab2114d",
      "name": "getQtlInheritanceTypeCountUsingGET",
      "request": {
        "url": {
          "protocol": "http",
          "host": "rest.rgd.mcw.edu",
          "path": [
            "rgdws",
            "stats/count/qtlInheritanceType/:speciesTypeKey/:dateYYYYMMDD"
          ],
          "variable": [
            {
              "id": "dateYYYYMMDD",
              "value": "{}",
              "type": "string"
            },
            {
              "id": "speciesTypeKey",
              "value": "{}",
              "type": "string"
            }
          ]
        },
        "method": "GET",
        "header": [
          {
            "key": "Accept",
            "value": "*/*",
            "disabled": false
          }
        ],
        "body": {
          "mode": "raw"
        },
        "description": "Count of strains, by qtl inheritance type, for specified species and date"
      },
      "response": [
        {
          "status": "OK",
          "code": 200,
          "name": "Response_200",
          "id": "a22c2849-ab7c-49b7-ac48-b2be13636f53"
        }
      ]
    },
    {
      "id": "c63eabb9-a7bf-4ae0-86d4-65b7d0072ed7",
      "name": "getRetiredObjectCountUsingGET",
      "request": {
        "url": {
          "protocol": "http",
          "host": "rest.rgd.mcw.edu",
          "path": [
            "rgdws",
            "stats/count/retiredObject/:speciesTypeKey/:dateYYYYMMDD"
          ],
          "variable": [
            {
              "id": "dateYYYYMMDD",
              "value": "{}",
              "type": "string"
            },
            {
              "id": "speciesTypeKey",
              "value": "{}",
              "type": "string"
            }
          ]
        },
        "method": "GET",
        "header": [
          {
            "key": "Accept",
            "value": "*/*",
            "disabled": false
          }
        ],
        "body": {
          "mode": "raw"
        },
        "description": "Count of retired objects by type, for specified species and date"
      },
      "response": [
        {
          "status": "OK",
          "code": 200,
          "name": "Response_200",
          "id": "d14f0afe-c0d0-499c-a2f6-71bb84c5b300"
        }
      ]
    },
    {
      "id": "1ef0c5ef-c91d-45de-b749-29f3a7e678a4",
      "name": "getStrainTypeCountUsingGET",
      "request": {
        "url": {
          "protocol": "http",
          "host": "rest.rgd.mcw.edu",
          "path": [
            "rgdws",
            "stats/count/strainType/:speciesTypeKey/:dateYYYYMMDD"
          ],
          "variable": [
            {
              "id": "dateYYYYMMDD",
              "value": "{}",
              "type": "string"
            },
            {
              "id": "speciesTypeKey",
              "value": "{}",
              "type": "string"
            }
          ]
        },
        "method": "GET",
        "header": [
          {
            "key": "Accept",
            "value": "*/*",
            "disabled": false
          }
        ],
        "body": {
          "mode": "raw"
        },
        "description": "Count of strain types, for specified species and date"
      },
      "response": [
        {
          "status": "OK",
          "code": 200,
          "name": "Response_200",
          "id": "7e375780-4c3d-4038-9387-e013733320c1"
        }
      ]
    },
    {
      "id": "31e40d4b-b185-4cd8-9bbb-de615b157c50",
      "name": "getWithdrawnObjectCountUsingGET",
      "request": {
        "url": {
          "protocol": "http",
          "host": "rest.rgd.mcw.edu",
          "path": [
            "rgdws",
            "stats/count/withdrawnObject/:speciesTypeKey/:dateYYYYMMDD"
          ],
          "variable": [
            {
              "id": "dateYYYYMMDD",
              "value": "{}",
              "type": "string"
            },
            {
              "id": "speciesTypeKey",
              "value": "{}",
              "type": "string"
            }
          ]
        },
        "method": "GET",
        "header": [
          {
            "key": "Accept",
            "value": "*/*",
            "disabled": false
          }
        ],
        "body": {
          "mode": "raw"
        },
        "description": "Count of withdrawn objects by type, for specified species and date"
      },
      "response": [
        {
          "status": "OK",
          "code": 200,
          "name": "Response_200",
          "id": "429b9886-f158-4c31-9862-f9587c416ff5"
        }
      ]
    },
    {
      "id": "3995311f-14db-40dd-a143-97486a0009f0",
      "name": "getXdbsCountUsingGET",
      "request": {
        "url": {
          "protocol": "http",
          "host": "rest.rgd.mcw.edu",
          "path": [
            "rgdws",
            "stats/count/xdb/:speciesTypeKey/:dateYYYYMMDD"
          ],
          "variable": [
            {
              "id": "dateYYYYMMDD",
              "value": "{}",
              "type": "string"
            },
            {
              "id": "speciesTypeKey",
              "value": "{}",
              "type": "string"
            }
          ]
        },
        "method": "GET",
        "header": [
          {
            "key": "Accept",
            "value": "*/*",
            "disabled": false
          }
        ],
        "body": {
          "mode": "raw"
        },
        "description": "Count of external database ids, for specied species and date"
      },
      "response": [
        {
          "status": "OK",
          "code": 200,
          "name": "Response_200",
          "id": "0bc56b15-de76-4be2-93c7-537eafb9d782"
        }
      ]
    },
    {
      "id": "15cb24c4-370e-48c3-97aa-ab97550fd541",
      "name": "getActiveObjectDiffUsingGET",
      "request": {
        "url": {
          "protocol": "http",
          "host": "rest.rgd.mcw.edu",
          "path": [
            "rgdws",
            "stats/diff/activeObject/:speciesTypeKey/:dateFromYYYYMMDD/:dateToYYYYMMDD"
          ],
          "variable": [
            {
              "id": "dateFromYYYYMMDD",
              "value": "{}",
              "type": "string"
            },
            {
              "id": "dateToYYYYMMDD",
              "value": "{}",
              "type": "string"
            },
            {
              "id": "speciesTypeKey",
              "value": "{}",
              "type": "string"
            }
          ]
        },
        "method": "GET",
        "header": [
          {
            "key": "Accept",
            "value": "*/*",
            "disabled": false
          }
        ],
        "body": {
          "mode": "raw"
        },
        "description": "Count difference of active objects, by type, for specified species and date range"
      },
      "response": [
        {
          "status": "OK",
          "code": 200,
          "name": "Response_200",
          "id": "cd8ea16d-9cf6-4412-8408-934bcdfda2f3"
        }
      ]
    },
    {
      "id": "6abc6f82-caec-4fef-92e8-2d12ad4ed59a",
      "name": "getGeneTypeDiffUsingGET",
      "request": {
        "url": {
          "protocol": "http",
          "host": "rest.rgd.mcw.edu",
          "path": [
            "rgdws",
            "stats/diff/geneType/:speciesTypeKey/:dateFromYYYYMMDD/:dateToYYYYMMDD"
          ],
          "variable": [
            {
              "id": "dateFromYYYYMMDD",
              "value": "{}",
              "type": "string"
            },
            {
              "id": "dateToYYYYMMDD",
              "value": "{}",
              "type": "string"
            },
            {
              "id": "speciesTypeKey",
              "value": "{}",
              "type": "string"
            }
          ]
        },
        "method": "GET",
        "header": [
          {
            "key": "Accept",
            "value": "*/*",
            "disabled": false
          }
        ],
        "body": {
          "mode": "raw"
        },
        "description": "Count difference of gene types, for specified species and date range"
      },
      "response": [
        {
          "status": "OK",
          "code": 200,
          "name": "Response_200",
          "id": "c03baeec-f8d4-4526-b83b-61daa1a111b7"
        }
      ]
    },
    {
      "id": "96bcd1cd-25a4-44f3-8f87-8ce08fbbdb7f",
      "name": "getObjectStatusDiffUsingGET",
      "request": {
        "url": {
          "protocol": "http",
          "host": "rest.rgd.mcw.edu",
          "path": [
            "rgdws",
            "stats/diff/objectStatus/:speciesTypeKey/:dateFromYYYYMMDD/:dateToYYYYMMDD"
          ],
          "variable": [
            {
              "id": "dateFromYYYYMMDD",
              "value": "{}",
              "type": "string"
            },
            {
              "id": "dateToYYYYMMDD",
              "value": "{}",
              "type": "string"
            },
            {
              "id": "speciesTypeKey",
              "value": "{}",
              "type": "string"
            }
          ]
        },
        "method": "GET",
        "header": [
          {
            "key": "Accept",
            "value": "*/*",
            "disabled": false
          }
        ],
        "body": {
          "mode": "raw"
        },
        "description": "Count difference of objects with given status, for specified species and date range"
      },
      "response": [
        {
          "status": "OK",
          "code": 200,
          "name": "Response_200",
          "id": "aa876627-5976-4f2e-8671-bd811775b11e"
        }
      ]
    },
    {
      "id": "2a29979c-2b77-4727-bb32-7c7edf34040f",
      "name": "getObjectsWithRefSeqDiffUsingGET",
      "request": {
        "url": {
          "protocol": "http",
          "host": "rest.rgd.mcw.edu",
          "path": [
            "rgdws",
            "stats/diff/objectWithRefSeq/:speciesTypeKey/:dateFromYYYYMMDD/:dateToYYYYMMDD"
          ],
          "variable": [
            {
              "id": "dateFromYYYYMMDD",
              "value": "{}",
              "type": "string"
            },
            {
              "id": "dateToYYYYMMDD",
              "value": "{}",
              "type": "string"
            },
            {
              "id": "speciesTypeKey",
              "value": "{}",
              "type": "string"
            }
          ]
        },
        "method": "GET",
        "header": [
          {
            "key": "Accept",
            "value": "*/*",
            "disabled": false
          }
        ],
        "body": {
          "mode": "raw"
        },
        "description": "Count difference of objects with reference sequence(s), by object type, for specified species and date range"
      },
      "response": [
        {
          "status": "OK",
          "code": 200,
          "name": "Response_200",
          "id": "db0c7d3e-637c-4b98-bab2-de753759b491"
        }
      ]
    },
    {
      "id": "91ebe302-dc5a-4a5f-b009-4884a58a8c85",
      "name": "getObjectsWithReferenceDiffUsingGET",
      "request": {
        "url": {
          "protocol": "http",
          "host": "rest.rgd.mcw.edu",
          "path": [
            "rgdws",
            "stats/diff/objectWithReference/:speciesTypeKey/:dateFromYYYYMMDD/:dateToYYYYMMDD"
          ],
          "variable": [
            {
              "id": "dateFromYYYYMMDD",
              "value": "{}",
              "type": "string"
            },
            {
              "id": "dateToYYYYMMDD",
              "value": "{}",
              "type": "string"
            },
            {
              "id": "speciesTypeKey",
              "value": "{}",
              "type": "string"
            }
          ]
        },
        "method": "GET",
        "header": [
          {
            "key": "Accept",
            "value": "*/*",
            "disabled": false
          }
        ],
        "body": {
          "mode": "raw"
        },
        "description": "Count difference of objects with reference, by object type, for specified species and date range"
      },
      "response": [
        {
          "status": "OK",
          "code": 200,
          "name": "Response_200",
          "id": "6b542026-6982-4a6f-86f3-5c3060396400"
        }
      ]
    },
    {
      "id": "94444429-226d-4b3b-9f5f-1c2a5103743f",
      "name": "getObjectsWithXDBsDiffUsingGET",
      "request": {
        "url": {
          "protocol": "http",
          "host": "rest.rgd.mcw.edu",
          "path": [
            "rgdws",
            "stats/diff/objectWithXdb/:speciesTypeKey/:objectKey/:dateFromYYYYMMDD/:dateToYYYYMMDD"
          ],
          "variable": [
            {
              "id": "dateFromYYYYMMDD",
              "value": "{}",
              "type": "string"
            },
            {
              "id": "dateToYYYYMMDD",
              "value": "{}",
              "type": "string"
            },
            {
              "id": "objectKey",
              "value": "{}",
              "type": "string"
            },
            {
              "id": "speciesTypeKey",
              "value": "{}",
              "type": "string"
            }
          ]
        },
        "method": "GET",
        "header": [
          {
            "key": "Accept",
            "value": "*/*",
            "disabled": false
          }
        ],
        "body": {
          "mode": "raw"
        },
        "description": "Count difference of objects with external database ids, by database id, for specified species, object type and date range"
      },
      "response": [
        {
          "status": "OK",
          "code": 200,
          "name": "Response_200",
          "id": "470188fd-6444-4e96-9e0e-35599b8dad6a"
        }
      ]
    },
    {
      "id": "c0b2402f-1f27-4ed7-9cb3-e35e23901926",
      "name": "getProteinInteractionDiffUsingGET",
      "request": {
        "url": {
          "protocol": "http",
          "host": "rest.rgd.mcw.edu",
          "path": [
            "rgdws",
            "stats/diff/proteinInteraction/:speciesTypeKey/:dateFromYYYYMMDD/:dateToYYYYMMDD"
          ],
          "variable": [
            {
              "id": "dateFromYYYYMMDD",
              "value": "{}",
              "type": "string"
            },
            {
              "id": "dateToYYYYMMDD",
              "value": "{}",
              "type": "string"
            },
            {
              "id": "speciesTypeKey",
              "value": "{}",
              "type": "string"
            }
          ]
        },
        "method": "GET",
        "header": [
          {
            "key": "Accept",
            "value": "*/*",
            "disabled": false
          }
        ],
        "body": {
          "mode": "raw"
        },
        "description": "Count difference of protein interactions, for specified species and date range"
      },
      "response": [
        {
          "status": "OK",
          "code": 200,
          "name": "Response_200",
          "id": "7157aa34-2aed-4c39-a7db-b1b1d1c2d6ee"
        }
      ]
    },
    {
      "id": "83ecc6ee-8def-46ad-9775-ba958379e1fb",
      "name": "getQtlInheritanceTypeDiffUsingGET",
      "request": {
        "url": {
          "protocol": "http",
          "host": "rest.rgd.mcw.edu",
          "path": [
            "rgdws",
            "stats/diff/qtlInheritanceType/:speciesTypeKey/:dateFromYYYYMMDD/:dateToYYYYMMDD"
          ],
          "variable": [
            {
              "id": "dateFromYYYYMMDD",
              "value": "{}",
              "type": "string"
            },
            {
              "id": "dateToYYYYMMDD",
              "value": "{}",
              "type": "string"
            },
            {
              "id": "speciesTypeKey",
              "value": "{}",
              "type": "string"
            }
          ]
        },
        "method": "GET",
        "header": [
          {
            "key": "Accept",
            "value": "*/*",
            "disabled": false
          }
        ],
        "body": {
          "mode": "raw"
        },
        "description": "Count difference of strains, by qtl inheritance type, for specified species and date range"
      },
      "response": [
        {
          "status": "OK",
          "code": 200,
          "name": "Response_200",
          "id": "8296d0f7-683b-4911-a180-c402779a0977"
        }
      ]
    },
    {
      "id": "b54790de-b24c-43f3-b38c-1c329bda1ce8",
      "name": "getRetiredObjectDiffUsingGET",
      "request": {
        "url": {
          "protocol": "http",
          "host": "rest.rgd.mcw.edu",
          "path": [
            "rgdws",
            "stats/diff/retiredObject/:speciesTypeKey/:dateFromYYYYMMDD/:dateToYYYYMMDD"
          ],
          "variable": [
            {
              "id": "dateFromYYYYMMDD",
              "value": "{}",
              "type": "string"
            },
            {
              "id": "dateToYYYYMMDD",
              "value": "{}",
              "type": "string"
            },
            {
              "id": "speciesTypeKey",
              "value": "{}",
              "type": "string"
            }
          ]
        },
        "method": "GET",
        "header": [
          {
            "key": "Accept",
            "value": "*/*",
            "disabled": false
          }
        ],
        "body": {
          "mode": "raw"
        },
        "description": "Count difference of retired objects, by type, for specified species and date range"
      },
      "response": [
        {
          "status": "OK",
          "code": 200,
          "name": "Response_200",
          "id": "cf793825-4c6b-4ad1-b815-cd961e5ad345"
        }
      ]
    },
    {
      "id": "abb6c7a9-e95b-49b9-bd49-38dd853124e6",
      "name": "getStrainTypeDiffUsingGET",
      "request": {
        "url": {
          "protocol": "http",
          "host": "rest.rgd.mcw.edu",
          "path": [
            "rgdws",
            "stats/diff/strainType/:speciesTypeKey/:dateFromYYYYMMDD/:dateToYYYYMMDD"
          ],
          "variable": [
            {
              "id": "dateFromYYYYMMDD",
              "value": "{}",
              "type": "string"
            },
            {
              "id": "dateToYYYYMMDD",
              "value": "{}",
              "type": "string"
            },
            {
              "id": "speciesTypeKey",
              "value": "{}",
              "type": "string"
            }
          ]
        },
        "method": "GET",
        "header": [
          {
            "key": "Accept",
            "value": "*/*",
            "disabled": false
          }
        ],
        "body": {
          "mode": "raw"
        },
        "description": "Count difference of strain types, for specified species and date range"
      },
      "response": [
        {
          "status": "OK",
          "code": 200,
          "name": "Response_200",
          "id": "71511c0f-da3f-4a77-a0d9-056f86b53ffa"
        }
      ]
    },
    {
      "id": "5155923b-ab9f-47ff-9458-b886baf0dd42",
      "name": "getWithdrawnObjectDiffUsingGET",
      "request": {
        "url": {
          "protocol": "http",
          "host": "rest.rgd.mcw.edu",
          "path": [
            "rgdws",
            "stats/diff/withdrawnObject/:speciesTypeKey/:dateFromYYYYMMDD/:dateToYYYYMMDD"
          ],
          "variable": [
            {
              "id": "dateFromYYYYMMDD",
              "value": "{}",
              "type": "string"
            },
            {
              "id": "dateToYYYYMMDD",
              "value": "{}",
              "type": "string"
            },
            {
              "id": "speciesTypeKey",
              "value": "{}",
              "type": "string"
            }
          ]
        },
        "method": "GET",
        "header": [
          {
            "key": "Accept",
            "value": "*/*",
            "disabled": false
          }
        ],
        "body": {
          "mode": "raw"
        },
        "description": "Count difference of withdrawn objects, by type, for specified species and date range"
      },
      "response": [
        {
          "status": "OK",
          "code": 200,
          "name": "Response_200",
          "id": "25a3771c-7416-4228-95e1-1668bab763cd"
        }
      ]
    },
    {
      "id": "ad14707e-f21d-45e2-9a05-1ef02cd15900",
      "name": "getXdbsDiffUsingGET",
      "request": {
        "url": {
          "protocol": "http",
          "host": "rest.rgd.mcw.edu",
          "path": [
            "rgdws",
            "stats/diff/xdb/:speciesTypeKey/:dateFromYYYYMMDD/:dateToYYYYMMDD"
          ],
          "variable": [
            {
              "id": "dateFromYYYYMMDD",
              "value": "{}",
              "type": "string"
            },
            {
              "id": "dateToYYYYMMDD",
              "value": "{}",
              "type": "string"
            },
            {
              "id": "speciesTypeKey",
              "value": "{}",
              "type": "string"
            }
          ]
        },
        "method": "GET",
        "header": [
          {
            "key": "Accept",
            "value": "*/*",
            "disabled": false
          }
        ],
        "body": {
          "mode": "raw"
        },
        "description": "Count difference of external database ids, for specified species and date range"
      },
      "response": [
        {
          "status": "OK",
          "code": 200,
          "name": "Response_200",
          "id": "2eea0f55-b984-4ed7-a5a7-fbf2984886c5"
        }
      ]
    }
  ]
}