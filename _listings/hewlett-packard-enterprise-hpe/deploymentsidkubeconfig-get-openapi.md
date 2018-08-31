---
swagger: "2.0"
x-collection-name: Hewlett Packard Enterprise (HPE)
x-complete: 0
info:
  title: HPE OneSphere API Get Deployments Kubeconfig
  description: Returns the kubeconfig. Applicable only to deployments of Kubernetes
    cluster. **Requires 'consumer' role on workspace**
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
    get:
      summary: Get Catalogs
      description: Returns a catalog based on its id. It requires the **consumer**
        global role.
      operationId: GetCatalogById
      x-api-path-slug: catalogsid-get
      parameters:
      - in: path
        name: id
        description: ID of catalog to fetch
      - in: query
        name: view
        description: 'Return related resources:  * `full` - Whether to return related
          content'
      responses:
        200:
          description: OK
      tags:
      - Catalogs
    patch:
      summary: Patch Catalogs
      description: Patches a catalog. Allowed fields for PATCH of catalogs are name(add,replace),
        password(add), accessKey(add), secretKey(add), state(add,replace)
      operationId: UpdateCatalog
      x-api-path-slug: catalogsid-patch
      parameters:
      - in: body
        name: catalog
        description: Update catalog
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: ID of catalog to update
      responses:
        200:
          description: OK
      tags:
      - Catalogs
  /connect-app:
    get:
      summary: Get Connect App
      description: Generates connect app s3 url
      operationId: connect-app
      x-api-path-slug: connectapp-get
      parameters:
      - in: query
        name: os
        description: OS type for which compatible connect app URL has to be generated
      responses:
        200:
          description: OK
      tags:
      - Connect
      - App
  /deployments:
    get:
      summary: Get Deployments
      description: Returns deployments. It requires any project role or non-'consumer'
        global role.
      operationId: FindDeployments
      x-api-path-slug: deployments-get
      parameters:
      - in: query
        name: query
        description: Filters the deployments returned
      - in: query
        name: userQuery
        description: Filters the deployments returned
      - in: query
        name: view
        description: 'Return related resources:  * `full` - include zone, service,
          volume details'
      responses:
        200:
          description: OK
      tags:
      - Deployments
    post:
      summary: Post Deployments
      description: Creates a new deployment. It requires any project role, or the
        **administrator** or **project creator** global role.
      operationId: CreateDeployment
      x-api-path-slug: deployments-post
      parameters:
      - in: body
        name: deployment
        description: Add new deployment
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Deployments
  /deployments/{id}:
    delete:
      summary: Delete Deployments
      description: Delete a deployment and associated resources. It requires any project
        role, or the **administrator** or **project creator** global role.
      operationId: DeleteDeployment
      x-api-path-slug: deploymentsid-delete
      parameters:
      - in: path
        name: id
        description: ID of deployment to delete
      responses:
        200:
          description: OK
      tags:
      - Deployments
    get:
      summary: Get Deployments
      description: Returns a deployment based on its id. It requires any project role
        or non-'consumer' global role.
      operationId: GetDeploymentById
      x-api-path-slug: deploymentsid-get
      parameters:
      - in: path
        name: id
        description: ID of deployment to fetch
      - in: query
        name: view
        description: 'Return related resources:  * `full` - include region, zone,
          service, virtual machine profile,  firewall, volume details'
      responses:
        200:
          description: OK
      tags:
      - Deployments
    patch:
      summary: Patch Deployments
      description: Updates a deployment. **Requires any project role, or 'administrator'
        or 'project creator' global role**. Allowed fields for PATCH of deployments
        are name(add,replace), volumes(add), k8snumWorkers(add), userData(add), serviceInput(add),
        version(add).
      operationId: UpdateDeployment
      x-api-path-slug: deploymentsid-patch
      parameters:
      - in: body
        name: deployment
        description: Update deployment
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: ID of deployment to update
      responses:
        200:
          description: OK
      tags:
      - Deployments
  /deployments/{id}/actions:
    post:
      summary: Post Deployments Actions
      description: Peforms an action to change the state of a deployment. It requires
        any project role, or the **administrator** or **project creator** global role.
      operationId: ActOnDeployment
      x-api-path-slug: deploymentsidactions-post
      parameters:
      - in: body
        name: action
        description: Action to perform
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: ID of deployment to act on
      responses:
        200:
          description: OK
      tags:
      - Deployments
      - Actions
  /deployments/{id}/console:
    post:
      summary: Post Deployments Console
      description: Returns a deployment console URL for deployment
      operationId: GetDeploymentConsoleURL
      x-api-path-slug: deploymentsidconsole-post
      parameters:
      - in: path
        name: id
        description: ID of deployment for which console URL is required
      responses:
        200:
          description: OK
      tags:
      - Deployments
      - Console
  /deployments/{id}/kubeconfig:
    get:
      summary: Get Deployments Kubeconfig
      description: Returns the kubeconfig. Applicable only to deployments of Kubernetes
        cluster. **Requires 'consumer' role on workspace**
      operationId: GetDeploymentKubeConfig
      x-api-path-slug: deploymentsidkubeconfig-get
      parameters:
      - in: path
        name: id
        description: ID of deployment for which kubeconfig is required
      responses:
        200:
          description: OK
      tags:
      - Deployments
      - Kubeconfig
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