{
  "info": {
    "name": "Rat Genome Database Count of objects with reference, by object type, for specified species and date",
    "_postman_id": "bcd6fbbe-aa6b-446d-9f0c-bb5fe29a273c",
    "description": "",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "id": "e0a43b74-8fb1-407d-abca-fe78975b47a5",
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
          "id": "a98d4fa6-bf7c-40b8-9fbb-fd80b7172026"
        }
      ]
    },
    {
      "id": "850bbc3f-9245-414b-a925-79f71c36f9c4",
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
          "id": "e4a0dc55-7f81-4eac-abfb-37ca17b21d70"
        }
      ]
    },
    {
      "id": "118462d9-0459-4c9d-8aa0-5bfa0dcc49dd",
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
          "id": "933f4f62-eee9-4f98-b4c0-b19c8a09ac30"
        }
      ]
    },
    {
      "id": "2e810721-0cf3-48e3-9056-3b2df818f2b0",
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
          "id": "d8e379aa-4647-4429-b51c-669528e89997"
        }
      ]
    },
    {
      "id": "9a9c363d-6606-43ca-87ef-fea7acf9b3eb",
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
          "id": "276c8637-26eb-4156-9b57-a21540a3a205"
        }
      ]
    },
    {
      "id": "11792206-fea7-45f4-8ba1-e7899ce7398a",
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
          "id": "4746aacf-08a2-4b14-96bb-a5146cb646b7"
        }
      ]
    },
    {
      "id": "cfb46096-90ff-4848-934c-15caea97ab8b",
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
          "id": "5fecec9c-f272-4ae6-bf5e-f9348bf26f8f"
        }
      ]
    },
    {
      "id": "7d787000-331b-4a1d-85dd-02f252e0ad08",
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
          "id": "04b84ffe-b6a7-4138-b64f-cb9a7e6cd3bf"
        }
      ]
    },
    {
      "id": "6a8be67b-4d52-46d0-9041-f99efdb4154f",
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
          "id": "7645c5f8-a1ba-4ad1-ac40-26cb0afd7695"
        }
      ]
    },
    {
      "id": "36a48794-592c-494d-a5ec-b6dcd08abb63",
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
          "id": "62778321-5f23-4271-9991-52d824bd8f1b"
        }
      ]
    },
    {
      "id": "eee49af1-be54-43f3-94da-e00a06300ee7",
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
          "id": "f7c14fc7-4c25-4c7d-a3d4-a7aa66353933"
        }
      ]
    },
    {
      "id": "0dd91179-1f1b-4124-9747-62e71b931485",
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
          "id": "0cdbfa7e-fdd7-40e1-8828-af0921e54e53"
        }
      ]
    },
    {
      "id": "4f8993c9-88cf-4ace-beca-329ada684361",
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
          "id": "b6547960-7315-4e14-8c58-508fd85d096a"
        }
      ]
    },
    {
      "id": "5467cb27-671d-40fe-89d6-d81b629a60ad",
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
          "id": "ecf8182a-84e4-4dd6-83cd-ee45e31c7d53"
        }
      ]
    },
    {
      "id": "3bb82b9c-5b60-4664-b3b2-d8acc62030eb",
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
          "id": "52af76ac-4806-4da5-8ce1-ce2cf4d23191"
        }
      ]
    },
    {
      "id": "d243f577-53be-48f4-bdb8-1a8cd1bac637",
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
          "id": "0965c857-ac41-47c5-87d1-8b036efde215"
        }
      ]
    },
    {
      "id": "4ddf7559-19ef-44f4-aeaa-99e293e23679",
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
          "id": "12d5016f-aad6-4ce9-88dd-0a31d98197d8"
        }
      ]
    },
    {
      "id": "0cf4a32a-f0ff-4975-9651-8f5781607213",
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
          "id": "b986806b-0801-4abd-8f95-114fe428d334"
        }
      ]
    },
    {
      "id": "59f97007-304d-4d5d-9fe7-fc75caae30cd",
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
          "id": "86c12da9-ca0c-4188-8fcb-8bb825907f14"
        }
      ]
    },
    {
      "id": "167c7d8b-b8a7-42e2-9973-19eea7191d47",
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
          "id": "d47f2169-846c-43d1-8c62-6659026772d6"
        }
      ]
    },
    {
      "id": "c58ae07a-6ae6-48fc-a64a-2bc54906b597",
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
          "id": "32bce784-f190-45ea-a762-73c360f0da70"
        }
      ]
    },
    {
      "id": "6ec5d395-d684-42cd-8aa7-6d8fea475ece",
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
          "id": "0d82b359-2f6b-4ea4-80d0-f18aedb5dd15"
        }
      ]
    },
    {
      "id": "2f1b8f99-f6d7-4384-92e2-21c7ab9bbc9e",
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
          "id": "6937ea62-35bf-4a24-a7aa-d25181100009"
        }
      ]
    },
    {
      "id": "5085f9ea-6124-4b55-b0a6-3b3b28af40b9",
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
          "id": "dc3e9292-7605-4a86-bb6c-14e2bba2ed53"
        }
      ]
    },
    {
      "id": "ff937a81-f886-4d73-9597-fa9754716b88",
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
          "id": "4758b02c-bfc6-4e2c-8905-ec69b45fd94b"
        }
      ]
    },
    {
      "id": "9ff6a73a-3e47-4a58-aadd-0ac83085a83f",
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
          "id": "1a82203b-7fe1-4505-a65b-dfa0337b2ae8"
        }
      ]
    },
    {
      "id": "5c0ef7c8-d48c-44d6-b943-5b649bf91298",
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
          "id": "9f54564d-9e07-4ba2-8a79-ad336d22f54d"
        }
      ]
    },
    {
      "id": "a983a63b-386f-4cd9-ae88-162b04cfd001",
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
          "id": "697bdfb9-11a6-4c50-9458-7a4baab4c638"
        }
      ]
    },
    {
      "id": "95416e9a-7022-4e72-a78d-7abbfb83b017",
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
          "id": "921cc9b7-ab74-4c43-9484-31ee2a1d3376"
        }
      ]
    },
    {
      "id": "7a7718ac-b5ec-4665-bc91-b7bcb3499b60",
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
          "id": "08f8e3a1-4105-4b2e-aced-45fc86492d2a"
        }
      ]
    },
    {
      "id": "0ce73e1f-b57d-4eb2-9c7f-e558a3511d6a",
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
          "id": "c7deb703-57f0-4160-bf23-8decc4d98f0f"
        }
      ]
    },
    {
      "id": "fcf7404b-c278-4295-9beb-0fc8e8a320b2",
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
          "id": "0ee73a1a-b289-416a-9ac6-b1576c498a35"
        }
      ]
    },
    {
      "id": "77ecf7ee-4b23-487f-a2a3-ffae1b86f27b",
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
          "id": "71712b00-6d24-4ab0-9485-1a5af9a1ad05"
        }
      ]
    }
  ]
}