---
swagger: "2.0"
x-collection-name: Xignite
x-complete: 0
info:
  title: Xignite VWAP Get Delayed VWAP
  description: Returns an intraday VWAP for a security based on all trades for the
    day up to the 15/20 minutes delayed quote.
  version: 1.0.0
host: www.xignite.com
basePath: xVWAP.json/XigniteVWAP
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /GetDelayedVWAP:
    get:
      summary: Get Delayed VWAP
      description: Returns an intraday VWAP for a security based on all trades for
        the day up to the 15/20 minutes delayed quote.
      operationId: GetDelayedVWAP
      x-api-path-slug: getdelayedvwap-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Delayed
      - VWAP
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