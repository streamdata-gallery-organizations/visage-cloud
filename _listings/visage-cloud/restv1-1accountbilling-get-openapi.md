---
swagger: "2.0"
x-collection-name: Visage Cloud
x-complete: 0
info:
  title: Visage Cloud Get billing information by accessKey and secretKey
  description: ""
  termsOfService: https://visagecloud.com/terms-of-use
  contact:
    name: VisageCloud
    url: https://visagecloud.com
    email: office@visagecloud.com
  version: "1.1"
host: visagecloud.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /rest/v1.1/account/account:
    get:
      summary: Get account information by accessKey and secretKey
      description: ""
      operationId: getAccountByAccessKeyUsingGET
      x-api-path-slug: restv1-1accountaccount-get
      parameters:
      - in: query
        name: accessKey
        description: accessKey
      - in: query
        name: secretKey
        description: secretKey
      responses:
        200:
          description: OK
      tags:
      - ""
  /rest/v1.1/account/billing:
    get:
      summary: Get billing information by accessKey and secretKey
      description: ""
      operationId: getBillingPerAccountUsingGET
      x-api-path-slug: restv1-1accountbilling-get
      parameters:
      - in: query
        name: accessKey
        description: accessKey
      - in: query
        name: dateTemplate
        description: dateTemplate
      - in: query
        name: endDateTime
        description: endDateTime
      - in: query
        name: secretKey
        description: secretKey
      - in: query
        name: startDateTime
        description: startDateTime
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