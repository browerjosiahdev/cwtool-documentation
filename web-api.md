#Create

_How to create new items._

##Node

**URL**: /api/nodes

**Method**: POST

**Content Type**: application/json; charset=utf-8

**Data Type**: JSON

**Data**:
```javascript
{
	"parentId": 1,
	"componentId": 27,
	"javascriptProcessorId": 1,
	"styleProcessorId": 5,
	"name": "Test Shell",
	"nodeType": "Course",
	"publish": false,
	"relativePath": null,
	"canEdit": false,
	"canDelete": false,
	"projectName": null,
	"data": null,
	"processedData": null,
	"attachedData": null,
	"id": 0,
	"customGuid": null,
	"gggParentName": null,
	"ggParentName": null,
	"gParentName": null,
	"parentName": "BaNCS Systems Training",
	"componentName": null,
	"childComponentId": null,
	"projectId": 1,
	"isDeleted": false,
	"orderingIndex": 0,
	"isInDevelopment": false,
	"createdDate": "0001-01-01T00:00:00",
	"lastModifiedDate": "0001-01-01T00:00:00",
	"errors": null
}
```

**Success**: (data)
- data
```javascript
{
	"result": {
		"errors": null,
		"entity": {
			"canEdit": true,
			"canDelete": true,
			"projectName": "BaNCS Systems Training",
			"data": "{\"id\":\"p-285\",\"parentId\":\"ZionsShell\",\"template\":null,\"schema\":null,\"attachedSchema\":null,\"style\":null,\"globalStyle\":null,\"data\":\"{}\",\"previewShell\":null,\"javascript\":null,\"globalJavascript\":null,\"dynamicContent\":null,\"templateProcessorId\":0,\"javascriptProcessorId\":1,\"styleProcessorId\":5,\"languageOverrides\":null}",
			"processedData": "{\"id\":\"p-285\",\"parentId\":\"ZionsShell\",\"template\":null,\"schema\":null,\"attachedSchema\":null,\"style\":null,\"globalStyle\":null,\"data\":\"{}\",\"previewShell\":null,\"javascript\":null,\"globalJavascript\":null,\"dynamicContent\":null,\"templateProcessorId\":0,\"javascriptProcessorId\":1,\"styleProcessorId\":5,\"languageOverrides\":null}",
			"attachedData": null,
			"id": 285,
			"customGuid": null,
			"parentId": 1,
			"gggParentName": null,
			"ggParentName": null,
			"gParentName": null,
			"parentName": "BaNCS Systems Training",
			"componentId": 27,
			"componentName": "ZionsShell",
			"javascriptProcessorId": 1,
			"styleProcessorId": 5,
			"childComponentId": 1,
			"projectId": 1,
			"isDeleted": false,
			"orderingIndex": 9,
			"name": "Test Shell",
			"nodeType": "Course",
			"isInDevelopment": false,
			"publish": false,
			"relativePath": null,
			"createdDate": "0001-01-01T00:00:00",
			"lastModifiedDate": "0001-01-01T00:00:00",
			"errors": null
		}
	},
	"failed": false,
	"exception": null
}
```

**Error**: (xhr, status, err)

##Component

**URL**: /api/components

**Method**: POST

**Content Type**: application/json; charset=utf-8

**Data Type**: JSON

**Data**:
```javascript
{
  "parentId": 10,
  "baseComponentVersionId": null,
  "name": "AnotherTest",
  "templateProcessorId": 3,
  "javascriptProcessorId": 1,
  "styleProcessorId": 5,
  "canBeNode": true,
  "childComponentId": null,
  "canEdit": false,
  "canDelete": false,
  "canStyle": false,
  "project": null,
  "data": null,
  "processedData": null,
  "componentEdits": null,
  "id": 0,
  "parentName": "Zions5in5Captivate",
  "baseComponentVersionName": null,
  "isDeleted": false,
  "projectId": 1,
  "childComponentName": null,
  "createdDate": "0001-01-01T00:00:00",
  "lastModifiedDate": "0001-01-01T00:00:00",
  "errors": null
}
```

**Success**: (data)
- data
```javascript
{
  "result": {
    "errors": [{
      "field": "name",
      "message": "Component names may only contain letters and numbers."
    }],
    "entity": {
      "canEdit": true,
      "canDelete": true,
      "canStyle": true,
      "project": {
        "id": 1,
        "isDeleted": false,
        "name": "BaNCS Systems Training",
        "code": null,
        "organizationId": 2,
        "organizationName": "Zions",
        "repositoryId": 1,
        "repositoryName": "Default Repository",
        "createdDate": "2016-08-23T11:58:51.1090979",
        "lastModifiedDate": "2016-08-23T11:58:51.1090979"
      },
      "data": "{\"id\":\"AnotherTest\",\"parentId\":\"Zions5in5Captivate\",\"template\":null,\"schema\":\"{\\n}\",\"attachedSchema\":\"{\\n}\",\"style\":null,\"globalStyle\":null,\"data\":\"{\\n}\",\"previewShell\":null,\"javascript\":null,\"globalJavascript\":null,\"dynamicContent\":null,\"templateProcessorId\":3,\"javascriptProcessorId\":1,\"styleProcessorId\":5,\"languageOverrides\":null}",
      "processedData": "{\"id\":\"AnotherTest\",\"parentId\":\"Zions5in5Captivate\",\"template\":null,\"schema\":\"{\\n}\",\"attachedSchema\":\"{\\n}\",\"style\":null,\"globalStyle\":null,\"data\":\"{\\n}\",\"previewShell\":null,\"javascript\":null,\"globalJavascript\":null,\"dynamicContent\":null,\"templateProcessorId\":3,\"javascriptProcessorId\":1,\"styleProcessorId\":5,\"languageOverrides\":null}",
      "componentEdits": [],
      "id": 35,
      "parentId": 10,
      "parentName": "Zions5in5Captivate",
      "baseComponentVersionId": null,
      "baseComponentVersionName": " ..",
      "isDeleted": false,
      "projectId": 1,
      "name": "AnotherTest",
      "templateProcessorId": 3,
      "javascriptProcessorId": 1,
      "styleProcessorId": 5,
      "canBeNode": true,
      "childComponentId": null,
      "childComponentName": null,
      "createdDate": "2016-08-23T14:15:22.992945",
      "lastModifiedDate": "2016-08-23T14:15:22.992945",
      "errors": null
    }
  },
  "failed": false,
  "exception": null
}
```

**Error**: (xhr, status, err)

#Delete

_How to delete pre-existing items, or items that have been soft deleted._

##Node

**URL**: /api/nodes/{id}

**Method**: DELETE

**Content Type**: application/json; charset=utf-8

**Data Type**: JSON

**Data**: true/false (is permanent?)

**Success**: (data)
- data
```javascript
{
  "failed": false,
  "exception": null
}
```

**Error**: (xhr, status, err)

##Component

**URL**: /api/components/{id}

**Method**: DELETE

**Content Type**: application/json; charset=utf-8

**Data Type**: JSON

**Data**: true/false (is permanent?)

**Success**: (data)
- data
```javascript
{
  "failed": false,
  "exception": null
}
```

**Error**: (xhr, status, err)

#Update

_How to update data for pre-existing items._

##Node

**URL**: /api/nodes

**Method**: PUT

**Content Type**: application/json; charset=utf-8

**Data Type**: JSON

**Data**: _[see Create -> Node]_

**Success**: (data)
- data _[see Create -> Node]_

**Error**: (xhr, status, err)

##Component

**URL**: /api/components

**Method**: PUT

**Content Type**: application/json; charset=utf-8

**Data Type**: JSON

**Data**: _[see Create -> Component]_

**Success**: (data)
- data _[see Create -> Component]_

**Error**: (xhr, status, err)

#Restore

_How to restore items that have been soft deleted._

##Node

**URL**: /api/nodes/restore/{id}

**Method**: POST

**Content Type**: application/json; charset=utf-8

**Data Type**: JSON

**Success**: (data)
- data
```javascript
{
  "failed": false,
  "exception": null
}
```

**Error**: (xhr, status, err)

##Component

**URL**: /api/components/restore/{id}

**Method**: POST

**Content Type**: application/json; charset=utf-8

**Data Type**: JSON

**Success**: (data)
- data
```javascript
{
  "failed": false,
  "exception": null
}
```

**Error**: (xhr, status, err)

#Move

_How to update the parent/child relationship of items._

##Node

**URL**: /api/nodes/move/{id}/to/{newParentId}/{newIndex}

**Method**: POST

**Content Type**: application/json; charset=utf-8

**Data Type**: JSON

**Success**: (data)
- data
```javascript
{
  "failed": false,
  "exception": null
}
```

**Error**: (xhr, status, err)
