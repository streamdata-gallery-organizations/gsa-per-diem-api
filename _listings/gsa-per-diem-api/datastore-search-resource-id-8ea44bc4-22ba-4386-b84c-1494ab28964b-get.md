---
swagger: "2.0"
info:
  title: GSA Per Diem API
  description: Per Diem Rates are the allowed reimbursement rates for hotel stays
    and meals for federal travelers. Rates are set for each of the federal government's
    fiscal years (FY 2014 is October 1, 2013 to September 30, 2014.) GSA is responsible
    for setting the rates in the continental United States.  Many businesses and other
    organizations adopt these rates as well. GSA is making the rates available using
    the CKAN's Action API via Data.gov to allow software developers programmatic access
    the data and create innovative uses for it.
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
        destinations
      operationId: getPerDiemRates
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
      - per diem rates
definitions: []
x-collection-name: GSA Per Diem API
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