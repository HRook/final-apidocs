# List thumbnails

Retrieve a list of thumbnailset objects.
### Prerequisites
The following **scopes** are required to execute this API: 
### HTTP request
<!-- { "blockType": "ignored" } -->
```http
GET /drive/root/thumbnails
GET /drive/items/<id>/thumbnails
GET /drives/<id>/root/thumbnails
```
### Optional query parameters
This method supports the [OData Query Parameters](http://graph.microsoft.io/docs/overview/query_parameters) to help customize the response.

### Request headers
| Name       | Type | Description|
|:-----------|:------|:----------|
| Authorization  | string  | Bearer <token>. Required. |

### Request body
Do not supply a request body for this method.
### Response
If successful, this method returns a `200 OK` response code and collection of [thumbnailSet](../resources/thumbnailset.md) objects in the response body.
### Example
##### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_thumbnails"
}-->
```http
GET https://graph.microsoft.com/beta/drive/root/thumbnails
```
##### Response
Here is an example of the response.
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.thumbnailset",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 585

{
  "value": [
    {
      "id": "id-value",
      "large": {
        "content": "content-value",
        "height": 99,
        "url": "url-value",
        "width": 99
      },
      "medium": {
        "content": "content-value",
        "height": 99,
        "url": "url-value",
        "width": 99
      },
      "small": {
        "content": "content-value",
        "height": 99,
        "url": "url-value",
        "width": 99
      },
      "source": {
        "content": "content-value",
        "height": 99,
        "url": "url-value",
        "width": 99
      }
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List thumbnails",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->