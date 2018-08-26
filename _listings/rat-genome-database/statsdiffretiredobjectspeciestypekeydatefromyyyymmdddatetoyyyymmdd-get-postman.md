{
  "info": {
    "name": "Rat Genome Database Count difference of retired objects, by type, for specified species and date range",
    "_postman_id": "ccd2d45c-049e-40e6-839c-723b0efbe45d",
    "description": "",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "id": "07925350-54ea-4c0c-8bc0-a903621676d4",
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
          "id": "f63c793c-b524-49bf-840f-9453410c8dcd"
        }
      ]
    },
    {
      "id": "b7ca9d86-05c4-4f0d-8af1-f00000a70d4f",
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
          "id": "d514916e-b182-4895-b51b-04524b50c17b"
        }
      ]
    },
    {
      "id": "b8f330e7-9656-4e3a-a194-5a856d8502a3",
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
          "id": "8a26022a-41a0-4710-874c-3352529d833c"
        }
      ]
    },
    {
      "id": "afd42b5c-71d3-418a-9132-63e8341df93b",
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
          "id": "3aa59127-c890-4195-b5d5-0fb0c290abf6"
        }
      ]
    },
    {
      "id": "3368f113-3fcb-45e0-82dd-6f5296dac2a6",
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
          "id": "96a3e04e-5304-4545-a78f-0a905fd4fc2a"
        }
      ]
    },
    {
      "id": "760bfa5e-4e4f-4655-8145-4f813ca4a78b",
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
          "id": "04270a40-8a3e-402f-ba14-a544db054165"
        }
      ]
    },
    {
      "id": "483e40bd-9229-4915-a06c-13fc4fc7a2bc",
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
          "id": "9877de59-412e-4c1c-a04c-2ee3e09fd2b1"
        }
      ]
    },
    {
      "id": "7c824a4c-7dce-49af-8b03-0263e486e592",
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
          "id": "aeee075d-2957-4214-b85b-b6e6e969d9a8"
        }
      ]
    },
    {
      "id": "6549bd87-d067-46c0-b00d-c55c233490fb",
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
          "id": "2ab02b2e-8aeb-4e12-85f9-7157cade29ff"
        }
      ]
    },
    {
      "id": "b4ac72a4-bb70-4364-acb2-767868d9b629",
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
          "id": "cb95b51e-3c3c-4fcb-9e3d-2635a2f39f17"
        }
      ]
    },
    {
      "id": "d3334dcb-826e-429c-84c5-888b6299824b",
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
          "id": "13302cab-465e-4947-bfe8-042de8375e34"
        }
      ]
    },
    {
      "id": "00bebd7f-9639-44d7-8e4a-4d5c75f186ba",
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
          "id": "1dd82cf3-9c57-423d-b5b1-e811fe747d19"
        }
      ]
    },
    {
      "id": "16a9767f-132e-405b-b5c7-424d40fb86bf",
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
          "id": "072bd47f-0b34-41ab-851c-0368761946ba"
        }
      ]
    },
    {
      "id": "cc821826-e9ae-48d3-9f67-83178e3fdca4",
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
          "id": "f568537c-4a84-4ca5-afba-b32a7d80fac8"
        }
      ]
    },
    {
      "id": "dea830af-6058-40b3-8fea-d3d04f3b139d",
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
          "id": "f77ac0c3-f385-485e-8e39-7b35659b3200"
        }
      ]
    },
    {
      "id": "9c3f41ab-9fd6-4ef5-9789-41a44fa45c98",
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
          "id": "84ed8de8-6db2-41bf-a65a-b2de84236dc3"
        }
      ]
    },
    {
      "id": "82663f88-8ae3-4dc7-b3f4-f47df1be3bfd",
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
          "id": "a1c6dc44-bc89-4a60-874d-45696e31453b"
        }
      ]
    },
    {
      "id": "40d366a8-6fe4-4527-b94d-27c875d27249",
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
          "id": "4de1d62c-147c-4857-a555-49a2908da6bc"
        }
      ]
    },
    {
      "id": "f611c5a5-1510-4058-97b5-f679cc2ebee1",
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
          "id": "87c3257c-7df9-45a5-8308-0f9b058268ac"
        }
      ]
    },
    {
      "id": "34d09353-d94b-4c80-b4c2-436b53938379",
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
          "id": "5b2fe33b-46fa-445e-b105-16efeb7c27fc"
        }
      ]
    },
    {
      "id": "fcd4c2ef-2dbb-4c6a-b6a7-eef9ba987a79",
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
          "id": "26285db7-4f63-478e-82cc-d3fe104e1ae0"
        }
      ]
    },
    {
      "id": "b67d73b8-4acb-4e41-8a46-2ac01e0ea121",
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
          "id": "d521d079-0e4e-48cf-a77f-c1a5b6c2a070"
        }
      ]
    },
    {
      "id": "b3a376d2-32e9-47c7-9b09-8ab279135d2f",
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
          "id": "e5e53809-9965-4696-bc26-1af55fdfbeb2"
        }
      ]
    },
    {
      "id": "c1799523-5c9d-4791-bb3b-33946c89bc9c",
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
          "id": "de70f5bc-d512-4c1b-a701-49afc9b7863e"
        }
      ]
    },
    {
      "id": "ee623412-6a48-4378-87a8-5b10ffc98d2e",
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
          "id": "cb331e1d-f9d8-44e1-aeee-27635bda77ef"
        }
      ]
    },
    {
      "id": "cb7b6f03-67ff-4107-b3e0-7d911c842b85",
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
          "id": "7d776edf-190b-496c-840f-28b89c44a703"
        }
      ]
    },
    {
      "id": "8ce50196-cefc-4baa-a183-3aee29609008",
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
          "id": "22e48506-9b7d-43df-8a71-21f09031de94"
        }
      ]
    },
    {
      "id": "a80f7948-c3f4-4bc9-b6ae-2bcef696c2dc",
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
          "id": "00e970ce-d2f2-40cd-affb-78799cff839a"
        }
      ]
    },
    {
      "id": "908c98af-6658-46dc-8cbb-69619ca6d2dc",
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
          "id": "003ad1eb-02f4-45be-b866-aad6b297e26a"
        }
      ]
    },
    {
      "id": "53b53f7b-31ac-400f-8ee0-7f6e926f996a",
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
          "id": "d1829c53-9cbb-4cb2-a269-1fe5b5f6f78f"
        }
      ]
    },
    {
      "id": "e8469ed0-da20-44f6-84c9-da1a17802ae7",
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
          "id": "26ec76bd-a279-45dd-aee1-8ecf632b2678"
        }
      ]
    },
    {
      "id": "b1e5feb1-f089-49d2-a34e-feb7169ed459",
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
          "id": "a4c38663-bbb8-4eaf-bea2-889a2ed7d8f8"
        }
      ]
    },
    {
      "id": "77eb6062-36d6-44f3-baf2-1da37960dc50",
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
          "id": "c1e98730-b624-41c0-a343-876608fc7fca"
        }
      ]
    },
    {
      "id": "6b03ed73-2658-4d47-b9a3-a573874b1262",
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
          "id": "fd57125f-f92f-4831-bd39-0b7ae2efb1ed"
        }
      ]
    },
    {
      "id": "6f17aa30-1dff-43f0-87d6-42d2056dff0a",
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
          "id": "a892ca2f-25e8-4ace-92f0-b122aff7df11"
        }
      ]
    },
    {
      "id": "372e85b4-1aa4-4c3a-b28c-9823d26047dd",
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
          "id": "ceffb7de-1bc9-4b96-a785-157761cb8ec2"
        }
      ]
    },
    {
      "id": "9a4ede52-de07-468a-ab38-de6fd167a561",
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
          "id": "ef3944d6-413c-4d60-8d06-a5cd49db42f3"
        }
      ]
    },
    {
      "id": "da0a48e8-1a88-43a3-9198-236df3d60f8b",
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
          "id": "c5174d8b-5366-4d07-94a9-8613fc8e357c"
        }
      ]
    },
    {
      "id": "7749aff7-3f17-4005-8775-6567c00eb4be",
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
          "id": "36570a0c-96dc-47cd-8a1f-a3de39425f4c"
        }
      ]
    },
    {
      "id": "4984573c-3210-44ae-bffa-2dbcaab2e4f0",
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
          "id": "c8d911bf-0365-497d-baba-b2a93f54a36d"
        }
      ]
    },
    {
      "id": "2a43f756-8616-4829-a4f5-0c3642c642e3",
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
          "id": "d359e6da-8cc9-4c6b-8738-8af28480c3dd"
        }
      ]
    },
    {
      "id": "b5a737c3-4c5f-4f06-beda-6d2cb2879229",
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
          "id": "9e583656-ffab-4703-806e-764416ce4846"
        }
      ]
    },
    {
      "id": "eb17a398-1f4f-4928-ad4d-3005e85477f1",
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
          "id": "61276f58-6657-473c-b5a3-5d0a1c48de7b"
        }
      ]
    },
    {
      "id": "1960c123-3f86-40b9-91b9-d4dc472ceb4b",
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
          "id": "b9b118e4-b60c-404d-a415-05dee9a58fb6"
        }
      ]
    },
    {
      "id": "2ebe66e2-714a-42a6-b970-83f8d22fdf2a",
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
          "id": "00ab5ebd-8a44-4cd6-bbb8-a6aec0540fb2"
        }
      ]
    },
    {
      "id": "5b4137b9-56d6-4e63-b2e7-4c4c92a55d4d",
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
          "id": "637ed930-8524-4f36-a6b1-a7f73e355b6e"
        }
      ]
    },
    {
      "id": "d99e6ae3-7669-4938-88ce-67a2db7544c8",
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
          "id": "a87cbe42-e0ff-48c1-b991-25a24a4d846b"
        }
      ]
    },
    {
      "id": "125cb120-2cab-4f3c-8e95-e02ce98fe216",
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
          "id": "a8c73662-fdf2-46aa-8f06-bbf5550b3507"
        }
      ]
    },
    {
      "id": "122a8974-a381-4a95-8793-7b6ca79fc45d",
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
          "id": "7b1d2d3e-d9ef-4bc8-a042-bb1dc41ffad3"
        }
      ]
    }
  ]
}