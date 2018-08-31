---
swagger: "2.0"
x-collection-name: Hewlett Packard Enterprise (HPE)
x-complete: 0
info:
  title: HPE OneSphere API Delete Catalogs
  description: Delete a catalog and associated resources. **Not implemented**
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
    get:
      summary: Get Appliances
      description: Returns an appliance based on its ID.
      operationId: GetApplianceById
      x-api-path-slug: appliancesid-get
      parameters:
      - in: path
        name: id
        description: ID of the appliance to retrieve
      responses:
        200:
          description: OK
      tags:
      - Appliances
    patch:
      summary: Patch Appliances
      description: Update properties of an appliance.
      operationId: UpdateAppliance
      x-api-path-slug: appliancesid-patch
      parameters:
      - in: body
        name: body
        description: List of appliance updates
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: ID of appliance to update
      responses:
        200:
          description: OK
      tags:
      - Appliances
  /billing-accounts:
    get:
      summary: Get Billing Accounts
      description: Returns billing accounts. It requires the **administrator** or
        **project creator** global role.
      operationId: FindBillingAccounts
      x-api-path-slug: billingaccounts-get
      parameters:
      - in: query
        name: query
        description: Filters the billing accounts returned
      - in: query
        name: view
        description: Whether to return related content
      responses:
        200:
          description: OK
      tags:
      - Billing
      - Accounts
    post:
      summary: Post Billing Accounts
      description: Creates a new billing account. It requires the **administrator**
        role.
      operationId: CreateBillingAccount
      x-api-path-slug: billingaccounts-post
      parameters:
      - in: body
        name: billing-account
        description: Add new billing account
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Billing
      - Accounts
  /billing-accounts/{id}:
    delete:
      summary: Delete Billing Accounts
      description: Deletes a billing account. It requires the **administrator** role.
      operationId: DeleteBillingAccountById
      x-api-path-slug: billingaccountsid-delete
      parameters:
      - in: path
        name: id
        description: ID of billing account to delete
      responses:
        200:
          description: OK
      tags:
      - Billing
      - Accounts
    get:
      summary: Get Billing Accounts
      description: Returns a billing account based on its id. It requires the **administrator**
        or **project creator** global role. Credentials are not included.
      operationId: GetBillingAccountById
      x-api-path-slug: billingaccountsid-get
      parameters:
      - in: path
        name: id
        description: ID of billing account to fetch
      - in: query
        name: view
        description: Whether to return related content
      responses:
        200:
          description: OK
      tags:
      - Billing
      - Accounts
    patch:
      summary: Patch Billing Accounts
      description: Updates a billing account. It requires the **administrator** role.
      operationId: UpdateBillingAccount
      x-api-path-slug: billingaccountsid-patch
      parameters:
      - in: body
        name: body
        description: The JSON patch to apply to the billing account
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: ID of billing account to update
      responses:
        200:
          description: OK
      tags:
      - Billing
      - Accounts
  /catalog-types:
    get:
      summary: Get Catalog Types
      description: Returns catalog types.
      operationId: FindCatalogTypes
      x-api-path-slug: catalogtypes-get
      responses:
        200:
          description: OK
      tags:
      - Catalog
      - Types
  /catalogs:
    get:
      summary: Get Catalogs
      description: Returns catalogs. It requires the **consumer** global role.
      operationId: FindCatalogs
      x-api-path-slug: catalogs-get
      parameters:
      - in: query
        name: userQuery
        description: Filters the catalogs returned
      - in: query
        name: view
        description: 'Return related resources:  * `full` - Whether to return related
          content'
      responses:
        200:
          description: OK
      tags:
      - Catalogs
    post:
      summary: Post Catalogs
      description: Creates a new catalog.
      operationId: CreateCatalog
      x-api-path-slug: catalogs-post
      parameters:
      - in: body
        name: catalog
        description: Add new catalog
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Catalogs
  /catalogs/{id}:
    delete:
      summary: Delete Catalogs
      description: Delete a catalog and associated resources. **Not implemented**
      operationId: DeleteCatalog
      x-api-path-slug: catalogsid-delete
      parameters:
      - in: path
        name: id
        description: ID of catalog to delete
      responses:
        200:
          description: OK
      tags:
      - Catalogs
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