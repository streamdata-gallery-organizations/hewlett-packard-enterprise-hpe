---
swagger: "2.0"
x-collection-name: Hewlett Packard Enterprise (HPE)
x-complete: 0
info:
  title: HPE OneSphere API Post Zones Connections
  description: Peforms an action to the zone. It requires the **administrator** role.
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
  /events:
    get:
      summary: Get Events
      description: Returns events based on the supplied criteria. **Not implemented**
      operationId: FindEvents
      x-api-path-slug: events-get
      parameters:
      - in: query
        name: resourceUri
        description: Resource to prune events by
      responses:
        200:
          description: OK
      tags:
      - Events
  /keypairs:
    get:
      summary: Get Keypairs
      description: Get keypairs (per region, per user). Currently a projectUri is
        required
      operationId: ListKeypairs
      x-api-path-slug: keypairs-get
      parameters:
      - in: query
        name: projectUri
      - in: query
        name: regionUri
      responses:
        200:
          description: OK
      tags:
      - Keypairs
  /membership-roles:
    get:
      summary: Get Membership Roles
      description: Returns membership (project-specific) roles.
      operationId: ListMembershipRoles
      x-api-path-slug: membershiproles-get
      responses:
        200:
          description: OK
      tags:
      - Membership
      - Roles
  /memberships:
    delete:
      summary: Delete Memberships
      description: Delete a membership. It requires the **administrator** or **project
        creator** global role or the **project owner** role on the project.
      operationId: DeleteMember
      x-api-path-slug: memberships-delete
      parameters:
      - in: body
        name: membership
        description: Delete membership
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Memberships
    get:
      summary: Get Memberships
      description: |-
        Returns memberships. Supports filtering by projectUri, userUri, userGroupUri, roleUri (but only
        individual values, not multiple) in 'query'.

        If projectURI and userUri/userGroupUri are given a different
        backend path will be used that should be authorized to a project owner even if they wouldn't ordinarily
        be able to see other users' roles.

        It requires the **administrator** or **project creator** global role or the **project owner** role on the project.
        **project owner** requires **projectUri** to be supplied.
      operationId: FindMembers
      x-api-path-slug: memberships-get
      parameters:
      - in: query
        name: query
        description: URI query to prune memberships by
      responses:
        200:
          description: OK
      tags:
      - Memberships
    post:
      summary: Post Memberships
      description: Creates a new membership. It requires the **administrator** or
        **project creator** global role or **project owner** role on the project.
      operationId: CreateMember
      x-api-path-slug: memberships-post
      parameters:
      - in: body
        name: membership
        description: Add new membership
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Memberships
  /metrics:
    get:
      summary: Get Metrics
      description: |-
        Returns all metrics based on the supplied criteria. It requires the **analyst** role.
        It requires one and only one of resourceUri or category to be specified.
      operationId: FindMetrics
      x-api-path-slug: metrics-get
      parameters:
      - in: query
        name: category
        description: A category name
      - in: query
        name: count
        description: Maximum number of response members to return
      - in: query
        name: groupBy
        description: A value to group the data by
      - in: query
        name: name
        description: Name(s) of metrics to return
      - in: query
        name: period
        description: How much time to cover per data point
      - in: query
        name: periodCount
        description: How many period data points to return relative to the periodStart
          time
      - in: query
        name: periodStart
        description: When the metric value(s) should be measured from
      - in: query
        name: query
        description: A query to filter the resources by
      - in: query
        name: resourceUri
        description: Resource(s) to return metrics for
      - in: query
        name: start
        description: Index into the response members to allow pagination
      - in: query
        name: view
        description: Whether to return related content
      responses:
        200:
          description: OK
      tags:
      - Metrics
  /networks:
    get:
      summary: Get Networks
      description: Returns networks. It requires any project role or non-'consumer'
        global role.
      operationId: FindNetworks
      x-api-path-slug: networks-get
      parameters:
      - in: query
        name: query
        description: Filters the networks returned
      responses:
        200:
          description: OK
      tags:
      - Networks
  /networks/{id}:
    get:
      summary: Get Networks
      description: Returns a network based on its id. It requires any project role
        or non-'consumer' global role.
      operationId: GetNetworkById
      x-api-path-slug: networksid-get
      parameters:
      - in: path
        name: id
        description: ID of network to fetch
      - in: query
        name: query
        description: Filters the networks returned
      responses:
        200:
          description: OK
      tags:
      - Networks
    patch:
      summary: Patch Networks
      description: Updates a network. It requires the **administrator** global role.
      operationId: ModifyNetwork
      x-api-path-slug: networksid-patch
      parameters:
      - in: path
        name: id
        description: ID of the network to update
      - in: body
        name: network
        description: Update network
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Networks
  /onboarding/azure/properties:
    get:
      summary: Get Onboarding Azure Properties
      description: Returns a properties object needed to build the Azure login url
      operationId: GetAzureLoginProperties
      x-api-path-slug: onboardingazureproperties-get
      responses:
        200:
          description: OK
      tags:
      - Onboarding
      - Azure
      - Properties
  /onboarding/azure/provider-info:
    get:
      summary: Get Onboarding Azure Prover Info
      description: Returns the provider information required to add an Azure provider
      operationId: getAzureProviderInfo
      x-api-path-slug: onboardingazureproviderinfo-get
      parameters:
      - in: query
        name: directoryUri
        description: The Azure Directory URI associated with the SubscriptionFor Example:myActiveDirectory
      - in: query
        name: location
        description: The full response Azure sends to the redirectURI including valid
          Azure authentication codeFor Example:https://customername
      responses:
        200:
          description: OK
      tags:
      - Onboarding
      - Azure
      - Prover
      - Info
  /onboarding/azure/subscriptions:
    get:
      summary: Get Onboarding Azure Subscriptions
      description: Returns a list of Azure subscriptions and their display names
      operationId: ListAzureSubscriptions
      x-api-path-slug: onboardingazuresubscriptions-get
      parameters:
      - in: query
        name: directoryUri
        description: The Azure Directory URI associated with the SubscriptionFor Example:myActiveDirectory
      - in: query
        name: location
        description: The full response Azure sends to the redirectURI including valid
          Azure authentication codeFor Example:https://customername
      responses:
        200:
          description: OK
      tags:
      - Onboarding
      - Azure
      - Subscriptions
  /onboarding/azure/subscriptions/{subscriptionId}:
    patch:
      summary: Patch Onboarding Azure Subscriptions Subscriptionid
      description: Updates a subscription
      operationId: UpdateSubscription
      x-api-path-slug: onboardingazuresubscriptionssubscriptionid-patch
      parameters:
      - in: body
        name: body
        description: Update subscription
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: directoryUri
        description: The Azure Directory URI associated with the SubscriptionFor Example:myActiveDirectory
      - in: query
        name: location
        description: The full response Azure sends to the redirectURI including valid
          Azure authentication codeFor Example:https://customername
      - in: path
        name: subscriptionId
        description: The Azure subscriptionId
      responses:
        200:
          description: OK
      tags:
      - Onboarding
      - Azure
      - Subscriptions
      - Subscriptionid
  /password-reset:
    post:
      summary: Post Password Reset
      description: Request a single-use password reset token.
      operationId: CreatePasswordReset
      x-api-path-slug: passwordreset-post
      parameters:
      - in: body
        name: passwordResetRequest
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Password
      - Reset
  /password-reset/change:
    post:
      summary: Post Password Reset Change
      description: Process a password reset.
      operationId: ProcessPasswordReset
      x-api-path-slug: passwordresetchange-post
      parameters:
      - in: body
        name: passwordReset
        description: Password reset information
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Password
      - Reset
      - Change
  /projects:
    get:
      summary: Get Projects
      description: Returns projects. It requires any project role or non-'consumer'
        global role.
      operationId: FindProjects
      x-api-path-slug: projects-get
      parameters:
      - in: query
        name: userQuery
        description: Filters the projects returned
      - in: query
        name: view
        description: 'Return related resources:  * `full` - Any deployments in the
          project; any tags referred to by tagUris (**not implemented**)'
      responses:
        200:
          description: OK
      tags:
      - Projects
    post:
      summary: Post Projects
      description: Creates a new project. It requires the **project-owner** project
        role, or **administrator** or **project creator** global role.
      operationId: CreateProject
      x-api-path-slug: projects-post
      parameters:
      - in: body
        name: project
        description: Add new project
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Projects
  /projects/{id}:
    delete:
      summary: Delete Projects
      description: Deletes a project. If resources (currently Deployments) exist within
        the project they must first be deleted. In this case, the response will be
        a 409 Conflict with the body listing the first ten offending items. It requires
        **administratpor** global role or **owner** project role. **not implemented**
      operationId: deletes-a-project-if-resources-currently-deployments-exist-within-the-project-they-must-first-be-del
      x-api-path-slug: projectsid-delete
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Projects
    get:
      summary: Get Projects
      description: Returns a project based on its id. It requires any project role
        or non-consumer global role.
      operationId: GetProjectById
      x-api-path-slug: projectsid-get
      parameters:
      - in: path
        name: id
        description: ID of project to fetch
      - in: query
        name: view
        description: 'Return related resources:  * `full` - Any deployments in the
          project; any tags referred to by tagUris (**not implemented**)'
      responses:
        200:
          description: OK
      tags:
      - Projects
    patch:
      summary: Patch Projects
      description: Updates a project. It requires the **administrator** global role
        or the **project owner** role on a project.
      operationId: UpdateProject
      x-api-path-slug: projectsid-patch
      parameters:
      - in: path
        name: id
        description: ID of project to update
      - in: body
        name: project
        description: Update project
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Projects
  /provider-types:
    get:
      summary: Get Prover Types
      description: Returns provider types.
      operationId: FindProviderTypes
      x-api-path-slug: providertypes-get
      responses:
        200:
          description: OK
      tags:
      - Prover
      - Types
  /providers:
    get:
      summary: Get Provers
      description: Returns providers. It requires the **consumer** global role.
      operationId: FindProviders
      x-api-path-slug: providers-get
      parameters:
      - in: query
        name: query
        description: Filters the providers returned
      responses:
        200:
          description: OK
      tags:
      - Provers
    post:
      summary: Post Provers
      description: Creates a new Master provider or Member provider.
      operationId: CreateProvider
      x-api-path-slug: providers-post
      parameters:
      - in: body
        name: provider
        description: Add new provider
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Provers
  /providers/{id}:
    delete:
      summary: Delete Provers
      description: Deletes a master provider or a child provider
      operationId: DeleteProviderById
      x-api-path-slug: providersid-delete
      parameters:
      - in: path
        name: id
        description: ID of provider to delete
      responses:
        200:
          description: OK
      tags:
      - Provers
    get:
      summary: Get Provers
      description: Returns a provider based on its id. It requires the **consumer**
        global role.
      operationId: GetProviderById
      x-api-path-slug: providersid-get
      parameters:
      - in: query
        name: discover
        description: Will return the merged set of regions from AWS and existing regions
          in Onesphere
      - in: path
        name: id
        description: ID of provider to fetch
      - in: query
        name: view
        description: Whether to return related content
      responses:
        200:
          description: OK
      tags:
      - Provers
    patch:
      summary: Patch Provers
      description: Updates a provider.
      operationId: UpdateProvider
      x-api-path-slug: providersid-patch
      parameters:
      - in: body
        name: body
        description: Update provider
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: ID of provider to update
      responses:
        200:
          description: OK
      tags:
      - Provers
  /rates:
    get:
      summary: Get Rates
      description: |-
        Returns rates. It requires the **administrator** global role.

        Optionally this list may be filtered, or the default rates specified with a resourceUri of 'default'.
      operationId: listRates
      x-api-path-slug: rates-get
      parameters:
      - in: query
        name: active
        description: Filter for active or inactive rates
      - in: query
        name: count
        description: Maximum number of response members to return
      - in: query
        name: effectiveDate
        description: The specific effective date to filter by
      - in: query
        name: effectiveForDate
        description: The date for which returned rates need be effective, a special
          filter that allows a search for a rate that would be effective on a date
      - in: query
        name: metricName
        description: The metric name to filter by
      - in: query
        name: resourceUri
        description: Resource(s) to return rates for
      - in: query
        name: start
        description: Index into the response members to allow pagination
      responses:
        200:
          description: OK
      tags:
      - Rates
  /rates/{id}:
    get:
      summary: Get Rates
      description: Retrieve a rate by id. It requires the **administrator** global
        role.
      operationId: getRateById
      x-api-path-slug: ratesid-get
      parameters:
      - in: path
        name: id
        description: Id of the rate to be retrieved
      responses:
        200:
          description: OK
      tags:
      - Rates
  /regions:
    get:
      summary: Get Regions
      description: Returns regions. It requires the **consumer** global role.
      operationId: FindRegions
      x-api-path-slug: regions-get
      parameters:
      - in: query
        name: query
        description: Filters the regions returned
      - in: query
        name: view
        description: Whether to return related content
      responses:
        200:
          description: OK
      tags:
      - Regions
    post:
      summary: Post Regions
      description: Creates a new region.
      operationId: CreateRegion
      x-api-path-slug: regions-post
      parameters:
      - in: body
        name: region
        description: Add new region
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Regions
  /regions/{id}:
    delete:
      summary: Delete Regions
      description: Deletes a region
      operationId: Delete Region
      x-api-path-slug: regionsid-delete
      parameters:
      - in: query
        name: force
        description: Region may be in an odd state
      - in: path
        name: id
        description: ID of region to delete
      responses:
        200:
          description: OK
      tags:
      - Regions
    get:
      summary: Get Regions
      description: Returns a region based on its id. It requires the **consumer**
        global role.
      operationId: GetRegionById
      x-api-path-slug: regionsid-get
      parameters:
      - in: query
        name: discover
        description: will return child providers from aws
      - in: path
        name: id
        description: ID of region to fetch
      - in: query
        name: view
        description: Whether to return related content
      responses:
        200:
          description: OK
      tags:
      - Regions
    patch:
      summary: Patch Regions
      description: Patches a region. PATCH only supports provider type(/rest/provider-types/ncs).
        Allowed fields to PATCH for NCS provider type are (name,location)
      operationId: PatchRegion
      x-api-path-slug: regionsid-patch
      parameters:
      - in: body
        name: body
        description: Patch region
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: ID of region to patch
      responses:
        200:
          description: OK
      tags:
      - Regions
    put:
      summary: Put Regions
      description: Updates a region. **Not implemented**
      operationId: UpdateRegion
      x-api-path-slug: regionsid-put
      parameters:
      - in: path
        name: id
        description: ID of region to update
      - in: body
        name: region
        description: Update region
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Regions
  /regions/{id}/connection:
    delete:
      summary: Delete Regions Connection
      description: ""
      operationId: DeleteRegionConnection
      x-api-path-slug: regionsidconnection-delete
      parameters:
      - in: path
        name: id
        description: ID of region
      responses:
        200:
          description: OK
      tags:
      - Regions
      - Connection
    get:
      summary: Get Regions Connection
      description: Get region connection.
      operationId: GetRegionConnection
      x-api-path-slug: regionsidconnection-get
      parameters:
      - in: path
        name: id
        description: ID of region
      responses:
        200:
          description: OK
      tags:
      - Regions
      - Connection
    post:
      summary: Post Regions Connection
      description: Creates a new region connection
      operationId: CreateRegionConnection
      x-api-path-slug: regionsidconnection-post
      parameters:
      - in: path
        name: id
        description: ID of region
      - in: body
        name: regionConnection
        description: Add new region connection
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Regions
      - Connection
  /regions/{id}/connector-image:
    get:
      summary: Get Regions Connector Image
      description: Generates connector-image url for the region. It requires the **administrator**
        role.
      operationId: getConnectorImage
      x-api-path-slug: regionsidconnectorimage-get
      parameters:
      - in: path
        name: id
        description: ID of region to fetch the connector-image
      responses:
        200:
          description: OK
      tags:
      - Regions
      - Connector
      - Image
  /roles:
    get:
      summary: Get Roles
      description: Returns global roles.
      operationId: ListRoles
      x-api-path-slug: roles-get
      responses:
        200:
          description: OK
      tags:
      - Roles
  /servers:
    get:
      summary: Get Servers
      description: Returns servers.
      operationId: GetServer
      x-api-path-slug: servers-get
      parameters:
      - in: query
        name: applianceUri
        description: Set of servers in this appliance
      - in: query
        name: regionUri
        description: Set of servers in this region
      - in: query
        name: zoneUri
        description: Set of servers in this zone
      responses:
        200:
          description: OK
      tags:
      - Servers
    post:
      summary: Post Servers
      description: Create/Register a server.
      operationId: CreateServer
      x-api-path-slug: servers-post
      parameters:
      - in: body
        name: server
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Servers
  /servers/{id}:
    delete:
      summary: Delete Servers
      description: |-
        Delete a server.
        Note that by default only servers created via the HPE OneSphere API can be
        subsequently deleted. HPE OneSphere managed servers (those that have
        an applianceUri) cannot be deleted via this operation (a '403' will be returned),
        unless the 'force' parameter is supplied and set to 'true'.
      operationId: DeleteServer
      x-api-path-slug: serversid-delete
      parameters:
      - in: query
        name: force
        description: Delete Server even if Delete operation is not allowed on this
          server by default,e
      - in: path
        name: id
        description: ID of the server to delete
      responses:
        200:
          description: OK
      tags:
      - Servers
    get:
      summary: Get Servers
      description: Returns a server based on its ID.
      operationId: GetServerById
      x-api-path-slug: serversid-get
      parameters:
      - in: path
        name: id
        description: ID of the server to retrieve
      responses:
        200:
          description: OK
      tags:
      - Servers
    patch:
      summary: Patch Servers
      description: Update properties of a server.
      operationId: UpdateServer
      x-api-path-slug: serversid-patch
      parameters:
      - in: body
        name: body
        description: List of server updates
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: ID of server to update
      responses:
        200:
          description: OK
      tags:
      - Servers
  /service-types:
    get:
      summary: Get Service Types
      description: Returns all service types. It requires the **consumer** global
        role.
      operationId: FindServiceTypes
      x-api-path-slug: servicetypes-get
      responses:
        200:
          description: OK
      tags:
      - Service
      - Types
  /service-types/{id}:
    get:
      summary: Get Service Types
      description: Return a service type based on its id. It requires the **consumer**
        global role.
      operationId: GetServiceTypeById
      x-api-path-slug: servicetypesid-get
      parameters:
      - in: path
        name: id
        description: ID of service type to fetch
      responses:
        200:
          description: OK
      tags:
      - Service
      - Types
  /services:
    get:
      summary: Get Services
      description: Returns services. It requires any project role or non-'consumer'
        global role.
      operationId: FindServices
      x-api-path-slug: services-get
      parameters:
      - in: query
        name: query
        description: Filters the services returned
      - in: query
        name: userQuery
        description: Filters the services returned
      - in: query
        name: view
        description: 'Return related resources:  * `full` - Include all the details
          of the services'
      responses:
        200:
          description: OK
      tags:
      - Services
  /services/{id}:
    get:
      summary: Get Services
      description: Returns a service based on its id. It requires any project role
        or non-'consumer' global role.
      operationId: GetServiceById
      x-api-path-slug: servicesid-get
      parameters:
      - in: path
        name: id
        description: ID of service to fetch
      - in: query
        name: view
        description: 'Return related resources:  * `full` - Include all the details
          of the services  * `deployment` - Return the zones to which the service
          can be deployed'
      responses:
        200:
          description: OK
      tags:
      - Services
  /session:
    delete:
      summary: Delete Session
      description: Deletes cached data and tokens for the current session.
      operationId: DeleteSession
      x-api-path-slug: session-delete
      responses:
        200:
          description: OK
      tags:
      - Session
    get:
      summary: Get Session
      description: Gets information for the current user.
      operationId: ReadSession
      x-api-path-slug: session-get
      parameters:
      - in: query
        name: view
        description: 'Return related resources:  * `full` - Include the related `user`'
      responses:
        200:
          description: OK
      tags:
      - Session
    post:
      summary: Post Session
      description: |-
        Authenticates a local user and generates an authorization token. This
        token should be used in subsequent HTTP requests as part of
        the "Authorization" header. For example:

        `Authorization: "Bearer <token>"`
      operationId: CreateSession
      x-api-path-slug: session-post
      parameters:
      - in: body
        name: credentials
        description: UserName and Password
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Session
  /session/idp:
    get:
      summary: Get Session P
      description: |-
        **Not implemented**

        Gets the Identity Provider login URL for a userName.
      operationId: ReadSessionIdp
      x-api-path-slug: sessionidp-get
      parameters:
      - in: query
        name: userName
        description: User Name of the User for which login context is needed
      responses:
        200:
          description: OK
      tags:
      - Session
      - P
  /session/sso:
    get:
      summary: Get Session Sso
      description: Get the redirect URL for a configured SSO provider
      operationId: GetSSOLogin
      x-api-path-slug: sessionsso-get
      responses:
        200:
          description: OK
      tags:
      - Session
      - Sso
    post:
      summary: Post Session Sso
      description: Callback for SSO login
      operationId: callback-for-sso-login
      x-api-path-slug: sessionsso-post
      parameters:
      - in: query
        name: token
        description: The unscoped token
      responses:
        200:
          description: OK
      tags:
      - Session
      - Sso
  /status:
    get:
      summary: Get Status
      description: Checks the service is running. It does not require authorization.
      operationId: ReadStatus
      x-api-path-slug: status-get
      responses:
        200:
          description: OK
      tags:
      - Status
  /tag-keys:
    get:
      summary: Get Tag Keys
      description: Lists tag keys.
      operationId: ListTagKeys
      x-api-path-slug: tagkeys-get
      parameters:
      - in: query
        name: view
        description: 'Return related resources:  * `full` - include each tag-keys
          related `tags`'
      responses:
        200:
          description: OK
      tags:
      - Tag
      - Keys
    post:
      summary: Post Tag Keys
      description: Create a tag key. It requires the **analyst** global role.
      operationId: CreateTagKey
      x-api-path-slug: tagkeys-post
      parameters:
      - in: body
        name: name
        description: New tag key
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Tag
      - Keys
  /tag-keys/{id}:
    delete:
      summary: Delete Tag Keys
      description: Delete a tag key and associated tags. It requires the **analyst**
        global role.
      operationId: DeleteTagKey
      x-api-path-slug: tagkeysid-delete
      parameters:
      - in: path
        name: id
        description: ID of tag key to delete
      responses:
        200:
          description: OK
      tags:
      - Tag
      - Keys
    get:
      summary: Get Tag Keys
      description: Returns a tag key based on its id.
      operationId: GetTagKeyById
      x-api-path-slug: tagkeysid-get
      parameters:
      - in: path
        name: id
        description: ID of tag key to fetch
      - in: query
        name: view
        description: 'Return related resources:  * `full` - Include the tag-keys related
          `tags`'
      responses:
        200:
          description: OK
      tags:
      - Tag
      - Keys
  /tags:
    get:
      summary: Get Tags
      description: Lists tags.
      operationId: ListTags
      x-api-path-slug: tags-get
      parameters:
      - in: query
        name: view
        description: 'Return related resources:  * `full` - include each tags related
          `tag-key`'
      responses:
        200:
          description: OK
      tags:
      - Tags
    post:
      summary: Post Tags
      description: Create a tag. It requires the **analyst** global role.
      operationId: CreateTag
      x-api-path-slug: tags-post
      parameters:
      - in: body
        name: tag
        description: New tag
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Tags
  /tags/{id}:
    delete:
      summary: Delete Tags
      description: Delete a tag. It requires the **analyst** global role.
      operationId: DeleteTag
      x-api-path-slug: tagsid-delete
      parameters:
      - in: path
        name: id
        description: ID of tag to delete
      responses:
        200:
          description: OK
      tags:
      - Tags
    get:
      summary: Get Tags
      description: Returns a tag based on its id. It requires the **consumer** global
        role.
      operationId: GetTagById
      x-api-path-slug: tagsid-get
      parameters:
      - in: path
        name: id
        description: ID of tag to fetch
      - in: query
        name: view
        description: 'Return related resources:  * `full` - Include the tags related
          `tag-key`'
      responses:
        200:
          description: OK
      tags:
      - Tags
  /users:
    get:
      summary: Get Users
      description: Returns users.
      operationId: ListUsers
      x-api-path-slug: users-get
      parameters:
      - in: query
        name: userQuery
        description: Filters the users returned
      responses:
        200:
          description: OK
      tags:
      - Users
    post:
      summary: Post Users
      description: |-
        Create a user. It requires the **administrator** or **project creator** global role.

        The password should be a minimum of 8 characters long.
      operationId: CreateUser
      x-api-path-slug: users-post
      parameters:
      - in: body
        name: user
        description: New user
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Users
  /users/{id}:
    delete:
      summary: Delete Users
      description: Delete a user. It requires the **administrator** or **project creator**
        global role.
      operationId: DeleteUser
      x-api-path-slug: usersid-delete
      parameters:
      - in: path
        name: id
        description: Delete user
      responses:
        200:
          description: OK
      tags:
      - Users
    get:
      summary: Get Users
      description: Returns a user based on its id. It requires the **administrator**
        or **project creator** global role, or matching user id.
      operationId: GetUserById
      x-api-path-slug: usersid-get
      parameters:
      - in: path
        name: id
        description: ID of user to fetch
      responses:
        200:
          description: OK
      tags:
      - Users
    patch:
      summary: Patch Users
      description: |-
        Update a user. It requires the **administrator** or **project creator** global role or matching user ID.

        If the password is updated it must be a minimum of 8 characters long.
      operationId: UpdateUser
      x-api-path-slug: usersid-patch
      parameters:
      - in: path
        name: id
        description: ID of user to update
      - in: body
        name: user
        description: Update user
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Users
  /virtual-machine-profiles:
    get:
      summary: Get Virtual Machine Profiles
      description: Returns all virtual machine profiles. It requires any project role
        or non-'consumer' global role.
      operationId: FindVirtualMachineProfiles
      x-api-path-slug: virtualmachineprofiles-get
      parameters:
      - in: query
        name: serviceUri
        description: service to filter virtual machine profiles by
      - in: query
        name: zoneUri
        description: Zone to filter virtual machine profiles by
      responses:
        200:
          description: OK
      tags:
      - Virtual
      - Machine
      - Profiles
  /virtual-machine-profiles/{id}:
    get:
      summary: Get Virtual Machine Profiles
      description: Returns a virtual machine profile based on its id. It equires any
        project role or non-'consumer' global role.
      operationId: GetVirtualMachineProfileById
      x-api-path-slug: virtualmachineprofilesid-get
      parameters:
      - in: path
        name: id
        description: ID of virtual machine profile to fetch
      responses:
        200:
          description: OK
      tags:
      - Virtual
      - Machine
      - Profiles
  /volumes:
    get:
      summary: Get Volumes
      description: Returns volumes. It requires any project role or non-'consumer'
        global role.
      operationId: FindVolumes
      x-api-path-slug: volumes-get
      parameters:
      - in: query
        name: query
        description: URI query string to prune volumes by
      - in: query
        name: view
        description: 'Return related resources:  * `full` - include zone, volume details'
      responses:
        200:
          description: OK
      tags:
      - Volumes
    post:
      summary: Post Volumes
      description: Creates a new volume. It requires any project role or the **administrator**
        or **project creator** global role.
      operationId: CreateVolume
      x-api-path-slug: volumes-post
      parameters:
      - in: body
        name: volume
        description: Add new volume
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Volumes
  /volumes/{id}:
    delete:
      summary: Delete Volumes
      description: Delete a volume. It requires any project role or the **administrator**
        or **project creator** global role.
      operationId: DeleteVolume
      x-api-path-slug: volumesid-delete
      parameters:
      - in: path
        name: id
        description: ID of volume to delete
      responses:
        200:
          description: OK
      tags:
      - Volumes
    get:
      summary: Get Volumes
      description: Returns a volume based on its id. It requires any project role
        or non-'consumer' global role.
      operationId: GetVolumeById
      x-api-path-slug: volumesid-get
      parameters:
      - in: path
        name: id
        description: ID of volume to fetch
      responses:
        200:
          description: OK
      tags:
      - Volumes
    patch:
      summary: Patch Volumes
      description: Updates a volume. **Requires any project role or 'administrator'
        or 'project creator' global role**. Allowed fields for PATCH of volumes are
        name(add,replace), size(add,replace)
      operationId: UpdateVolume
      x-api-path-slug: volumesid-patch
      parameters:
      - in: path
        name: id
        description: ID of volume to update
      - in: body
        name: volume
        description: Update volume
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Volumes
  /zone-types:
    get:
      summary: Get Zone Types
      description: Returns all zone types.
      operationId: FindZoneTypes
      x-api-path-slug: zonetypes-get
      responses:
        200:
          description: OK
      tags:
      - Zone
      - Types
  /zone-types/{id}/resource-profiles:
    get:
      summary: Get Zone Types Resource Profiles
      description: Returns all available resourceProfile for **vcenter zone type**.
        It requires the **administrator** role.
      operationId: FindResourceProfileName
      x-api-path-slug: zonetypesidresourceprofiles-get
      parameters:
      - in: path
        name: id
        description: ID of zone-type to fetch
      responses:
        200:
          description: OK
      tags:
      - Zone
      - Types
      - Resource
      - Profiles
  /zones:
    get:
      summary: Get Zones
      description: Returns zones.
      operationId: FindZones
      x-api-path-slug: zones-get
      parameters:
      - in: query
        name: applianceUri
        description: The appliance URI to prune zones by
      - in: query
        name: providerUri
        description: The provider URI to prune zones by
      - in: query
        name: query
        description: Filters the zones returned
      - in: query
        name: regionUri
        description: The region URI to prune zones by
      - in: query
        name: view
        description: 'Return related resources:  * `full` - Include all the details
          of the zones'
      responses:
        200:
          description: OK
      tags:
      - Zones
    post:
      summary: Post Zones
      description: Creates a new zone
      operationId: CreateZone
      x-api-path-slug: zones-post
      parameters:
      - in: body
        name: zone
        description: Add new zone
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Zones
  /zones/{id}:
    delete:
      summary: Delete Zones
      description: Deletes a zone
      operationId: DeleteZone
      x-api-path-slug: zonesid-delete
      parameters:
      - in: query
        name: force
        description: Zones may be in an odd state
      - in: path
        name: id
        description: ID of zone to delete
      responses:
        200:
          description: OK
      tags:
      - Zones
    get:
      summary: Get Zones
      description: Returns a zone based on its id.
      operationId: GetZoneById
      x-api-path-slug: zonesid-get
      parameters:
      - in: path
        name: id
        description: ID of zone to fetch
      - in: query
        name: view
        description: Whether to return related content
      responses:
        200:
          description: OK
      tags:
      - Zones
    patch:
      summary: Patch Zones
      description: Updates a zone
      operationId: UpdateZone
      x-api-path-slug: zonesid-patch
      parameters:
      - in: path
        name: id
        description: ID of zone to update
      - in: body
        name: zone
        description: Update zone
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Zones
  /zones/{id}/actions:
    post:
      summary: Post Zones Actions
      description: Peforms an action to the zone. It requires the **administrator**
        role.
      operationId: ActOnZone
      x-api-path-slug: zonesidactions-post
      parameters:
      - in: body
        name: action
        description: Action to perform
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: ID of zone to act on
      responses:
        200:
          description: OK
      tags:
      - Zones
      - Actions
  /zones/{id}/appliance-image:
    get:
      summary: Get Zones Appliance Image
      description: Generates appliance-image url for the zone
      operationId: appliance-image
      x-api-path-slug: zonesidapplianceimage-get
      parameters:
      - in: path
        name: id
        description: ID of zone to fetch the appliance-image
      responses:
        200:
          description: OK
      tags:
      - Zones
      - Appliance
      - Image
  /zones/{id}/connections:
    get:
      summary: Get Zones Connections
      description: Gets the list of connection for the zone. It requires the **administrator**
        role.
      operationId: zoneConnectionInstances
      x-api-path-slug: zonesidconnections-get
      parameters:
      - in: path
        name: id
        description: ID of zone to fetch the list of connection for the zone
      - in: query
        name: uuid
        description: Type to filter connection by
      responses:
        200:
          description: OK
      tags:
      - Zones
      - Connections
    post:
      summary: Post Zones Connections
      description: Peforms an action to the zone. It requires the **administrator**
        role.
      operationId: RegisterZoneConnection
      x-api-path-slug: zonesidconnections-post
      parameters:
      - in: path
        name: id
        description: ID of zone to act on
      - in: body
        name: zoneConnection
        description: Create a new connection instance for the zone
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Zones
      - Connections
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