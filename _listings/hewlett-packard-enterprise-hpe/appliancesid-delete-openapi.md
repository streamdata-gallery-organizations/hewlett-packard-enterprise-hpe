---
swagger: "2.0"
x-collection-name: Hewlett Packard Enterprise (HPE)
x-complete: 0
info:
  title: HPE OneSphere API Delete Appliances
  description: |-
    Delete an appliance.
    This removes the appliance registration and tears down the secure
    comms link to the on-premise appliance.
    If zones exist on this appliance, an '409' error will be returned.
    The zones on this appliance must be removed before the appliance
    delete request can be accepted.
  termsOfService: http://www.hpe.com/onesphere
  contact:
    name: HPE OneSphere API team
    url: http://www.hpe.com/onesphere
  version: 1.0.0
host: deic02-hpe.hpeonesphere.com
basePath: /rest
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /about/versions:
    get:
      summary: Get About Versions
      description: Get supported versions
      operationId: GetVersions
      x-api-path-slug: aboutversions-get
      responses:
        200:
          description: OK
      tags:
      - About
      - Versions
  /account:
    get:
      summary: Get Account
      description: Returns the global account information. **Not implemented**
      operationId: GetAccount
      x-api-path-slug: account-get
      parameters:
      - in: query
        name: view
        description: Whether to return related content
      responses:
        200:
          description: OK
      tags:
      - Account
  /appliances:
    get:
      summary: Get Appliances
      description: Returns appliances.
      operationId: GetAppliance
      x-api-path-slug: appliances-get
      parameters:
      - in: query
        name: name
        description: The name of the desired appliance
      - in: query
        name: regionUri
        description: Set of appliances in this region
      responses:
        200:
          description: OK
      tags:
      - Appliances
    post:
      summary: Post Appliances
      description: Create an appliance.
      operationId: CreateAppliance
      x-api-path-slug: appliances-post
      parameters:
      - in: body
        name: appliance
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Appliances
  /appliances/{id}:
    delete:
      summary: Delete Appliances
      description: |-
        Delete an appliance.
        This removes the appliance registration and tears down the secure
        comms link to the on-premise appliance.
        If zones exist on this appliance, an '409' error will be returned.
        The zones on this appliance must be removed before the appliance
        delete request can be accepted.
      operationId: DeleteAppliance
      x-api-path-slug: appliancesid-delete
      parameters:
      - in: path
        name: id
        description: ID of the appliance to delete
      responses:
        200:
          description: OK
      tags:
      - Appliances
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