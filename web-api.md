#Create

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

##Component

**URL**: /api/components

**Method**: PUT

**Content Type**: application/json; charset=utf-8

**Data Type**: JSON

**Data**: [see Create -> Component]

**Success**: (data)
- data [see Create -> Component]

**Error**: (xhr, status, err)

#Restore

##Component

**URL**: /api/components/restore/{id}

**Method**: POST

**Content Type**: application/json; charset=utf-8

**Data Type**: JSON

**Success**: (data)
- data [see Delete -> Component]

**Error**: (xhr, status, err)

#Move

##Node

**URL**: /api/components/move/{id}/to/{newParentId}/{newIndex}

**Method**: POST

**Content Type**: application/json; charset=utf-8

**Data Type**: JSON

**Success**: (data)
- data [see Delete -> Component]

**Error**: (xhr, status, err)
