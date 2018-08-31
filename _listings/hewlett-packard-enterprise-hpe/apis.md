---
name: Hewlett Packard Enterprise (HPE)
x-slug: hewlett-packard-enterprise-hpe
description: We help customers use technology to slash the time it takes to turn ideas
  into value. In turn, they transform industries, markets and lives. Some of our customers
  run traditional IT environments. Most are transitioning to a secure, cloud-enabled,
  mobile-friendly infrastructure. Many rely on a combination of both. Wherever they
  are in that journey, we provide the technology and solutions to help them succeed.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/HPE-logo.png
x-kinRank: "8"
x-alexaRank: "0"
tags: Hewlett Packard Enterprise (HPE)
created: "2018-08-30"
modified: "2018-08-30"
url: https://raw.githubusercontent.com/streamdata-gallery-organizations/hewlett-packard-enterprise-hpe/master/_listings/hewlett-packard-enterprise-hpe/apis.md
specificationVersion: "0.14"
apis:
- name: HPE OneSphere API - Get About Versions
  x-api-slug: aboutversions-get
  description: Get supported versions
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/HPE-logo.png
  humanURL: http://HPE.com
  baseURL: https://deic02-hpe.hpeonesphere.com//rest
  tags: Enterprise, Cloud, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/hewlett-packard-enterprise-hpe/master/_listings/hewlett-packard-enterprise-hpe/aboutversions-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/hewlett-packard-enterprise-hpe/master/_listings/hewlett-packard-enterprise-hpe/aboutversions-get-openapi.md
- name: HPE OneSphere API - Get Account
  x-api-slug: account-get
  description: Returns the global account information. **Not implemented**
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/HPE-logo.png
  humanURL: http://HPE.com
  baseURL: https://deic02-hpe.hpeonesphere.com//rest
  tags: Enterprise, Cloud, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/hewlett-packard-enterprise-hpe/master/_listings/hewlett-packard-enterprise-hpe/account-get-openapi.md
- name: HPE OneSphere API - Get Appliances
  x-api-slug: appliances-get
  description: Returns appliances.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/HPE-logo.png
  humanURL: http://HPE.com
  baseURL: https://deic02-hpe.hpeonesphere.com//rest
  tags: Enterprise, Cloud, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/hewlett-packard-enterprise-hpe/master/_listings/hewlett-packard-enterprise-hpe/appliances-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/hewlett-packard-enterprise-hpe/master/_listings/hewlett-packard-enterprise-hpe/appliances-get-openapi.md
- name: HPE OneSphere API - Post Appliances
  x-api-slug: appliances-post
  description: Create an appliance.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/HPE-logo.png
  humanURL: http://HPE.com
  baseURL: https://deic02-hpe.hpeonesphere.com//rest
  tags: Enterprise, Cloud, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/hewlett-packard-enterprise-hpe/master/_listings/hewlett-packard-enterprise-hpe/appliances-post-openapi.md
- name: HPE OneSphere API - Delete Appliances
  x-api-slug: appliancesid-delete
  description: |-
    Delete an appliance.
    This removes the appliance registration and tears down the secure
    comms link to the on-premise appliance.
    If zones exist on this appliance, an '409' error will be returned.
    The zones on this appliance must be removed before the appliance
    delete request can be accepted.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/HPE-logo.png
  humanURL: http://HPE.com
  baseURL: https://deic02-hpe.hpeonesphere.com//rest
  tags: Enterprise, Cloud, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/hewlett-packard-enterprise-hpe/master/_listings/hewlett-packard-enterprise-hpe/appliancesid-delete-openapi.md
- name: HPE OneSphere API - Get Appliances
  x-api-slug: appliancesid-get
  description: Returns an appliance based on its ID.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/HPE-logo.png
  humanURL: http://HPE.com
  baseURL: https://deic02-hpe.hpeonesphere.com//rest
  tags: Enterprise, Cloud, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/hewlett-packard-enterprise-hpe/master/_listings/hewlett-packard-enterprise-hpe/appliancesid-get-openapi.md
- name: HPE OneSphere API - Patch Appliances
  x-api-slug: appliancesid-patch
  description: Update properties of an appliance.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/HPE-logo.png
  humanURL: http://HPE.com
  baseURL: https://deic02-hpe.hpeonesphere.com//rest
  tags: Enterprise, Cloud, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/hewlett-packard-enterprise-hpe/master/_listings/hewlett-packard-enterprise-hpe/appliancesid-patch-openapi.md
- name: HPE OneSphere API - Get Billing Accounts
  x-api-slug: billingaccounts-get
  description: Returns billing accounts. It requires the **administrator** or **project
    creator** global role.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/HPE-logo.png
  humanURL: http://HPE.com
  baseURL: https://deic02-hpe.hpeonesphere.com//rest
  tags: Enterprise, Cloud, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/hewlett-packard-enterprise-hpe/master/_listings/hewlett-packard-enterprise-hpe/billingaccounts-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/hewlett-packard-enterprise-hpe/master/_listings/hewlett-packard-enterprise-hpe/billingaccounts-get-openapi.md
- name: HPE OneSphere API - Post Billing Accounts
  x-api-slug: billingaccounts-post
  description: Creates a new billing account. It requires the **administrator** role.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/HPE-logo.png
  humanURL: http://HPE.com
  baseURL: https://deic02-hpe.hpeonesphere.com//rest
  tags: Enterprise, Cloud, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/hewlett-packard-enterprise-hpe/master/_listings/hewlett-packard-enterprise-hpe/billingaccounts-post-openapi.md
- name: HPE OneSphere API - Delete Billing Accounts
  x-api-slug: billingaccountsid-delete
  description: Deletes a billing account. It requires the **administrator** role.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/HPE-logo.png
  humanURL: http://HPE.com
  baseURL: https://deic02-hpe.hpeonesphere.com//rest
  tags: Enterprise, Cloud, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/hewlett-packard-enterprise-hpe/master/_listings/hewlett-packard-enterprise-hpe/billingaccountsid-delete-openapi.md
- name: HPE OneSphere API - Get Billing Accounts
  x-api-slug: billingaccountsid-get
  description: Returns a billing account based on its id. It requires the **administrator**
    or **project creator** global role. Credentials are not included.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/HPE-logo.png
  humanURL: http://HPE.com
  baseURL: https://deic02-hpe.hpeonesphere.com//rest
  tags: Enterprise, Cloud, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/hewlett-packard-enterprise-hpe/master/_listings/hewlett-packard-enterprise-hpe/billingaccountsid-get-openapi.md
- name: HPE OneSphere API - Patch Billing Accounts
  x-api-slug: billingaccountsid-patch
  description: Updates a billing account. It requires the **administrator** role.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/HPE-logo.png
  humanURL: http://HPE.com
  baseURL: https://deic02-hpe.hpeonesphere.com//rest
  tags: Enterprise, Cloud, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/hewlett-packard-enterprise-hpe/master/_listings/hewlett-packard-enterprise-hpe/billingaccountsid-patch-openapi.md
- name: HPE OneSphere API - Get Catalog Types
  x-api-slug: catalogtypes-get
  description: Returns catalog types.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/HPE-logo.png
  humanURL: http://HPE.com
  baseURL: https://deic02-hpe.hpeonesphere.com//rest
  tags: Enterprise, Cloud, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/hewlett-packard-enterprise-hpe/master/_listings/hewlett-packard-enterprise-hpe/catalogtypes-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/hewlett-packard-enterprise-hpe/master/_listings/hewlett-packard-enterprise-hpe/catalogtypes-get-openapi.md
- name: HPE OneSphere API - Get Catalogs
  x-api-slug: catalogs-get
  description: Returns catalogs. It requires the **consumer** global role.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/HPE-logo.png
  humanURL: http://HPE.com
  baseURL: https://deic02-hpe.hpeonesphere.com//rest
  tags: Enterprise, Cloud, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/hewlett-packard-enterprise-hpe/master/_listings/hewlett-packard-enterprise-hpe/catalogs-get-openapi.md
- name: HPE OneSphere API - Post Catalogs
  x-api-slug: catalogs-post
  description: Creates a new catalog.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/HPE-logo.png
  humanURL: http://HPE.com
  baseURL: https://deic02-hpe.hpeonesphere.com//rest
  tags: Enterprise, Cloud, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/hewlett-packard-enterprise-hpe/master/_listings/hewlett-packard-enterprise-hpe/catalogs-post-openapi.md
- name: HPE OneSphere API - Delete Catalogs
  x-api-slug: catalogsid-delete
  description: Delete a catalog and associated resources. **Not implemented**
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/HPE-logo.png
  humanURL: http://HPE.com
  baseURL: https://deic02-hpe.hpeonesphere.com//rest
  tags: Enterprise, Cloud, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/hewlett-packard-enterprise-hpe/master/_listings/hewlett-packard-enterprise-hpe/catalogsid-delete-openapi.md
- name: HPE OneSphere API - Get Catalogs
  x-api-slug: catalogsid-get
  description: Returns a catalog based on its id. It requires the **consumer** global
    role.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/HPE-logo.png
  humanURL: http://HPE.com
  baseURL: https://deic02-hpe.hpeonesphere.com//rest
  tags: Enterprise, Cloud, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/hewlett-packard-enterprise-hpe/master/_listings/hewlett-packard-enterprise-hpe/catalogsid-get-openapi.md
- name: HPE OneSphere API - Patch Catalogs
  x-api-slug: catalogsid-patch
  description: Patches a catalog. Allowed fields for PATCH of catalogs are name(add,replace),
    password(add), accessKey(add), secretKey(add), state(add,replace)
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/HPE-logo.png
  humanURL: http://HPE.com
  baseURL: https://deic02-hpe.hpeonesphere.com//rest
  tags: Enterprise, Cloud, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/hewlett-packard-enterprise-hpe/master/_listings/hewlett-packard-enterprise-hpe/catalogsid-patch-openapi.md
- name: HPE OneSphere API - Get Connect App
  x-api-slug: connectapp-get
  description: Generates connect app s3 url
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/HPE-logo.png
  humanURL: http://HPE.com
  baseURL: https://deic02-hpe.hpeonesphere.com//rest
  tags: Enterprise, Cloud, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/hewlett-packard-enterprise-hpe/master/_listings/hewlett-packard-enterprise-hpe/connectapp-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/hewlett-packard-enterprise-hpe/master/_listings/hewlett-packard-enterprise-hpe/connectapp-get-openapi.md
- name: HPE OneSphere API - Get Deployments
  x-api-slug: deployments-get
  description: Returns deployments. It requires any project role or non-'consumer'
    global role.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/HPE-logo.png
  humanURL: http://HPE.com
  baseURL: https://deic02-hpe.hpeonesphere.com//rest
  tags: Enterprise, Cloud, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/hewlett-packard-enterprise-hpe/master/_listings/hewlett-packard-enterprise-hpe/deployments-get-openapi.md
- name: HPE OneSphere API - Post Deployments
  x-api-slug: deployments-post
  description: Creates a new deployment. It requires any project role, or the **administrator**
    or **project creator** global role.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/HPE-logo.png
  humanURL: http://HPE.com
  baseURL: https://deic02-hpe.hpeonesphere.com//rest
  tags: Enterprise, Cloud, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/hewlett-packard-enterprise-hpe/master/_listings/hewlett-packard-enterprise-hpe/deployments-post-openapi.md
- name: HPE OneSphere API - Delete Deployments
  x-api-slug: deploymentsid-delete
  description: Delete a deployment and associated resources. It requires any project
    role, or the **administrator** or **project creator** global role.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/HPE-logo.png
  humanURL: http://HPE.com
  baseURL: https://deic02-hpe.hpeonesphere.com//rest
  tags: Enterprise, Cloud, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/hewlett-packard-enterprise-hpe/master/_listings/hewlett-packard-enterprise-hpe/deploymentsid-delete-openapi.md
- name: HPE OneSphere API - Get Deployments
  x-api-slug: deploymentsid-get
  description: Returns a deployment based on its id. It requires any project role
    or non-'consumer' global role.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/HPE-logo.png
  humanURL: http://HPE.com
  baseURL: https://deic02-hpe.hpeonesphere.com//rest
  tags: Enterprise, Cloud, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/hewlett-packard-enterprise-hpe/master/_listings/hewlett-packard-enterprise-hpe/deploymentsid-get-openapi.md
- name: HPE OneSphere API - Patch Deployments
  x-api-slug: deploymentsid-patch
  description: Updates a deployment. **Requires any project role, or 'administrator'
    or 'project creator' global role**. Allowed fields for PATCH of deployments are
    name(add,replace), volumes(add), k8snumWorkers(add), userData(add), serviceInput(add),
    version(add).
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/HPE-logo.png
  humanURL: http://HPE.com
  baseURL: https://deic02-hpe.hpeonesphere.com//rest
  tags: Enterprise, Cloud, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/hewlett-packard-enterprise-hpe/master/_listings/hewlett-packard-enterprise-hpe/deploymentsid-patch-openapi.md
- name: HPE OneSphere API - Post Deployments Actions
  x-api-slug: deploymentsidactions-post
  description: Peforms an action to change the state of a deployment. It requires
    any project role, or the **administrator** or **project creator** global role.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/HPE-logo.png
  humanURL: http://HPE.com
  baseURL: https://deic02-hpe.hpeonesphere.com//rest
  tags: Enterprise, Cloud, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/hewlett-packard-enterprise-hpe/master/_listings/hewlett-packard-enterprise-hpe/deploymentsidactions-post-openapi.md
- name: HPE OneSphere API - Post Deployments Console
  x-api-slug: deploymentsidconsole-post
  description: Returns a deployment console URL for deployment
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/HPE-logo.png
  humanURL: http://HPE.com
  baseURL: https://deic02-hpe.hpeonesphere.com//rest
  tags: Enterprise, Cloud, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/hewlett-packard-enterprise-hpe/master/_listings/hewlett-packard-enterprise-hpe/deploymentsidconsole-post-openapi.md
- name: HPE OneSphere API - Get Deployments Kubeconfig
  x-api-slug: deploymentsidkubeconfig-get
  description: Returns the kubeconfig. Applicable only to deployments of Kubernetes
    cluster. **Requires 'consumer' role on workspace**
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/HPE-logo.png
  humanURL: http://HPE.com
  baseURL: https://deic02-hpe.hpeonesphere.com//rest
  tags: Enterprise, Cloud, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/hewlett-packard-enterprise-hpe/master/_listings/hewlett-packard-enterprise-hpe/deploymentsidkubeconfig-get-openapi.md
- name: HPE OneSphere API - Get Events
  x-api-slug: events-get
  description: Returns events based on the supplied criteria. **Not implemented**
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/HPE-logo.png
  humanURL: http://HPE.com
  baseURL: https://deic02-hpe.hpeonesphere.com//rest
  tags: Enterprise, Cloud, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/hewlett-packard-enterprise-hpe/master/_listings/hewlett-packard-enterprise-hpe/events-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/hewlett-packard-enterprise-hpe/master/_listings/hewlett-packard-enterprise-hpe/events-get-openapi.md
- name: HPE OneSphere API - Get Keypairs
  x-api-slug: keypairs-get
  description: Get keypairs (per region, per user). Currently a projectUri is required
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/HPE-logo.png
  humanURL: http://HPE.com
  baseURL: https://deic02-hpe.hpeonesphere.com//rest
  tags: Enterprise, Cloud, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/hewlett-packard-enterprise-hpe/master/_listings/hewlett-packard-enterprise-hpe/keypairs-get-openapi.md
- name: HPE OneSphere API - Get Membership Roles
  x-api-slug: membershiproles-get
  description: Returns membership (project-specific) roles.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/HPE-logo.png
  humanURL: http://HPE.com
  baseURL: https://deic02-hpe.hpeonesphere.com//rest
  tags: Enterprise, Cloud, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/hewlett-packard-enterprise-hpe/master/_listings/hewlett-packard-enterprise-hpe/membershiproles-get-openapi.md
- name: HPE OneSphere API - Delete Memberships
  x-api-slug: memberships-delete
  description: Delete a membership. It requires the **administrator** or **project
    creator** global role or the **project owner** role on the project.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/HPE-logo.png
  humanURL: http://HPE.com
  baseURL: https://deic02-hpe.hpeonesphere.com//rest
  tags: Enterprise, Cloud, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/hewlett-packard-enterprise-hpe/master/_listings/hewlett-packard-enterprise-hpe/memberships-delete-openapi.md
- name: HPE OneSphere API - Get Memberships
  x-api-slug: memberships-get
  description: |-
    Returns memberships. Supports filtering by projectUri, userUri, userGroupUri, roleUri (but only
    individual values, not multiple) in 'query'.

    If projectURI and userUri/userGroupUri are given a different
    backend path will be used that should be authorized to a project owner even if they wouldn't ordinarily
    be able to see other users' roles.

    It requires the **administrator** or **project creator** global role or the **project owner** role on the project.
    **project owner** requires **projectUri** to be supplied.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/HPE-logo.png
  humanURL: http://HPE.com
  baseURL: https://deic02-hpe.hpeonesphere.com//rest
  tags: Enterprise, Cloud, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/hewlett-packard-enterprise-hpe/master/_listings/hewlett-packard-enterprise-hpe/memberships-get-openapi.md
- name: HPE OneSphere API - Post Memberships
  x-api-slug: memberships-post
  description: Creates a new membership. It requires the **administrator** or **project
    creator** global role or **project owner** role on the project.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/HPE-logo.png
  humanURL: http://HPE.com
  baseURL: https://deic02-hpe.hpeonesphere.com//rest
  tags: Enterprise, Cloud, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/hewlett-packard-enterprise-hpe/master/_listings/hewlett-packard-enterprise-hpe/memberships-post-openapi.md
- name: HPE OneSphere API - Get Metrics
  x-api-slug: metrics-get
  description: |-
    Returns all metrics based on the supplied criteria. It requires the **analyst** role.
    It requires one and only one of resourceUri or category to be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/HPE-logo.png
  humanURL: http://HPE.com
  baseURL: https://deic02-hpe.hpeonesphere.com//rest
  tags: Enterprise, Cloud, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/hewlett-packard-enterprise-hpe/master/_listings/hewlett-packard-enterprise-hpe/metrics-get-openapi.md
- name: HPE OneSphere API - Get Networks
  x-api-slug: networks-get
  description: Returns networks. It requires any project role or non-'consumer' global
    role.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/HPE-logo.png
  humanURL: http://HPE.com
  baseURL: https://deic02-hpe.hpeonesphere.com//rest
  tags: Enterprise, Cloud, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/hewlett-packard-enterprise-hpe/master/_listings/hewlett-packard-enterprise-hpe/networks-get-openapi.md
- name: HPE OneSphere API - Get Networks
  x-api-slug: networksid-get
  description: Returns a network based on its id. It requires any project role or
    non-'consumer' global role.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/HPE-logo.png
  humanURL: http://HPE.com
  baseURL: https://deic02-hpe.hpeonesphere.com//rest
  tags: Enterprise, Cloud, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/hewlett-packard-enterprise-hpe/master/_listings/hewlett-packard-enterprise-hpe/networksid-get-openapi.md
- name: HPE OneSphere API - Patch Networks
  x-api-slug: networksid-patch
  description: Updates a network. It requires the **administrator** global role.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/HPE-logo.png
  humanURL: http://HPE.com
  baseURL: https://deic02-hpe.hpeonesphere.com//rest
  tags: Enterprise, Cloud, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/hewlett-packard-enterprise-hpe/master/_listings/hewlett-packard-enterprise-hpe/networksid-patch-openapi.md
- name: HPE OneSphere API - Get Onboarding Azure Properties
  x-api-slug: onboardingazureproperties-get
  description: Returns a properties object needed to build the Azure login url
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/HPE-logo.png
  humanURL: http://HPE.com
  baseURL: https://deic02-hpe.hpeonesphere.com//rest
  tags: Enterprise, Cloud, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/hewlett-packard-enterprise-hpe/master/_listings/hewlett-packard-enterprise-hpe/onboardingazureproperties-get-openapi.md
- name: HPE OneSphere API - Get Onboarding Azure Prover Info
  x-api-slug: onboardingazureproviderinfo-get
  description: Returns the provider information required to add an Azure provider
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/HPE-logo.png
  humanURL: http://HPE.com
  baseURL: https://deic02-hpe.hpeonesphere.com//rest
  tags: Enterprise, Cloud, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/hewlett-packard-enterprise-hpe/master/_listings/hewlett-packard-enterprise-hpe/onboardingazureproviderinfo-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/hewlett-packard-enterprise-hpe/master/_listings/hewlett-packard-enterprise-hpe/onboardingazureproviderinfo-get-openapi.md
- name: HPE OneSphere API - Get Onboarding Azure Subscriptions
  x-api-slug: onboardingazuresubscriptions-get
  description: Returns a list of Azure subscriptions and their display names
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/HPE-logo.png
  humanURL: http://HPE.com
  baseURL: https://deic02-hpe.hpeonesphere.com//rest
  tags: Enterprise, Cloud, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/hewlett-packard-enterprise-hpe/master/_listings/hewlett-packard-enterprise-hpe/onboardingazuresubscriptions-get-openapi.md
- name: HPE OneSphere API - Patch Onboarding Azure Subscriptions Subscriptionid
  x-api-slug: onboardingazuresubscriptionssubscriptionid-patch
  description: Updates a subscription
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/HPE-logo.png
  humanURL: http://HPE.com
  baseURL: https://deic02-hpe.hpeonesphere.com//rest
  tags: Enterprise, Cloud, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/hewlett-packard-enterprise-hpe/master/_listings/hewlett-packard-enterprise-hpe/onboardingazuresubscriptionssubscriptionid-patch-openapi.md
- name: HPE OneSphere API - Post Password Reset
  x-api-slug: passwordreset-post
  description: Request a single-use password reset token.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/HPE-logo.png
  humanURL: http://HPE.com
  baseURL: https://deic02-hpe.hpeonesphere.com//rest
  tags: Enterprise, Cloud, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/hewlett-packard-enterprise-hpe/master/_listings/hewlett-packard-enterprise-hpe/passwordreset-post-openapi.md
- name: HPE OneSphere API - Post Password Reset Change
  x-api-slug: passwordresetchange-post
  description: Process a password reset.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/HPE-logo.png
  humanURL: http://HPE.com
  baseURL: https://deic02-hpe.hpeonesphere.com//rest
  tags: Enterprise, Cloud, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/hewlett-packard-enterprise-hpe/master/_listings/hewlett-packard-enterprise-hpe/passwordresetchange-post-openapi.md
- name: HPE OneSphere API - Get Projects
  x-api-slug: projects-get
  description: Returns projects. It requires any project role or non-'consumer' global
    role.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/HPE-logo.png
  humanURL: http://HPE.com
  baseURL: https://deic02-hpe.hpeonesphere.com//rest
  tags: Enterprise, Cloud, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/hewlett-packard-enterprise-hpe/master/_listings/hewlett-packard-enterprise-hpe/projects-get-openapi.md
- name: HPE OneSphere API - Post Projects
  x-api-slug: projects-post
  description: Creates a new project. It requires the **project-owner** project role,
    or **administrator** or **project creator** global role.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/HPE-logo.png
  humanURL: http://HPE.com
  baseURL: https://deic02-hpe.hpeonesphere.com//rest
  tags: Enterprise, Cloud, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/hewlett-packard-enterprise-hpe/master/_listings/hewlett-packard-enterprise-hpe/projects-post-openapi.md
- name: HPE OneSphere API - Delete Projects
  x-api-slug: projectsid-delete
  description: Deletes a project. If resources (currently Deployments) exist within
    the project they must first be deleted. In this case, the response will be a 409
    Conflict with the body listing the first ten offending items. It requires **administratpor**
    global role or **owner** project role. **not implemented**
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/HPE-logo.png
  humanURL: http://HPE.com
  baseURL: https://deic02-hpe.hpeonesphere.com//rest
  tags: Enterprise, Cloud, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/hewlett-packard-enterprise-hpe/master/_listings/hewlett-packard-enterprise-hpe/projectsid-delete-openapi.md
- name: HPE OneSphere API - Get Projects
  x-api-slug: projectsid-get
  description: Returns a project based on its id. It requires any project role or
    non-consumer global role.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/HPE-logo.png
  humanURL: http://HPE.com
  baseURL: https://deic02-hpe.hpeonesphere.com//rest
  tags: Enterprise, Cloud, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/hewlett-packard-enterprise-hpe/master/_listings/hewlett-packard-enterprise-hpe/projectsid-get-openapi.md
- name: HPE OneSphere API - Patch Projects
  x-api-slug: projectsid-patch
  description: Updates a project. It requires the **administrator** global role or
    the **project owner** role on a project.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/HPE-logo.png
  humanURL: http://HPE.com
  baseURL: https://deic02-hpe.hpeonesphere.com//rest
  tags: Enterprise, Cloud, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/hewlett-packard-enterprise-hpe/master/_listings/hewlett-packard-enterprise-hpe/projectsid-patch-openapi.md
- name: HPE OneSphere API - Get Prover Types
  x-api-slug: providertypes-get
  description: Returns provider types.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/HPE-logo.png
  humanURL: http://HPE.com
  baseURL: https://deic02-hpe.hpeonesphere.com//rest
  tags: Enterprise, Cloud, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/hewlett-packard-enterprise-hpe/master/_listings/hewlett-packard-enterprise-hpe/providertypes-get-openapi.md
- name: HPE OneSphere API - Get Provers
  x-api-slug: providers-get
  description: Returns providers. It requires the **consumer** global role.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/HPE-logo.png
  humanURL: http://HPE.com
  baseURL: https://deic02-hpe.hpeonesphere.com//rest
  tags: Enterprise, Cloud, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/hewlett-packard-enterprise-hpe/master/_listings/hewlett-packard-enterprise-hpe/providers-get-openapi.md
- name: HPE OneSphere API - Post Provers
  x-api-slug: providers-post
  description: Creates a new Master provider or Member provider.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/HPE-logo.png
  humanURL: http://HPE.com
  baseURL: https://deic02-hpe.hpeonesphere.com//rest
  tags: Enterprise, Cloud, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/hewlett-packard-enterprise-hpe/master/_listings/hewlett-packard-enterprise-hpe/providers-post-openapi.md
- name: HPE OneSphere API - Delete Provers
  x-api-slug: providersid-delete
  description: Deletes a master provider or a child provider
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/HPE-logo.png
  humanURL: http://HPE.com
  baseURL: https://deic02-hpe.hpeonesphere.com//rest
  tags: Enterprise, Cloud, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/hewlett-packard-enterprise-hpe/master/_listings/hewlett-packard-enterprise-hpe/providersid-delete-openapi.md
- name: HPE OneSphere API - Get Provers
  x-api-slug: providersid-get
  description: Returns a provider based on its id. It requires the **consumer** global
    role.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/HPE-logo.png
  humanURL: http://HPE.com
  baseURL: https://deic02-hpe.hpeonesphere.com//rest
  tags: Enterprise, Cloud, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/hewlett-packard-enterprise-hpe/master/_listings/hewlett-packard-enterprise-hpe/providersid-get-openapi.md
- name: HPE OneSphere API - Patch Provers
  x-api-slug: providersid-patch
  description: Updates a provider.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/HPE-logo.png
  humanURL: http://HPE.com
  baseURL: https://deic02-hpe.hpeonesphere.com//rest
  tags: Enterprise, Cloud, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/hewlett-packard-enterprise-hpe/master/_listings/hewlett-packard-enterprise-hpe/providersid-patch-openapi.md
- name: HPE OneSphere API - Get Rates
  x-api-slug: rates-get
  description: |-
    Returns rates. It requires the **administrator** global role.

    Optionally this list may be filtered, or the default rates specified with a resourceUri of 'default'.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/HPE-logo.png
  humanURL: http://HPE.com
  baseURL: https://deic02-hpe.hpeonesphere.com//rest
  tags: Enterprise, Cloud, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/hewlett-packard-enterprise-hpe/master/_listings/hewlett-packard-enterprise-hpe/rates-get-openapi.md
- name: HPE OneSphere API - Get Rates
  x-api-slug: ratesid-get
  description: Retrieve a rate by id. It requires the **administrator** global role.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/HPE-logo.png
  humanURL: http://HPE.com
  baseURL: https://deic02-hpe.hpeonesphere.com//rest
  tags: Enterprise, Cloud, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/hewlett-packard-enterprise-hpe/master/_listings/hewlett-packard-enterprise-hpe/ratesid-get-openapi.md
- name: HPE OneSphere API - Get Regions
  x-api-slug: regions-get
  description: Returns regions. It requires the **consumer** global role.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/HPE-logo.png
  humanURL: http://HPE.com
  baseURL: https://deic02-hpe.hpeonesphere.com//rest
  tags: Enterprise, Cloud, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/hewlett-packard-enterprise-hpe/master/_listings/hewlett-packard-enterprise-hpe/regions-get-openapi.md
- name: HPE OneSphere API - Post Regions
  x-api-slug: regions-post
  description: Creates a new region.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/HPE-logo.png
  humanURL: http://HPE.com
  baseURL: https://deic02-hpe.hpeonesphere.com//rest
  tags: Enterprise, Cloud, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/hewlett-packard-enterprise-hpe/master/_listings/hewlett-packard-enterprise-hpe/regions-post-openapi.md
- name: HPE OneSphere API - Delete Regions
  x-api-slug: regionsid-delete
  description: Deletes a region
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/HPE-logo.png
  humanURL: http://HPE.com
  baseURL: https://deic02-hpe.hpeonesphere.com//rest
  tags: Enterprise, Cloud, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/hewlett-packard-enterprise-hpe/master/_listings/hewlett-packard-enterprise-hpe/regionsid-delete-openapi.md
- name: HPE OneSphere API - Get Regions
  x-api-slug: regionsid-get
  description: Returns a region based on its id. It requires the **consumer** global
    role.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/HPE-logo.png
  humanURL: http://HPE.com
  baseURL: https://deic02-hpe.hpeonesphere.com//rest
  tags: Enterprise, Cloud, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/hewlett-packard-enterprise-hpe/master/_listings/hewlett-packard-enterprise-hpe/regionsid-get-openapi.md
- name: HPE OneSphere API - Patch Regions
  x-api-slug: regionsid-patch
  description: Patches a region. PATCH only supports provider type(/rest/provider-types/ncs).
    Allowed fields to PATCH for NCS provider type are (name,location)
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/HPE-logo.png
  humanURL: http://HPE.com
  baseURL: https://deic02-hpe.hpeonesphere.com//rest
  tags: Enterprise, Cloud, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/hewlett-packard-enterprise-hpe/master/_listings/hewlett-packard-enterprise-hpe/regionsid-patch-openapi.md
- name: HPE OneSphere API - Put Regions
  x-api-slug: regionsid-put
  description: Updates a region. **Not implemented**
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/HPE-logo.png
  humanURL: http://HPE.com
  baseURL: https://deic02-hpe.hpeonesphere.com//rest
  tags: Enterprise, Cloud, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/hewlett-packard-enterprise-hpe/master/_listings/hewlett-packard-enterprise-hpe/regionsid-put-openapi.md
- name: HPE OneSphere API - Delete Regions Connection
  x-api-slug: regionsidconnection-delete
  description: ""
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/HPE-logo.png
  humanURL: http://HPE.com
  baseURL: https://deic02-hpe.hpeonesphere.com//rest
  tags: Enterprise, Cloud, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/hewlett-packard-enterprise-hpe/master/_listings/hewlett-packard-enterprise-hpe/regionsidconnection-delete-openapi.md
- name: HPE OneSphere API - Get Regions Connection
  x-api-slug: regionsidconnection-get
  description: Get region connection.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/HPE-logo.png
  humanURL: http://HPE.com
  baseURL: https://deic02-hpe.hpeonesphere.com//rest
  tags: Enterprise, Cloud, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/hewlett-packard-enterprise-hpe/master/_listings/hewlett-packard-enterprise-hpe/regionsidconnection-get-openapi.md
- name: HPE OneSphere API - Post Regions Connection
  x-api-slug: regionsidconnection-post
  description: Creates a new region connection
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/HPE-logo.png
  humanURL: http://HPE.com
  baseURL: https://deic02-hpe.hpeonesphere.com//rest
  tags: Enterprise, Cloud, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/hewlett-packard-enterprise-hpe/master/_listings/hewlett-packard-enterprise-hpe/regionsidconnection-post-openapi.md
- name: HPE OneSphere API - Get Regions Connector Image
  x-api-slug: regionsidconnectorimage-get
  description: Generates connector-image url for the region. It requires the **administrator**
    role.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/HPE-logo.png
  humanURL: http://HPE.com
  baseURL: https://deic02-hpe.hpeonesphere.com//rest
  tags: Enterprise, Cloud, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/hewlett-packard-enterprise-hpe/master/_listings/hewlett-packard-enterprise-hpe/regionsidconnectorimage-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/hewlett-packard-enterprise-hpe/master/_listings/hewlett-packard-enterprise-hpe/regionsidconnectorimage-get-openapi.md
- name: HPE OneSphere API - Get Roles
  x-api-slug: roles-get
  description: Returns global roles.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/HPE-logo.png
  humanURL: http://HPE.com
  baseURL: https://deic02-hpe.hpeonesphere.com//rest
  tags: Enterprise, Cloud, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/hewlett-packard-enterprise-hpe/master/_listings/hewlett-packard-enterprise-hpe/roles-get-openapi.md
- name: HPE OneSphere API - Get Servers
  x-api-slug: servers-get
  description: Returns servers.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/HPE-logo.png
  humanURL: http://HPE.com
  baseURL: https://deic02-hpe.hpeonesphere.com//rest
  tags: Enterprise, Cloud, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/hewlett-packard-enterprise-hpe/master/_listings/hewlett-packard-enterprise-hpe/servers-get-openapi.md
- name: HPE OneSphere API - Post Servers
  x-api-slug: servers-post
  description: Create/Register a server.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/HPE-logo.png
  humanURL: http://HPE.com
  baseURL: https://deic02-hpe.hpeonesphere.com//rest
  tags: Enterprise, Cloud, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/hewlett-packard-enterprise-hpe/master/_listings/hewlett-packard-enterprise-hpe/servers-post-openapi.md
- name: HPE OneSphere API - Delete Servers
  x-api-slug: serversid-delete
  description: |-
    Delete a server.
    Note that by default only servers created via the HPE OneSphere API can be
    subsequently deleted. HPE OneSphere managed servers (those that have
    an applianceUri) cannot be deleted via this operation (a '403' will be returned),
    unless the 'force' parameter is supplied and set to 'true'.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/HPE-logo.png
  humanURL: http://HPE.com
  baseURL: https://deic02-hpe.hpeonesphere.com//rest
  tags: Enterprise, Cloud, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/hewlett-packard-enterprise-hpe/master/_listings/hewlett-packard-enterprise-hpe/serversid-delete-openapi.md
- name: HPE OneSphere API - Get Servers
  x-api-slug: serversid-get
  description: Returns a server based on its ID.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/HPE-logo.png
  humanURL: http://HPE.com
  baseURL: https://deic02-hpe.hpeonesphere.com//rest
  tags: Enterprise, Cloud, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/hewlett-packard-enterprise-hpe/master/_listings/hewlett-packard-enterprise-hpe/serversid-get-openapi.md
- name: HPE OneSphere API - Patch Servers
  x-api-slug: serversid-patch
  description: Update properties of a server.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/HPE-logo.png
  humanURL: http://HPE.com
  baseURL: https://deic02-hpe.hpeonesphere.com//rest
  tags: Enterprise, Cloud, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/hewlett-packard-enterprise-hpe/master/_listings/hewlett-packard-enterprise-hpe/serversid-patch-openapi.md
- name: HPE OneSphere API - Get Service Types
  x-api-slug: servicetypes-get
  description: Returns all service types. It requires the **consumer** global role.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/HPE-logo.png
  humanURL: http://HPE.com
  baseURL: https://deic02-hpe.hpeonesphere.com//rest
  tags: Enterprise, Cloud, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/hewlett-packard-enterprise-hpe/master/_listings/hewlett-packard-enterprise-hpe/servicetypes-get-openapi.md
- name: HPE OneSphere API - Get Service Types
  x-api-slug: servicetypesid-get
  description: Return a service type based on its id. It requires the **consumer**
    global role.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/HPE-logo.png
  humanURL: http://HPE.com
  baseURL: https://deic02-hpe.hpeonesphere.com//rest
  tags: Enterprise, Cloud, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/hewlett-packard-enterprise-hpe/master/_listings/hewlett-packard-enterprise-hpe/servicetypesid-get-openapi.md
- name: HPE OneSphere API - Get Services
  x-api-slug: services-get
  description: Returns services. It requires any project role or non-'consumer' global
    role.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/HPE-logo.png
  humanURL: http://HPE.com
  baseURL: https://deic02-hpe.hpeonesphere.com//rest
  tags: Enterprise, Cloud, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/hewlett-packard-enterprise-hpe/master/_listings/hewlett-packard-enterprise-hpe/services-get-openapi.md
- name: HPE OneSphere API - Get Services
  x-api-slug: servicesid-get
  description: Returns a service based on its id. It requires any project role or
    non-'consumer' global role.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/HPE-logo.png
  humanURL: http://HPE.com
  baseURL: https://deic02-hpe.hpeonesphere.com//rest
  tags: Enterprise, Cloud, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/hewlett-packard-enterprise-hpe/master/_listings/hewlett-packard-enterprise-hpe/servicesid-get-openapi.md
- name: HPE OneSphere API - Delete Session
  x-api-slug: session-delete
  description: Deletes cached data and tokens for the current session.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/HPE-logo.png
  humanURL: http://HPE.com
  baseURL: https://deic02-hpe.hpeonesphere.com//rest
  tags: Enterprise, Cloud, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/hewlett-packard-enterprise-hpe/master/_listings/hewlett-packard-enterprise-hpe/session-delete-openapi.md
- name: HPE OneSphere API - Get Session
  x-api-slug: session-get
  description: Gets information for the current user.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/HPE-logo.png
  humanURL: http://HPE.com
  baseURL: https://deic02-hpe.hpeonesphere.com//rest
  tags: Enterprise, Cloud, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/hewlett-packard-enterprise-hpe/master/_listings/hewlett-packard-enterprise-hpe/session-get-openapi.md
- name: HPE OneSphere API - Post Session
  x-api-slug: session-post
  description: |-
    Authenticates a local user and generates an authorization token. This
    token should be used in subsequent HTTP requests as part of
    the "Authorization" header. For example:

    `Authorization: "Bearer <token>"`
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/HPE-logo.png
  humanURL: http://HPE.com
  baseURL: https://deic02-hpe.hpeonesphere.com//rest
  tags: Enterprise, Cloud, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/hewlett-packard-enterprise-hpe/master/_listings/hewlett-packard-enterprise-hpe/session-post-openapi.md
- name: HPE OneSphere API - Get Session P
  x-api-slug: sessionidp-get
  description: |-
    **Not implemented**

    Gets the Identity Provider login URL for a userName.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/HPE-logo.png
  humanURL: http://HPE.com
  baseURL: https://deic02-hpe.hpeonesphere.com//rest
  tags: Enterprise, Cloud, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/hewlett-packard-enterprise-hpe/master/_listings/hewlett-packard-enterprise-hpe/sessionidp-get-openapi.md
- name: HPE OneSphere API - Get Session Sso
  x-api-slug: sessionsso-get
  description: Get the redirect URL for a configured SSO provider
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/HPE-logo.png
  humanURL: http://HPE.com
  baseURL: https://deic02-hpe.hpeonesphere.com//rest
  tags: Enterprise, Cloud, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/hewlett-packard-enterprise-hpe/master/_listings/hewlett-packard-enterprise-hpe/sessionsso-get-openapi.md
- name: HPE OneSphere API - Post Session Sso
  x-api-slug: sessionsso-post
  description: Callback for SSO login
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/HPE-logo.png
  humanURL: http://HPE.com
  baseURL: https://deic02-hpe.hpeonesphere.com//rest
  tags: Enterprise, Cloud, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/hewlett-packard-enterprise-hpe/master/_listings/hewlett-packard-enterprise-hpe/sessionsso-post-openapi.md
- name: HPE OneSphere API - Get Status
  x-api-slug: status-get
  description: Checks the service is running. It does not require authorization.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/HPE-logo.png
  humanURL: http://HPE.com
  baseURL: https://deic02-hpe.hpeonesphere.com//rest
  tags: Enterprise, Cloud, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/hewlett-packard-enterprise-hpe/master/_listings/hewlett-packard-enterprise-hpe/status-get-openapi.md
- name: HPE OneSphere API - Get Tag Keys
  x-api-slug: tagkeys-get
  description: Lists tag keys.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/HPE-logo.png
  humanURL: http://HPE.com
  baseURL: https://deic02-hpe.hpeonesphere.com//rest
  tags: Enterprise, Cloud, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/hewlett-packard-enterprise-hpe/master/_listings/hewlett-packard-enterprise-hpe/tagkeys-get-openapi.md
- name: HPE OneSphere API - Post Tag Keys
  x-api-slug: tagkeys-post
  description: Create a tag key. It requires the **analyst** global role.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/HPE-logo.png
  humanURL: http://HPE.com
  baseURL: https://deic02-hpe.hpeonesphere.com//rest
  tags: Enterprise, Cloud, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/hewlett-packard-enterprise-hpe/master/_listings/hewlett-packard-enterprise-hpe/tagkeys-post-openapi.md
- name: HPE OneSphere API - Delete Tag Keys
  x-api-slug: tagkeysid-delete
  description: Delete a tag key and associated tags. It requires the **analyst** global
    role.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/HPE-logo.png
  humanURL: http://HPE.com
  baseURL: https://deic02-hpe.hpeonesphere.com//rest
  tags: Enterprise, Cloud, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/hewlett-packard-enterprise-hpe/master/_listings/hewlett-packard-enterprise-hpe/tagkeysid-delete-openapi.md
- name: HPE OneSphere API - Get Tag Keys
  x-api-slug: tagkeysid-get
  description: Returns a tag key based on its id.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/HPE-logo.png
  humanURL: http://HPE.com
  baseURL: https://deic02-hpe.hpeonesphere.com//rest
  tags: Enterprise, Cloud, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/hewlett-packard-enterprise-hpe/master/_listings/hewlett-packard-enterprise-hpe/tagkeysid-get-openapi.md
- name: HPE OneSphere API - Get Tags
  x-api-slug: tags-get
  description: Lists tags.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/HPE-logo.png
  humanURL: http://HPE.com
  baseURL: https://deic02-hpe.hpeonesphere.com//rest
  tags: Enterprise, Cloud, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/hewlett-packard-enterprise-hpe/master/_listings/hewlett-packard-enterprise-hpe/tags-get-openapi.md
- name: HPE OneSphere API - Post Tags
  x-api-slug: tags-post
  description: Create a tag. It requires the **analyst** global role.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/HPE-logo.png
  humanURL: http://HPE.com
  baseURL: https://deic02-hpe.hpeonesphere.com//rest
  tags: Enterprise, Cloud, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/hewlett-packard-enterprise-hpe/master/_listings/hewlett-packard-enterprise-hpe/tags-post-openapi.md
- name: HPE OneSphere API - Delete Tags
  x-api-slug: tagsid-delete
  description: Delete a tag. It requires the **analyst** global role.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/HPE-logo.png
  humanURL: http://HPE.com
  baseURL: https://deic02-hpe.hpeonesphere.com//rest
  tags: Enterprise, Cloud, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/hewlett-packard-enterprise-hpe/master/_listings/hewlett-packard-enterprise-hpe/tagsid-delete-openapi.md
- name: HPE OneSphere API - Get Tags
  x-api-slug: tagsid-get
  description: Returns a tag based on its id. It requires the **consumer** global
    role.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/HPE-logo.png
  humanURL: http://HPE.com
  baseURL: https://deic02-hpe.hpeonesphere.com//rest
  tags: Enterprise, Cloud, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/hewlett-packard-enterprise-hpe/master/_listings/hewlett-packard-enterprise-hpe/tagsid-get-openapi.md
- name: HPE OneSphere API - Get Users
  x-api-slug: users-get
  description: Returns users.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/HPE-logo.png
  humanURL: http://HPE.com
  baseURL: https://deic02-hpe.hpeonesphere.com//rest
  tags: Enterprise, Cloud, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/hewlett-packard-enterprise-hpe/master/_listings/hewlett-packard-enterprise-hpe/users-get-openapi.md
- name: HPE OneSphere API - Post Users
  x-api-slug: users-post
  description: |-
    Create a user. It requires the **administrator** or **project creator** global role.

    The password should be a minimum of 8 characters long.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/HPE-logo.png
  humanURL: http://HPE.com
  baseURL: https://deic02-hpe.hpeonesphere.com//rest
  tags: Enterprise, Cloud, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/hewlett-packard-enterprise-hpe/master/_listings/hewlett-packard-enterprise-hpe/users-post-openapi.md
- name: HPE OneSphere API - Delete Users
  x-api-slug: usersid-delete
  description: Delete a user. It requires the **administrator** or **project creator**
    global role.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/HPE-logo.png
  humanURL: http://HPE.com
  baseURL: https://deic02-hpe.hpeonesphere.com//rest
  tags: Enterprise, Cloud, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/hewlett-packard-enterprise-hpe/master/_listings/hewlett-packard-enterprise-hpe/usersid-delete-openapi.md
- name: HPE OneSphere API - Get Users
  x-api-slug: usersid-get
  description: Returns a user based on its id. It requires the **administrator** or
    **project creator** global role, or matching user id.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/HPE-logo.png
  humanURL: http://HPE.com
  baseURL: https://deic02-hpe.hpeonesphere.com//rest
  tags: Enterprise, Cloud, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/hewlett-packard-enterprise-hpe/master/_listings/hewlett-packard-enterprise-hpe/usersid-get-openapi.md
- name: HPE OneSphere API - Patch Users
  x-api-slug: usersid-patch
  description: |-
    Update a user. It requires the **administrator** or **project creator** global role or matching user ID.

    If the password is updated it must be a minimum of 8 characters long.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/HPE-logo.png
  humanURL: http://HPE.com
  baseURL: https://deic02-hpe.hpeonesphere.com//rest
  tags: Enterprise, Cloud, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/hewlett-packard-enterprise-hpe/master/_listings/hewlett-packard-enterprise-hpe/usersid-patch-openapi.md
- name: HPE OneSphere API - Get Virtual Machine Profiles
  x-api-slug: virtualmachineprofiles-get
  description: Returns all virtual machine profiles. It requires any project role
    or non-'consumer' global role.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/HPE-logo.png
  humanURL: http://HPE.com
  baseURL: https://deic02-hpe.hpeonesphere.com//rest
  tags: Enterprise, Cloud, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/hewlett-packard-enterprise-hpe/master/_listings/hewlett-packard-enterprise-hpe/virtualmachineprofiles-get-openapi.md
- name: HPE OneSphere API - Get Virtual Machine Profiles
  x-api-slug: virtualmachineprofilesid-get
  description: Returns a virtual machine profile based on its id. It equires any project
    role or non-'consumer' global role.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/HPE-logo.png
  humanURL: http://HPE.com
  baseURL: https://deic02-hpe.hpeonesphere.com//rest
  tags: Enterprise, Cloud, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/hewlett-packard-enterprise-hpe/master/_listings/hewlett-packard-enterprise-hpe/virtualmachineprofilesid-get-openapi.md
- name: HPE OneSphere API - Get Volumes
  x-api-slug: volumes-get
  description: Returns volumes. It requires any project role or non-'consumer' global
    role.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/HPE-logo.png
  humanURL: http://HPE.com
  baseURL: https://deic02-hpe.hpeonesphere.com//rest
  tags: Enterprise, Cloud, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/hewlett-packard-enterprise-hpe/master/_listings/hewlett-packard-enterprise-hpe/volumes-get-openapi.md
- name: HPE OneSphere API - Post Volumes
  x-api-slug: volumes-post
  description: Creates a new volume. It requires any project role or the **administrator**
    or **project creator** global role.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/HPE-logo.png
  humanURL: http://HPE.com
  baseURL: https://deic02-hpe.hpeonesphere.com//rest
  tags: Enterprise, Cloud, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/hewlett-packard-enterprise-hpe/master/_listings/hewlett-packard-enterprise-hpe/volumes-post-openapi.md
- name: HPE OneSphere API - Delete Volumes
  x-api-slug: volumesid-delete
  description: Delete a volume. It requires any project role or the **administrator**
    or **project creator** global role.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/HPE-logo.png
  humanURL: http://HPE.com
  baseURL: https://deic02-hpe.hpeonesphere.com//rest
  tags: Enterprise, Cloud, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/hewlett-packard-enterprise-hpe/master/_listings/hewlett-packard-enterprise-hpe/volumesid-delete-openapi.md
- name: HPE OneSphere API - Get Volumes
  x-api-slug: volumesid-get
  description: Returns a volume based on its id. It requires any project role or non-'consumer'
    global role.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/HPE-logo.png
  humanURL: http://HPE.com
  baseURL: https://deic02-hpe.hpeonesphere.com//rest
  tags: Enterprise, Cloud, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/hewlett-packard-enterprise-hpe/master/_listings/hewlett-packard-enterprise-hpe/volumesid-get-openapi.md
- name: HPE OneSphere API - Patch Volumes
  x-api-slug: volumesid-patch
  description: Updates a volume. **Requires any project role or 'administrator' or
    'project creator' global role**. Allowed fields for PATCH of volumes are name(add,replace),
    size(add,replace)
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/HPE-logo.png
  humanURL: http://HPE.com
  baseURL: https://deic02-hpe.hpeonesphere.com//rest
  tags: Enterprise, Cloud, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/hewlett-packard-enterprise-hpe/master/_listings/hewlett-packard-enterprise-hpe/volumesid-patch-openapi.md
- name: HPE OneSphere API - Get Zone Types
  x-api-slug: zonetypes-get
  description: Returns all zone types.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/HPE-logo.png
  humanURL: http://HPE.com
  baseURL: https://deic02-hpe.hpeonesphere.com//rest
  tags: Enterprise, Cloud, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/hewlett-packard-enterprise-hpe/master/_listings/hewlett-packard-enterprise-hpe/zonetypes-get-openapi.md
- name: HPE OneSphere API - Get Zone Types Resource Profiles
  x-api-slug: zonetypesidresourceprofiles-get
  description: Returns all available resourceProfile for **vcenter zone type**. It
    requires the **administrator** role.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/HPE-logo.png
  humanURL: http://HPE.com
  baseURL: https://deic02-hpe.hpeonesphere.com//rest
  tags: Enterprise, Cloud, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/hewlett-packard-enterprise-hpe/master/_listings/hewlett-packard-enterprise-hpe/zonetypesidresourceprofiles-get-openapi.md
- name: HPE OneSphere API - Get Zones
  x-api-slug: zones-get
  description: Returns zones.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/HPE-logo.png
  humanURL: http://HPE.com
  baseURL: https://deic02-hpe.hpeonesphere.com//rest
  tags: Enterprise, Cloud, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/hewlett-packard-enterprise-hpe/master/_listings/hewlett-packard-enterprise-hpe/zones-get-openapi.md
- name: HPE OneSphere API - Post Zones
  x-api-slug: zones-post
  description: Creates a new zone
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/HPE-logo.png
  humanURL: http://HPE.com
  baseURL: https://deic02-hpe.hpeonesphere.com//rest
  tags: Enterprise, Cloud, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/hewlett-packard-enterprise-hpe/master/_listings/hewlett-packard-enterprise-hpe/zones-post-openapi.md
- name: HPE OneSphere API - Delete Zones
  x-api-slug: zonesid-delete
  description: Deletes a zone
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/HPE-logo.png
  humanURL: http://HPE.com
  baseURL: https://deic02-hpe.hpeonesphere.com//rest
  tags: Enterprise, Cloud, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/hewlett-packard-enterprise-hpe/master/_listings/hewlett-packard-enterprise-hpe/zonesid-delete-openapi.md
- name: HPE OneSphere API - Get Zones
  x-api-slug: zonesid-get
  description: Returns a zone based on its id.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/HPE-logo.png
  humanURL: http://HPE.com
  baseURL: https://deic02-hpe.hpeonesphere.com//rest
  tags: Enterprise, Cloud, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/hewlett-packard-enterprise-hpe/master/_listings/hewlett-packard-enterprise-hpe/zonesid-get-openapi.md
- name: HPE OneSphere API - Patch Zones
  x-api-slug: zonesid-patch
  description: Updates a zone
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/HPE-logo.png
  humanURL: http://HPE.com
  baseURL: https://deic02-hpe.hpeonesphere.com//rest
  tags: Enterprise, Cloud, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/hewlett-packard-enterprise-hpe/master/_listings/hewlett-packard-enterprise-hpe/zonesid-patch-openapi.md
- name: HPE OneSphere API - Post Zones Actions
  x-api-slug: zonesidactions-post
  description: Peforms an action to the zone. It requires the **administrator** role.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/HPE-logo.png
  humanURL: http://HPE.com
  baseURL: https://deic02-hpe.hpeonesphere.com//rest
  tags: Enterprise, Cloud, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/hewlett-packard-enterprise-hpe/master/_listings/hewlett-packard-enterprise-hpe/zonesidactions-post-openapi.md
- name: HPE OneSphere API - Get Zones Appliance Image
  x-api-slug: zonesidapplianceimage-get
  description: Generates appliance-image url for the zone
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/HPE-logo.png
  humanURL: http://HPE.com
  baseURL: https://deic02-hpe.hpeonesphere.com//rest
  tags: Enterprise, Cloud, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/hewlett-packard-enterprise-hpe/master/_listings/hewlett-packard-enterprise-hpe/zonesidapplianceimage-get-openapi.md
- name: HPE OneSphere API - Get Zones Connections
  x-api-slug: zonesidconnections-get
  description: Gets the list of connection for the zone. It requires the **administrator**
    role.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/HPE-logo.png
  humanURL: http://HPE.com
  baseURL: https://deic02-hpe.hpeonesphere.com//rest
  tags: Enterprise, Cloud, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/hewlett-packard-enterprise-hpe/master/_listings/hewlett-packard-enterprise-hpe/zonesidconnections-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/hewlett-packard-enterprise-hpe/master/_listings/hewlett-packard-enterprise-hpe/zonesidconnections-get-openapi.md
- name: HPE OneSphere API - Post Zones Connections
  x-api-slug: zonesidconnections-post
  description: Peforms an action to the zone. It requires the **administrator** role.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/HPE-logo.png
  humanURL: http://HPE.com
  baseURL: https://deic02-hpe.hpeonesphere.com//rest
  tags: Enterprise, Cloud, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/hewlett-packard-enterprise-hpe/master/_listings/hewlett-packard-enterprise-hpe/zonesidconnections-post-openapi.md
- name: HPE OneSphere API - Delete Zones Connections Uu
  x-api-slug: zonesidconnectionsuuid-delete
  description: Deletes a connection instance of the zone
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/HPE-logo.png
  humanURL: http://HPE.com
  baseURL: https://deic02-hpe.hpeonesphere.com//rest
  tags: Enterprise, Cloud, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/hewlett-packard-enterprise-hpe/master/_listings/hewlett-packard-enterprise-hpe/zonesidconnectionsuuid-delete-openapi.md
- name: HPE OneSphere API - Patch Zones Connections Uu
  x-api-slug: zonesidconnectionsuuid-patch
  description: Updates a connection of the zone.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/HPE-logo.png
  humanURL: http://HPE.com
  baseURL: https://deic02-hpe.hpeonesphere.com//rest
  tags: Enterprise, Cloud, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/hewlett-packard-enterprise-hpe/master/_listings/hewlett-packard-enterprise-hpe/zonesidconnectionsuuid-patch-openapi.md
- name: HPE OneSphere API - Get Zones Task Status
  x-api-slug: zonesidtaskstatus-get
  description: Returns the status of the task for the zone
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/HPE-logo.png
  humanURL: http://HPE.com
  baseURL: https://deic02-hpe.hpeonesphere.com//rest
  tags: Enterprise, Cloud, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/hewlett-packard-enterprise-hpe/master/_listings/hewlett-packard-enterprise-hpe/zonesidtaskstatus-get-openapi.md
x-common:
- type: x-developer
  url: https://developer.hpe.com/
- type: x-github
  url: https://github.com/hewlettpackard
- type: x-openapi
  url: https://raw.githubusercontent.com/HewlettPackard/hpe-onesphere-http/master/swagger.yml
- type: x-twitter
  url: https://twitter.com/HPE
- type: x-website
  url: http://HPE.com
- type: x-api-gallery
  url: http://heroku.api.gallery.streamdata.io
- type: x-api-stack
  url: http://hewlett.packard.enterprise.hpe.stack.network
- type: x-blog
  url: https://developer.hpe.com/blog
- type: x-curated-source
  url: http://community.hpe.com/t5/LoadRunner-and-Performance/LoadRunner-and-VuGen-12-53-load-testing-software-What-s-new-in/ba-p/6885101
- type: x-website
  url: https://www.hpe.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---