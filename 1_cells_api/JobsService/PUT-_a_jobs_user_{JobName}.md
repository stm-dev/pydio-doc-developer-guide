






 
Create a predefined job to be run directly  


### Body Parameters

Name | Description | Type | Required
---|---|---|---
**JobName** | Name of the job to create in the user space | _string_ |   
**JsonParameters** | Json-encoded parameters for this job | _string_ |   


### Body Example
```
{
  "JobName": "string",
  "JsonParameters": "string"
}
```






### Response Example (200)
Response Type /definitions/restUserJobResponse

```
{
  "JobUuid": "string"
}
```




###### Auto generated by Pydio Cells Home Edition v2.0.1 on 18-Nov-2019