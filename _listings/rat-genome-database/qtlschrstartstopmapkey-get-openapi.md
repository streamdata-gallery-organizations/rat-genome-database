---
swagger: "2.0"
x-collection-name: Rat Genome Database
x-complete: 0
info:
  title: Rat Genome Database Returns a list QTL for given position and assembly map
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
  /annotations/count/{accId}/{speciesTypeKey}/{includeChildren}:
    get:
      summary: Returns annotation count for ontology accession ID and speicies
      description: ""
      operationId: getAnnotationCountByAccIdAndSpeciesUsingGET
      x-api-path-slug: annotationscountaccidspeciestypekeyincludechildren-get
      parameters:
      - in: path
        name: accId
        description: Ontology term accession ID
      - in: path
        name: includeChildren
        description: 'true: return annotations for the term and children, false: return
          annotations for the term only'
      - in: path
        name: speciesTypeKey
        description: A list of species type keys can be found using the lookup service
      responses:
        200:
          description: OK
      tags:
      - ""
  /annotations/count/{accId}/{speciesTypeKey}/{includeChildren}/{objectType}:
    get:
      summary: Returns annotation count for ontology accession ID and object type
      description: ""
      operationId: getAnnotationCountByAccIdAndObjectTypeUsingGET
      x-api-path-slug: annotationscountaccidspeciestypekeyincludechildrenobjecttype-get
      parameters:
      - in: path
        name: accId
        description: Ontology term accession ID
      - in: path
        name: includeChildren
        description: 'true: return annotations for the term and children, false: return
          annotations for the term only'
      - in: path
        name: objectType
        description: A list of object types can be found using the lookup service
      - in: path
        name: speciesTypeKey
        description: A list of species type keys can be found using the lookup service
      responses:
        200:
          description: OK
      tags:
      - ""
  /annotations/reference/{refRgdId}:
    get:
      summary: Returns a list of annotations for a reference
      description: ""
      operationId: getAnnotsByRefrerenceUsingGET
      x-api-path-slug: annotationsreferencerefrgdid-get
      parameters:
      - in: path
        name: refRgdId
        description: Reference RGD ID
      responses:
        200:
          description: OK
      tags:
      - ""
  /annotations/rgdId/{rgdId}:
    get:
      summary: Returns a list of annotations by RGD ID
      description: ""
      operationId: getAnnotationsByRgdIdUsingGET
      x-api-path-slug: annotationsrgdidrgdid-get
      parameters:
      - in: path
        name: rgdId
        description: RGD ID
      responses:
        200:
          description: OK
      tags:
      - ""
  /annotations/rgdId/{rgdId}/{ontologyPrefix}:
    get:
      summary: Returns a list of annotations by RGD ID and ontology prefix
      description: ""
      operationId: getAnnotationsByRgdIdAndOntologyUsingGET
      x-api-path-slug: annotationsrgdidrgdidontologyprefix-get
      parameters:
      - in: path
        name: ontologyPrefix
        description: Ontology Prefix
      - in: path
        name: rgdId
        description: RGD ID
      responses:
        200:
          description: OK
      tags:
      - ""
  /annotations/{accId}/{rgdId}:
    get:
      summary: Returns a list of annotations by RGD ID and ontology term accession
        ID
      description: ""
      operationId: getAnnotationsByAccIdAndRgdIdUsingGET
      x-api-path-slug: annotationsaccidrgdid-get
      parameters:
      - in: path
        name: accId
        description: Ontology Term Accession ID
      - in: path
        name: rgdId
        description: RGD ID
      responses:
        200:
          description: OK
      tags:
      - ""
  /annotations/{accId}/{speciesTypeKey}/{includeChildren}:
    get:
      summary: Returns a list annotations for an ontology term or a term and it's
        children
      description: ""
      operationId: getAnnotationsUsingGET
      x-api-path-slug: annotationsaccidspeciestypekeyincludechildren-get
      parameters:
      - in: path
        name: accId
        description: Ontology term accession ID
      - in: path
        name: includeChildren
        description: 'true: return annotations for the term and children, false: return
          annotations for the term only'
      - in: path
        name: speciesTypeKey
        description: A list of species type keys can be found using the lookup service
      responses:
        200:
          description: OK
      tags:
      - ""
  /genes/affyId/{affyId}/{speciesTypeKey}:
    get:
      summary: Return a list of genes for an affymetrix ID
      description: ""
      operationId: getGenesByAffyIdUsingGET
      x-api-path-slug: genesaffyidaffyidspeciestypekey-get
      parameters:
      - in: path
        name: affyId
        description: Affymetrix ID
      - in: path
        name: speciesTypeKey
        description: A list of RGD species type keys can be found in the lookup service
      responses:
        200:
          description: OK
      tags:
      - ""
  /genes/alias/{aliasSymbol}/{speciesTypeKey}:
    get:
      summary: Return a list of genes for an alias and species
      description: ""
      operationId: getGenesByAliasSymbolUsingGET
      x-api-path-slug: genesaliasaliassymbolspeciestypekey-get
      parameters:
      - in: path
        name: aliasSymbol
        description: Gene alias symbol
      - in: path
        name: speciesTypeKey
        description: A list of RGD species type keys can be found in the lookup service
      responses:
        200:
          description: OK
      tags:
      - ""
  /genes/allele/{rgdId}:
    get:
      summary: Return a list of gene alleles
      description: ""
      operationId: getGeneAllelesUsingGET
      x-api-path-slug: genesallelergdid-get
      parameters:
      - in: path
        name: rgdId
        description: RGD ID of gene
      responses:
        200:
          description: OK
      tags:
      - ""
  /genes/annotation/{accId}/{speciesTypeKey}:
    get:
      summary: Return a list of genes annotated to an ontology term
      description: ""
      operationId: getGenesAnnotatedUsingGET
      x-api-path-slug: genesannotationaccidspeciestypekey-get
      parameters:
      - in: path
        name: accId
        description: Ontology term accession ID
      - in: path
        name: speciesTypeKey
        description: Species type key
      responses:
        200:
          description: OK
      tags:
      - ""
  /genes/keyword/{keyword}/{speciesTypeKey}:
    get:
      summary: Return a list of genes by keyword and species type key
      description: ""
      operationId: getGenesByKeywordUsingGET
      x-api-path-slug: geneskeywordkeywordspeciestypekey-get
      parameters:
      - in: path
        name: keyword
        description: Search keyword
      - in: path
        name: speciesTypeKey
        description: Species type key
      responses:
        200:
          description: OK
      tags:
      - ""
  /genes/map/{mapKey}:
    get:
      summary: Return a list of all genes with position information for an assembly
      description: ""
      operationId: getGeneByMapKeyUsingGET
      x-api-path-slug: genesmapmapkey-get
      parameters:
      - in: path
        name: mapKey
        description: A list of RGD assembly map keys can be found in the lookup service
      responses:
        200:
          description: OK
      tags:
      - ""
  /genes/ortholog/{rgdId}:
    get:
      summary: Return a list of gene orthologs
      description: ""
      operationId: getGeneOrthologsUsingGET
      x-api-path-slug: genesorthologrgdid-get
      parameters:
      - in: path
        name: rgdId
        description: RGD ID of a gene
      responses:
        200:
          description: OK
      tags:
      - ""
  /genes/species/{speciesTypeKey}:
    get:
      summary: Return a list of all genes for a species in RGD
      description: ""
      operationId: getGenesBySpeciesUsingGET
      x-api-path-slug: genesspeciesspeciestypekey-get
      parameters:
      - in: path
        name: speciesTypeKey
        description: A list of RGD species type keys can be found in the lookup service
      responses:
        200:
          description: OK
      tags:
      - ""
  /genes/{chr}/{start}/{stop}/{mapKey}:
    get:
      summary: Return a list of genes position and map key
      description: ""
      operationId: getGenesByPositionUsingGET
      x-api-path-slug: geneschrstartstopmapkey-get
      parameters:
      - in: path
        name: chr
        description: Chromosome
      - in: path
        name: mapKey
        description: A list of RGD assembly map keys can be found in the lookup service
      - in: path
        name: start
        description: Start Position
      - in: path
        name: stop
        description: Stop Position
      responses:
        200:
          description: OK
      tags:
      - ""
  /genes/{rgdId}:
    get:
      summary: Get a gene record by RGD ID
      description: ""
      operationId: getGeneByRgdIdUsingGET
      x-api-path-slug: genesrgdid-get
      parameters:
      - in: path
        name: rgdId
        description: The RGD ID of a Gene in RGD
      responses:
        200:
          description: OK
      tags:
      - ""
  /genes/{symbol}/{speciesTypeKey}:
    get:
      summary: Get a gene record by symbol and species type key
      description: ""
      operationId: getGeneBySymbolUsingGET
      x-api-path-slug: genessymbolspeciestypekey-get
      parameters:
      - in: path
        name: speciesTypeKey
        description: Species type key
      - in: path
        name: symbol
        description: Gene Symbol
      responses:
        200:
          description: OK
      tags:
      - ""
  /lookup/geneTypes:
    get:
      summary: Returns a list of gene types avialable in RGD
      description: ""
      operationId: getGeneTypesUsingGET
      x-api-path-slug: lookupgenetypes-get
      responses:
        200:
          description: OK
      tags:
      - ""
  /lookup/maps/{speciesTypeKey}:
    get:
      summary: Return a list assembly maps for a species
      description: ""
      operationId: getMapsUsingGET
      x-api-path-slug: lookupmapsspeciestypekey-get
      parameters:
      - in: path
        name: speciesTypeKey
        description: RGD species type key
      responses:
        200:
          description: OK
      tags:
      - ""
  /lookup/speciesTypeKeys:
    get:
      summary: Return a Map of species type keys available in RGD
      description: ""
      operationId: getSpeciesTypesUsingGET
      x-api-path-slug: lookupspeciestypekeys-get
      responses:
        200:
          description: OK
      tags:
      - ""
  /pathways/diagrams/search/{searchString}:
    get:
      summary: Return a list of pathways based on search term
      description: ""
      operationId: searchPathwaysUsingGET
      x-api-path-slug: pathwaysdiagramssearchsearchstring-get
      parameters:
      - in: path
        name: searchString
        description: Free text search string
      responses:
        200:
          description: OK
      tags:
      - ""
  /pathways/diagramsForCategory/{category}:
    get:
      summary: Return a list of pathways based on category provided
      description: ""
      operationId: getPathwaysWithDiagramsForCategoryUsingGET
      x-api-path-slug: pathwaysdiagramsforcategorycategory-get
      parameters:
      - in: path
        name: category
        description: Pathway Category
      responses:
        200:
          description: OK
      tags:
      - ""
  /phenotype/phenominer/chart/{speciesTypeKey}/{termString}:
    get:
      summary: Return a list of pathways based on search term and species type.  3=rat
        4=chinchilla
      description: ""
      operationId: getChartInfoUsingGET
      x-api-path-slug: phenotypephenominerchartspeciestypekeytermstring-get
      parameters:
      - in: path
        name: speciesTypeKey
        description: Species Type Key - 3=rat 4=chinchilla
      - in: path
        name: termString
        description: List of term accession IDs
      responses:
        200:
          description: OK
      tags:
      - ""
  /qtls/{chr}/{start}/{stop}/{mapKey}:
    get:
      summary: Returns a list QTL for given position and assembly map
      description: ""
      operationId: getQtlListByPositionUsingGET
      x-api-path-slug: qtlschrstartstopmapkey-get
      parameters:
      - in: path
        name: chr
        description: Chromosome
      - in: path
        name: mapKey
        description: A list of assembly map keys can be found using the lookup service
      - in: path
        name: start
        description: Start Position
      - in: path
        name: stop
        description: Stop Position
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