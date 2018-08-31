---
swagger: "2.0"
x-collection-name: GSA Per Diem API
x-complete: 0
info:
  title: GSA Per Diem API Per Diem Rates
  description: GSA sets rates for geographic areas it determines called primary destinations.
    Areas outside the primary destinations are covered by the same, nation-wide standard
    rate.
  version: 1.0.0
host: inventory.data.gov
basePath: /api/action/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /datastore_search?resource_id=8ea44bc4-22ba-4386-b84c-1494ab28964b:
    get:
      summary: Per Diem Rates
      description: GSA sets rates for geographic areas it determines called primary
        destinations. Areas outside the primary destinations are covered by the same,
        nation-wide standard rate.
      operationId: getPerDiemRates
      x-api-path-slug: datastore-searchresource-id8ea44bc422ba4386b84c1494ab28964b-get
      parameters:
      - in: query
        name: filters
        description: FiscalYear, Zip, State, DestinationID, City, County, Month, Meals
        type: string
        format: string
      responses:
        200:
          description: OK
      tags:
      - Per Diem Rates
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