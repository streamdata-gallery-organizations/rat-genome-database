{
  "info": {
    "name": "Rat Genome Database Return a list of gene alleles",
    "_postman_id": "3b3f3b8c-bbb0-41d0-9218-9fdb6aab10a0",
    "description": "",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "id": "6348942e-d089-4d92-b2c9-8ae2a37badde",
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
          "id": "34275a83-4f4f-459e-8f70-7d4bec8e8c79"
        }
      ]
    },
    {
      "id": "5b07730a-fed1-4f57-be1b-f8a61c81c773",
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
          "id": "b8c1b443-f88a-447f-8d7b-935e06628df2"
        }
      ]
    },
    {
      "id": "81db9f50-c781-4960-bf7d-f3bc49c7deee",
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
          "id": "89b3c7fd-41d5-478a-b608-478ba2a11333"
        }
      ]
    },
    {
      "id": "be2f8998-bfa8-4329-b14d-326793e816b8",
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
          "id": "a736ec8c-459b-4f46-a8b5-78f7d5bd404e"
        }
      ]
    },
    {
      "id": "51281c28-e63c-4e47-9cc6-b5a96852ab5b",
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
          "id": "8d95a50b-fae5-4125-915e-5f58415697e2"
        }
      ]
    },
    {
      "id": "3e1f74cd-18c3-4778-b68a-946d1913549f",
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
          "id": "de88a324-468d-42e1-a888-504ee4a26571"
        }
      ]
    },
    {
      "id": "c325b48a-78d8-4087-a108-3f31f7063b2e",
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
          "id": "c12c3bfe-d863-444d-b6a2-0adf8afe0945"
        }
      ]
    },
    {
      "id": "85bae80e-f815-4d23-a159-dd62ef86edae",
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
          "id": "8688e0da-8edd-49f4-8cbc-3ce5199e476f"
        }
      ]
    },
    {
      "id": "4b018371-4734-46fc-8249-6cbc38f9e083",
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
          "id": "127db14f-7678-41d4-b008-4c0543dd91d5"
        }
      ]
    },
    {
      "id": "9ca9a16c-6976-4fbd-99d2-17f8f323b07e",
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
          "id": "f6241312-3853-4c23-bc0e-aa52754b27aa"
        }
      ]
    },
    {
      "id": "8650f7b2-c7b3-4ab6-a3fb-5069ec3df933",
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
          "id": "dd9096fc-f6a1-4887-b1a3-3b23054d6cff"
        }
      ]
    },
    {
      "id": "0c537857-2dd1-412f-bc23-191711a51c0b",
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
          "id": "79a2ba4c-4b95-48f1-8573-b67a9a92cf4f"
        }
      ]
    }
  ]
}