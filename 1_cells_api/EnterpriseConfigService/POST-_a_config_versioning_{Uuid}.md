






 
[Enterprise Only] Create or update a versioning policy  


### Body Parameters

Name | Description | Type | Required
---|---|---|---
**Description** |  | _string_ |   
**IgnoreFilesGreaterThan** |  | _string_ |   
**KeepPeriods** |  | _array_ |   
**MaxSizePerFile** |  | _string_ |   
**MaxTotalSize** |  | _string_ |   
**Name** |  | _string_ |   
**Uuid** |  | _string_ |   
**VersionsDataSourceBucket** |  | _string_ |   
**VersionsDataSourceName** |  | _string_ |   


### Body Example
```
{
  "Description": "string",
  "IgnoreFilesGreaterThan": "string",
  "KeepPeriods": [
    {
      "IntervalStart": "string",
      "MaxNumber": 10
    }
  ],
  "MaxSizePerFile": "string",
  "MaxTotalSize": "string",
  "Name": "string",
  "Uuid": "string",
  "VersionsDataSourceBucket": "string",
  "VersionsDataSourceName": "string"
}
```






### Response Example (200)
Response Type /definitions/treeVersioningPolicy

```
{
  "Description": "string",
  "IgnoreFilesGreaterThan": "string",
  "KeepPeriods": [
    {
      "IntervalStart": "string",
      "MaxNumber": 10
    }
  ],
  "MaxSizePerFile": "string",
  "MaxTotalSize": "string",
  "Name": "string",
  "Uuid": "string",
  "VersionsDataSourceBucket": "string",
  "VersionsDataSourceName": "string"
}
```

