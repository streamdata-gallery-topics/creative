---
swagger: "2.0"
x-collection-name: Google Doubleclick
x-complete: 0
info:
  title: Google Doubleclick API Get Creatives
  version: 1.0.0
  description: Retrieves a list of the authenticated user's active creatives. A creative
    will be available 30-40 minutes after submission.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /creatives:
    get:
      summary: Get Creatives
      description: Retrieves a list of the authenticated user's active creatives.
        A creative will be available 30-40 minutes after submission.
      operationId: adexchangebuyer.creatives.list
      x-api-path-slug: creatives-get
      parameters:
      - in: query
        name: accountId
        description: When specified, only creatives for the given account ids are
          returned
      - in: query
        name: buyerCreativeId
        description: When specified, only creatives for the given buyer creative ids
          are returned
      - in: query
        name: dealsStatusFilter
        description: When specified, only creatives having the given deals status
          are returned
      - in: query
        name: maxResults
        description: Maximum number of entries returned on one result page
      - in: query
        name: openAuctionStatusFilter
        description: When specified, only creatives having the given open auction
          status are returned
      - in: query
        name: pageToken
        description: A continuation token, used to page through ad clients
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Creative
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