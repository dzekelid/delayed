---
swagger: "2.0"
x-collection-name: Xignite
x-complete: 1
info:
  title: Xignite VWAP
  description: provides-delayed-and-historical-volumeweightedaverage-price-vwap-information-
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
---