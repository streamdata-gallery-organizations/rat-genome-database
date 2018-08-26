{
  "info": {
    "name": "Rat Genome Database Count of gene types, for specified species and date",
    "_postman_id": "c8382d2a-9462-4b99-b13c-7270e06189e5",
    "description": "",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "id": "0621c99f-fb5f-460a-9a7d-3127e05f52d3",
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
          "id": "1e0ca5fb-f486-439d-9def-28c7259a5230"
        }
      ]
    },
    {
      "id": "c2e3b0b4-2928-49cf-972c-53bd58859fcb",
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
          "id": "006cb8d7-890d-47a6-8b58-1418b747575f"
        }
      ]
    },
    {
      "id": "4e92f67e-f2c0-45fc-9766-7806e378df75",
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
          "id": "f99754ef-0269-4344-a061-f14ee6f4e05e"
        }
      ]
    },
    {
      "id": "861e86d9-ad0d-4b63-a72c-bdf16e253151",
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
          "id": "e93187ba-fe41-4a12-b909-640d7af6e9c1"
        }
      ]
    },
    {
      "id": "c2d627f5-2d12-493d-91fa-16cf3000d413",
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
          "id": "3733b29c-bf4f-441a-ba94-f6c02daed5d0"
        }
      ]
    },
    {
      "id": "80f8b803-4f29-4187-857f-844bb2b18d69",
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
          "id": "1606ba71-6c89-4029-a0ad-c8ed0b3feec1"
        }
      ]
    },
    {
      "id": "3c1c46a1-7c98-4074-ad72-dd235865ad6b",
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
          "id": "0f494c75-f8e7-448b-9186-ed98ab6d901e"
        }
      ]
    },
    {
      "id": "0366fcfd-72c4-4c2d-9b1f-c5ca028ef12a",
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
          "id": "f065e86a-0678-4814-a4e5-fe8c3410f46f"
        }
      ]
    },
    {
      "id": "9d6d14fa-f538-4210-bc2f-55cb626d2383",
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
          "id": "ec79597f-ed49-492a-998d-ff58ec3e5a1a"
        }
      ]
    },
    {
      "id": "2e6c1666-16d4-49aa-9162-2d9b6ab14ada",
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
          "id": "f0ec4df4-a100-4879-9b2b-772d8d1a35f1"
        }
      ]
    },
    {
      "id": "71934464-de63-441e-a33c-9ffb7120325d",
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
          "id": "dc13d58e-60b7-4b20-8a5c-4bc61b43ae82"
        }
      ]
    },
    {
      "id": "5d84f437-0e31-4b60-bef4-35baf64dac2a",
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
          "id": "e04931aa-df90-4ee8-a071-cce8b2d19eb5"
        }
      ]
    },
    {
      "id": "81544fa6-abeb-4ac6-a293-d8e70759b6c3",
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
          "id": "f18f160b-8ba1-40e7-8065-9ea673bef953"
        }
      ]
    },
    {
      "id": "51e75225-690c-4a00-aea5-190c2d02289b",
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
          "id": "dddfecf7-6adb-4718-bd7c-29b0c70e7c1e"
        }
      ]
    },
    {
      "id": "e12a0aff-3a7e-4c28-bfad-13f868cdf798",
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
          "id": "471ccb58-6f00-412d-bee7-ebd50383ef0f"
        }
      ]
    },
    {
      "id": "ad6a472d-6078-42fe-b673-cfe6c20f1250",
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
          "id": "1474c74a-d49a-43fd-a629-c7dd9535edc0"
        }
      ]
    },
    {
      "id": "d1d0c47e-6cda-4c26-b19f-8d0c7b045eff",
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
          "id": "ee9243fe-df9a-45ca-99f5-dd42902fa5f2"
        }
      ]
    },
    {
      "id": "e28a7d2a-75db-4935-b132-0abe52e40bbb",
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
          "id": "0808c034-0bf8-477e-8534-83a123b0ea3d"
        }
      ]
    },
    {
      "id": "3e0bd064-6ba9-447d-b2b2-8000ecb0c326",
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
          "id": "80d05705-7d3f-4d37-9c57-581aec1e53de"
        }
      ]
    },
    {
      "id": "7d1bfdfd-efe2-4220-a0c6-2d47448a8a79",
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
          "id": "b6f3b6ea-63d3-4503-85df-fb52597cb4c9"
        }
      ]
    },
    {
      "id": "51587e60-55af-4299-bab1-158951f05b55",
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
          "id": "95ba7853-cfc3-4936-a6d3-8993e894f1a3"
        }
      ]
    },
    {
      "id": "f075bd4c-afe8-4b0e-9e10-6c456765c9c2",
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
          "id": "73880330-fcf6-4e5a-8145-90c835814fa5"
        }
      ]
    },
    {
      "id": "dc5b5d27-5a27-45f3-8ae0-63baf2b3d4e6",
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
          "id": "84d23fd9-383d-40f7-9e2a-049d0239957d"
        }
      ]
    },
    {
      "id": "a5e09caf-9611-431e-bb2b-cbdbafb5b9d4",
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
          "id": "e5a2db3d-d53b-4284-99a1-e69b64576ed1"
        }
      ]
    },
    {
      "id": "008d71cd-70df-4ca9-982e-ce7fb130f256",
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
          "id": "cc9f03d5-bb06-4ed9-b9cb-6ef63e7b72af"
        }
      ]
    },
    {
      "id": "e7181e49-6386-459e-8bb4-57facac952e5",
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
          "id": "183f0553-6d90-4b11-8888-4a2f359a2ef7"
        }
      ]
    },
    {
      "id": "8387b140-f369-44de-9628-da25bc5b07ff",
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
          "id": "69e6f493-9a08-4e52-9236-cb480bd9354b"
        }
      ]
    },
    {
      "id": "fa1c95f8-4c78-44b6-8eec-a621463dd97b",
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
          "id": "16cbf1bc-ae1a-45dd-b453-6d1774aa05df"
        }
      ]
    },
    {
      "id": "1e45bc56-3980-42cb-ba3f-201b5160a268",
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
          "id": "64f5252b-d454-4f7c-91c0-fc8a0f871836"
        }
      ]
    },
    {
      "id": "1627f1f6-e342-4fd7-aa41-c6a81d342f2f",
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
          "id": "31621dc1-6314-41af-98e7-84146e69f274"
        }
      ]
    }
  ]
}