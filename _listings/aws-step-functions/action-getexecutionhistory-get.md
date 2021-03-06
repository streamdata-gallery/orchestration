---
swagger: "2.0"
info:
  title: AWS Step Functions API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=GetExecutionHistory&k=1:
    get:
      summary: ' Get Execution History '
      description: Returns the history of the specified execution as a list of events
      operationId: getExecutionHistory
      parameters:
      - in: query
        name: executionArn
        description: The Amazon Resource Name (ARN) of the execution
        type: string
      - in: query
        name: maxResults
        description: The maximum number of results that will be returned per call
        type: string
      - in: query
        name: nextToken
        description: If a nextToken was returned by a previous call, there are more
          results available
        type: string
      - in: query
        name: reverseOrder
        description: Lists events in descending order of their timeStamp
        type: string
      responses:
        200:
          description: OK
      tags:
      - execution
definitions: []
x-collection-name: AWS Step Functions
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