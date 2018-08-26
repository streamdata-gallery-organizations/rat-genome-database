{
  "info": {
    "name": "Rat Genome Database Count of objects with given status, for specified species and date",
    "_postman_id": "0f18b27d-ab47-44d0-94b5-586bcd88bfeb",
    "description": "",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "id": "59b6dc18-0eb5-4699-a959-d4720c6463ce",
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
          "id": "ba794011-9850-41eb-90d6-5a82c466cd49"
        }
      ]
    },
    {
      "id": "96c9461e-87dc-47a8-9cf9-f9c3c5b7de15",
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
          "id": "7a2b8e96-52aa-4140-8e66-638d0db4d8d8"
        }
      ]
    },
    {
      "id": "4c35a24d-ba9d-4209-bdbd-cee8ae4dc29b",
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
          "id": "8af96c26-13a9-4af3-9d59-28542e9c083a"
        }
      ]
    },
    {
      "id": "15d2a91d-b2a0-465b-a718-0e1976abd50e",
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
          "id": "05a99ea1-bc8c-4406-bcf7-77e472e6bf51"
        }
      ]
    },
    {
      "id": "7027f53b-2a7f-4736-af17-e88d4f3940d5",
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
          "id": "5ef91fb9-b784-4367-813f-4cc1659d2244"
        }
      ]
    },
    {
      "id": "04cfd500-12c9-4e7f-9c67-eb159326199d",
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
          "id": "dde98948-1a52-4d2f-afbb-8cb794582999"
        }
      ]
    },
    {
      "id": "24c1a7f7-5e45-4df9-9489-3591d415c28b",
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
          "id": "0c48fdd2-1906-42e9-8a0b-d3a03124ee11"
        }
      ]
    },
    {
      "id": "7fcb78f0-0522-49d2-9338-3daf66338e71",
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
          "id": "322616a5-5a61-46cb-97ad-83bcc42a558c"
        }
      ]
    },
    {
      "id": "87d98c4c-47e2-436e-a76c-5222003add7e",
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
          "id": "70d9778d-af2d-4bec-b450-db888f8134af"
        }
      ]
    },
    {
      "id": "9cf01805-2316-4656-a2d0-6829c94c113d",
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
          "id": "c0914ee6-cacc-4064-a78b-14eaf76117dd"
        }
      ]
    },
    {
      "id": "8d707d1a-1ce0-46d1-8a96-f097356688cc",
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
          "id": "ba7746ba-fa1f-41d5-afc2-adadf2d2ab43"
        }
      ]
    },
    {
      "id": "4beba38e-2087-411d-a431-50352026b170",
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
          "id": "b86b418c-ad07-47d0-bfe4-b8df7a5b35a0"
        }
      ]
    },
    {
      "id": "41909dd8-3283-41d4-9bee-fc184b1d21a6",
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
          "id": "8abf92e5-f522-4cda-9b43-ff0b22a9ba42"
        }
      ]
    },
    {
      "id": "b17e962b-1a3c-43e5-b7a4-5b22e967b5b1",
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
          "id": "2106546d-3ade-452a-a850-29ba951ccddb"
        }
      ]
    },
    {
      "id": "3147617f-be6d-4c8e-81cb-8063439e5333",
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
          "id": "e7ae5ed5-f7ab-499b-9273-db3098a3b6cb"
        }
      ]
    },
    {
      "id": "667bde23-be4d-4588-8768-a7e81e3abde2",
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
          "id": "ea12ae8f-4f97-4f85-b480-b8103289d2dd"
        }
      ]
    },
    {
      "id": "48cd4548-0d25-431b-9c3a-9b6915cb4bfd",
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
          "id": "c4f4ca1d-1755-4ded-9ea8-a5f21177c20d"
        }
      ]
    },
    {
      "id": "1d32d05e-f865-4328-8c74-25f40df82b87",
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
          "id": "2b49a979-081b-48d8-af9c-d6cab61fd1d8"
        }
      ]
    },
    {
      "id": "44b64f41-e82a-4cee-ae45-19f6aa47cd8f",
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
          "id": "57322523-a817-4c8c-b73e-bf047791f1b6"
        }
      ]
    },
    {
      "id": "439888f9-dad7-47d5-b4ce-e9777fea453e",
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
          "id": "3be1e074-a24c-4d55-a36f-bc98a1e2c432"
        }
      ]
    },
    {
      "id": "4579a668-7b41-4bc9-9892-e67da780e28c",
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
          "id": "69ed251f-a737-4ac6-960c-4662c4a13f2d"
        }
      ]
    },
    {
      "id": "99b8848c-78f3-41f8-a43a-568e954d5e7c",
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
          "id": "f9f2c26f-2a52-4417-94af-5a3374821471"
        }
      ]
    },
    {
      "id": "7c04a7b3-ac9f-4be7-a25f-e2bb70adf22a",
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
          "id": "ba22274b-6068-46b5-983c-12be1108cc97"
        }
      ]
    },
    {
      "id": "cf8abcd2-129a-43ab-a96c-6d2b05c7a39c",
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
          "id": "d1ade5bd-89c8-48c5-80e0-ee8fb78507a4"
        }
      ]
    },
    {
      "id": "18c6da38-815d-42d3-90ba-a0c37919197a",
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
          "id": "76750b4d-806c-4bdd-9a3d-de293b322e67"
        }
      ]
    },
    {
      "id": "9da6029d-cfc8-4fba-9ab3-791e208f7699",
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
          "id": "f991946b-be30-4e59-984f-e514606aa9c4"
        }
      ]
    },
    {
      "id": "7c8e96f8-52ac-4176-aacb-dc7e0250f59b",
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
          "id": "8e0b8fef-b707-40f0-9596-05f82a94f6f0"
        }
      ]
    },
    {
      "id": "2bd10961-6382-42ad-893d-97896bfd657e",
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
          "id": "bb2ccbf8-64a8-4419-a1e3-c8593204aeee"
        }
      ]
    },
    {
      "id": "cd0cc8f2-597a-48ad-bd24-889d9cc112eb",
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
          "id": "671e6b67-16c1-4094-b137-1e6d96429e72"
        }
      ]
    },
    {
      "id": "5bd968ee-e6ed-44da-a4f2-4b1dc826f801",
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
          "id": "3eb53ede-146c-46bd-8e18-7bf66c223ec9"
        }
      ]
    },
    {
      "id": "5a8b3508-eb56-4af1-a9a6-2e8705e89b81",
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
          "id": "5a36f5d9-cdb8-4b06-9b8d-e6c8b282b54d"
        }
      ]
    }
  ]
}