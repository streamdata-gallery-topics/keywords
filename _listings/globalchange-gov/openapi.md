swagger: "2.0"
x-collection-name: GlobalChange.gov
x-complete: 1
info:
  title: Global Change Information System API
  description: who-we-are-what-the-gcis-is-and-how-we-use-identifiers-and-semantic-information-to-provide-points-of-reference-and-traceability--examples-and-tutorials-for-using-this-system-as-a-researcher-citizen-scientist-application-developer-or-information-theorist--a-description-of-how-the-information-is-structured-including-the-overlaps-between-relational-and-semantic-representations-of-the-information--complete-documentation-for-the-api-including-methods-for-browsing-and-finding-resources-
  version: v1
host: data.globalchange.gov
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /gcmd_keyword:
    get:
      summary: List GCMD keywords in the GCIS.
      description: List the GCMD keywords in the GCIS, 20 per page.
      operationId: list-the-gcmd-keywords-in-the-gcis-20-per-page
      x-api-path-slug: gcmd-keyword-get
      parameters:
      - in: query
        name: page
        description: The page number (starting at 1)
      responses:
        200:
          description: OK
      tags:
      - GCMD
      - Keywords
      - GCIS
  /gcmd_keyword/{gcmd_keyword_identifier}:
    get:
      summary: Get a representation of a GCMD keyword.
      description: Get JSON which represents the structure of a GCMD keyword.
      operationId: get-json-which-represents-the-structure-of-a-gcmd-keyword
      x-api-path-slug: gcmd-keywordgcmd-keyword-identifier-get
      parameters:
      - in: path
        name: gcmd_keyword_identifier
        description: gcmd_keyword_identifier description
      responses:
        200:
          description: OK
      tags:
      - Representation
      - GCMD
      - Keyword