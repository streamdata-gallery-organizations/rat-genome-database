---
swagger: "2.0"
x-collection-name: Rat Genome Database
x-complete: 0
info:
  title: Rat Genome Database Returns annotation count for ontology accession ID
  description: ""
  termsOfService: http://rgd.mcw.edu/wg/citing-rgd
  contact:
    name: Rat Genome Database
    url: http://rgd.mcw.edu
    email: RGD.Data2@mcw.edu
  version: "1.1"
host: rest.rgd.mcw.edu
basePath: /rgdws
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /annotations/accId/{rgdId}:
    get:
      summary: Returns a list ontology term accession IDs annotated to an rgd object
      description: ""
      operationId: getTermAccIdsUsingGET
      x-api-path-slug: annotationsaccidrgdid-get
      parameters:
      - in: path
        name: rgdId
        description: RGD ID
      responses:
        200:
          description: OK
      tags:
      - ""
  /annotations/count/{accId}/{includeChildren}:
    get:
      summary: Returns annotation count for ontology accession ID
      description: ""
      operationId: getAnnotationCountByAccIdUsingGET
      x-api-path-slug: annotationscountaccidincludechildren-get
      parameters:
      - in: path
        name: accId
        description: Ontology term accession ID
      - in: path
        name: includeChildren
        description: 'true: return annotations for the term and children, false: return
          annotations for the term only'
      responses:
        200:
          description: OK
      tags:
      - ""
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---