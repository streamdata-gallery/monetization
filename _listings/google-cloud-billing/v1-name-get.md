---
swagger: "2.0"
info:
  title: Google Cloud Billing
  description: Allows developers to manage billing for their Google Cloud Platform
    projects    programmatically.
  contact:
    name: Google
    url: https://google.com
  version: v1
host: cloudbilling.googleapis.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v1/{name}:
    get:
      summary: Get Billing Account
      description: Gets information about a billing account
      operationId: cloudbilling.billingAccounts.get
      parameters:
      - in: path
        name: name
        description: The resource name of the billing account to retrieve
      responses:
        200:
          description: OK
      tags:
      - account
definitions:
  BillingAccount:
    properties:
      displayName:
        description: This is a default description.
        type: parameters
      name:
        description: This is a default description.
        type: parameters
      open:
        description: This is a default description.
        type: parameters
  ListBillingAccountsResponse:
    properties:
      billingAccounts:
        description: This is a default description.
        type: parameters
      nextPageToken:
        description: This is a default description.
        type: parameters
  ListProjectBillingInfoResponse:
    properties:
      nextPageToken:
        description: This is a default description.
        type: parameters
      projectBillingInfo:
        description: This is a default description.
        type: parameters
  ProjectBillingInfo:
    properties:
      billingAccountName:
        description: This is a default description.
        type: parameters
      billingEnabled:
        description: This is a default description.
        type: parameters
      name:
        description: This is a default description.
        type: parameters
      projectId:
        description: This is a default description.
        type: parameters
x-collection-name: Google Cloud Billing
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