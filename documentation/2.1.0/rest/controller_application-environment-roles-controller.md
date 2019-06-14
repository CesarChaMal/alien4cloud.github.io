---
layout: post
title: Manages application's environments
root: ../../
categories: DOCUMENTATION-2.1.0
parent: [rest_api, rest_api_applications-api]
node_name: rest_api_controller_application-environment-roles-controller
weight: 30
---

### Add a role to a group on a specific application environment
```
PUT /rest/v1/applications/{applicationId}/environments/{applicationEnvironmentId}/roles/groups/{groupId}/{role}
```

#### Description

Any user with application role APPLICATION_MANAGER can assign any role to a group of users. Application role required [ APPLICATION_MANAGER ]

#### Parameters

{: .table .table-bordered}
|Type|Name|Description|Required|Schema|Default|
|----|----|----|----|----|----|
|PathParameter|applicationEnvironmentId|applicationEnvironmentId|true|string||
|PathParameter|groupId|groupId|true|string||
|PathParameter|role|role|true|string||


#### Responses

{: .table .table-bordered}
|HTTP Code|Description|Schema|
|----|----|----|
|200|OK|RestResponse«Void»|
|201|Created|No Content|
|401|Unauthorized|No Content|
|403|Forbidden|No Content|
|404|Not Found|No Content|


#### Consumes

* application/json

#### Produces

* application/json

### Remove a role of a group on a specific application environment
```
DELETE /rest/v1/applications/{applicationId}/environments/{applicationEnvironmentId}/roles/groups/{groupId}/{role}
```

#### Description

Any user with application role APPLICATION_MANAGER can un-assign any role to a group. Application role required [ APPLICATION_MANAGER ]

#### Parameters

{: .table .table-bordered}
|Type|Name|Description|Required|Schema|Default|
|----|----|----|----|----|----|
|PathParameter|applicationEnvironmentId|applicationEnvironmentId|true|string||
|PathParameter|groupId|groupId|true|string||
|PathParameter|role|role|true|string||


#### Responses

{: .table .table-bordered}
|HTTP Code|Description|Schema|
|----|----|----|
|200|OK|RestResponse«Void»|
|401|Unauthorized|No Content|
|204|No Content|No Content|
|403|Forbidden|No Content|


#### Consumes

* application/json

#### Produces

* application/json

### Add a role to a user on a specific application environment
```
PUT /rest/v1/applications/{applicationId}/environments/{applicationEnvironmentId}/roles/users/{username}/{role}
```

#### Description

Any user with application role APPLICATION_MANAGER can assign any role to another user. Application role required [ APPLICATION_MANAGER ]

#### Parameters

{: .table .table-bordered}
|Type|Name|Description|Required|Schema|Default|
|----|----|----|----|----|----|
|PathParameter|applicationEnvironmentId|applicationEnvironmentId|true|string||
|PathParameter|username|username|true|string||
|PathParameter|role|role|true|string||


#### Responses

{: .table .table-bordered}
|HTTP Code|Description|Schema|
|----|----|----|
|200|OK|RestResponse«Void»|
|201|Created|No Content|
|401|Unauthorized|No Content|
|403|Forbidden|No Content|
|404|Not Found|No Content|


#### Consumes

* application/json

#### Produces

* application/json

### Remove a role to a user on a specific application environment
```
DELETE /rest/v1/applications/{applicationId}/environments/{applicationEnvironmentId}/roles/users/{username}/{role}
```

#### Description

Any user with application role APPLICATION_MANAGER can unassign any role to another user. Application role required [ APPLICATION_MANAGER ]

#### Parameters

{: .table .table-bordered}
|Type|Name|Description|Required|Schema|Default|
|----|----|----|----|----|----|
|PathParameter|applicationEnvironmentId|applicationEnvironmentId|true|string||
|PathParameter|username|username|true|string||
|PathParameter|role|role|true|string||


#### Responses

{: .table .table-bordered}
|HTTP Code|Description|Schema|
|----|----|----|
|200|OK|RestResponse«Void»|
|401|Unauthorized|No Content|
|204|No Content|No Content|
|403|Forbidden|No Content|


#### Consumes

* application/json

#### Produces

* application/json
