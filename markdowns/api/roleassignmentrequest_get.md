# Get roleAssignmentRequest

Retrieve the properties and relationships of roleassignmentrequest object.
### Prerequisites
The following **scopes** are required to execute this API: 
### HTTP request
<!-- { "blockType": "ignored" } -->
```http
GET /roleAssignmentRequests/<id>
GET /providers/<id>/roleAssignmentRequests/<id>
```
### Optional query parameters
This method supports the [OData Query Parameters](http://graph.microsoft.io/docs/overview/query_parameters) to help customize the response.

### Request headers
| Name      |Description|
|:----------|:----------|
| Authorization  | Bearer {code}|
| Workbook-Session-Id  | Workbook session Id that determines if changes are persisted or not. Optional.|

### Request body
Do not supply a request body for this method.
### Response
If successful, this method returns a `200 OK` response code and [roleAssignmentRequest](../resources/roleassignmentrequest.md) object in the response body.
### Example
##### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_roleassignmentrequest"
}-->
```http
GET https://graph.microsoft.com/beta/providers('00000000-0000-0000-0000-000000000002')/roleAssignmentRequests/<id>
```
##### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.roleAssignmentRequest"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 226

{
  "id": "id-value",
  "assignmentLevel": "assignmentLevel-value",
  "requestType": "requestType-value",
  "requestedDateTime": "datetime-value",
  "roleAssignmentStartDateTime": "datetime-value",
  "status": "status-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get roleAssignmentRequest",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->