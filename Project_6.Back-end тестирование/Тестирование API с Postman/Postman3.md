## PUT/api/v1/Activities/{0}
- URL: **{{url глобал}}{{вся активность глобал}}/{{0}}**
- Ожидаемый результат: статус-код ответа **200**, тест успешно пройден
- Заголовки запроса: 
```javascript
Content-Type: "application/json"
User-Agent: "PostmanRuntime/7.32.3"
Accept: "*/*"
Cache-Control: "no-cache"
Postman-Token: "d0db613d-59ed-4d10-a94c-5db233426daa"
Host: "fakerestapi.azurewebsites.net"
Accept-Encoding: "gzip, deflate, br"
Connection: "keep-alive"
```
- Тело запроса:
```javascript
{
"id": 0, 
"title": "string",
"dueDate": "2023-06-22T08:32:29.719Z", 
"completed": true 
}
```
- Заголовки ответа:
```javascript
 access-control-allow-origin: * 
 api-supported-versions: 1.0 
 content-type: application/json; charset=utf-8; v=1.0 
 date: Thu22 Jun 2023 14:17:08 GMT 
 server: Kestrel 
 transfer-encoding: chunked 
 ```
- Тело ответа: 
```javascript
{
  "id": 0,
  "title": "string",
  "dueDate": "2023-06-22T14:17:09.044Z",
  "completed": true
}
```

## PUT/api​/v1​/Activities/{>int 32}
- URL: **{{url глобал}}{{вся активность глобал}}/{{>int 32}}**
- Ожидаемый результат: статус-код ответа **400**, тест провален
- Заголовки запроса: 
```javascript
{
    "content-type": "application/json",
    "user-agent": "PostmanRuntime/7.32.3",
    "accept": "*/*",
    "cache-control": "no-cache",
    "postman-token": "e2aefa1a-208c-4494-8d35-24bf048384d0",
    "host": "fakerestapi.azurewebsites.net",
    "accept-encoding": "gzip, deflate, br",
    "connection": "keep-alive"
}
```
- Тело запроса:
```javascript
{
  "id": 12345678911,
  "title": "string",
  "dueDate": "2023-06-22T08:32:29.719Z",
  "completed": true
}
```
- Заголовки ответа:
```javascript
 access-control-allow-origin: * 
 api-supported-versions: 1.0 
 content-type: application/json; charset=utf-8; v=1.0 
 date: Thu22 Jun 2023 14:17:08 GMT 
 server: Kestrel 
 transfer-encoding: chunked 
 ```
- Тело ответа: 
```javascript
{
    "type": "https://tools.ietf.org/html/rfc7231#section-6.5.1",
    "title": "One or more validation errors occurred.",
    "status": 400,
    "traceId": "00-1606999409074341b3e6afbf7459789b-0a6572b607bb1b40-00",
    "errors": {
        "id": [
            "The value '2147483648' is not valid."
        ],
        "$.id": [
            "The JSON value could not be converted to System.Int32. Path: $.id | LineNumber: 1 | BytePositionInLine: 19."
        ]
    }
}
```

## PUT/api​/v1​/Activities/{null}
- URL: **{{url глобал}}{{вся активность глобал}}/{{null}}**
- Ожидаемый результат: статус-код ответа **400**, тест провален
- Заголовки запроса: 
```javascript
{
    "content-type": "application/json",
    "user-agent": "PostmanRuntime/7.32.3",
    "accept": "*/*",
    "cache-control": "no-cache",
    "postman-token": "80faf737-5afa-4ea5-a449-0f6428e641fc",
    "host": "fakerestapi.azurewebsites.net",
    "accept-encoding": "gzip, deflate, br",
    "connection": "keep-alive"
  }
```
- Тело запроса:
```javascript
{
  "id": null,
  "title": "string",
  "dueDate": "2023-06-22T09:06:30.921Z",
  "completed": true
}
```
- Заголовки ответа:
```javascript
 access-control-allow-origin: * 
 api-supported-versions: 1.0 
 content-type: application/json; charset=utf-8; v=1.0 
 date: Thu22 Jun 2023 14:17:08 GMT 
 server: Kestrel 
 transfer-encoding: chunked 
 ```
- Тело ответа: 
```javascript
{
    "type": "https://tools.ietf.org/html/rfc7231#section-6.5.1",
    "title": "One or more validation errors occurred.",
    "status": 400,
    "traceId": "00-490ea5e29dde3540ac740c623a7e4d03-b831cc15d782c143-00",
    "errors": {
        "id": [
            "The value 'null' is not valid."
        ],
        "$.id": [
            "The JSON value could not be converted to System.Int32. Path: $.id | LineNumber: 1 | BytePositionInLine: 12."
        ]
    }
}
```

## PUT/api​/v1​/Activities/{empty line}
- URL: **{{url глобал}}{{вся активность глобал}}/{{empty line}}**
- Ожидаемый результат: статус-код ответа **400**, тест провален
- Заголовки запроса: 
```javascript
{
    "content-type": "application/json",
    "user-agent": "PostmanRuntime/7.32.3",
    "accept": "*/*",
    "cache-control": "no-cache",
    "postman-token": "80faf737-5afa-4ea5-a449-0f6428e641fc",
    "host": "fakerestapi.azurewebsites.net",
    "accept-encoding": "gzip, deflate, br",
    "connection": "keep-alive"
  }
```
- Тело запроса:
```javascript
{
  "id": 
  "title": "string",
  "dueDate": "2023-06-22T09:06:30.921Z",
  "completed": true
}
```
- Заголовки ответа:
```javascript
 access-control-allow-origin: * 
 api-supported-versions: 1.0 
 content-type: application/json; charset=utf-8; v=1.0 
 date: Thu22 Jun 2023 14:17:08 GMT 
 server: Kestrel 
 transfer-encoding: chunked 
 ```
- Тело ответа: 
```javascript
{
    "type": "https://tools.ietf.org/html/rfc7231#section-6.5.1",
    "title": "One or more validation errors occurred.",
    "status": 400,
    "traceId": "00-3aeed29acb6ce24389aaf78f1dfd2d49-92b62470ec55b64a-00",
    "errors": {
        "id": [
            "The value ' ' is invalid."
        ],
        "$.id": [
            "The JSON value could not be converted to System.Int32. Path: $.id | LineNumber: 2 | BytePositionInLine: 9."
        ]
    }
}
```

## PUT/api/v1/Authors/{0}
- URL: **{{url глобал}}{{авторы все глобал}}/{{0}}**
- Ожидаемый результат: статус-код ответа **200**, тест успешно пройден
- Заголовки запроса: 
```javascript
{
    "content-type": "application/json",
    "user-agent": "PostmanRuntime/7.32.3",
    "accept": "*/*",
    "cache-control": "no-cache",
    "postman-token": "80faf737-5afa-4ea5-a449-0f6428e641fc",
    "host": "fakerestapi.azurewebsites.net",
    "accept-encoding": "gzip, deflate, br",
    "connection": "keep-alive"
  }
```
- Тело запроса:
```javascript
{
  "id": 0,
  "idBook": 0,
  "firstName": "string",
  "lastName": "string"
}
```
- Заголовки ответа:
```javascript
  access-control-allow-origin: * 
 api-supported-versions: 1.0 
 content-type: application/json; charset=utf-8; v=1.0 
 date: Thu22 Jun 2023 14:50:21 GMT 
 server: Kestrel 
 transfer-encoding: chunked 
 ```
- Тело ответа: 
```javascript
{
    "id": 0,
    "idBook": 0,
    "firstName": "string",
    "lastName": "string"
}
```

## PUT/api/v1/Authors/{>int 32}
- URL: **{{url глобал}}{{авторы все глобал}}/{{>int 32}}**
- Ожидаемый результат: статус-код ответа **400**, тест не пройден
- Заголовки запроса: 
```javascript
{
    "content-type": "application/json",
    "user-agent": "PostmanRuntime/7.32.3",
    "accept": "*/*",
    "cache-control": "no-cache",
    "postman-token": "80faf737-5afa-4ea5-a449-0f6428e641fc",
    "host": "fakerestapi.azurewebsites.net",
    "accept-encoding": "gzip, deflate, br",
    "connection": "keep-alive"
  }
```
- Тело запроса:
```javascript
{
  "id": 12345678911,
  "idBook": 0,
  "firstName": "string",
  "lastName": "string"
}
```
- Заголовки ответа:
```javascript
 access-control-allow-origin: * 
 api-supported-versions: 1.0 
 content-type: application/json; charset=utf-8; v=1.0 
 date: Thu22 Jun 2023 14:50:21 GMT 
 server: Kestrel 
 transfer-encoding: chunked 
 ```
- Тело ответа: 
```javascript
{
    "type": "https://tools.ietf.org/html/rfc7231#section-6.5.1",
    "title": "One or more validation errors occurred.",
    "status": 400,
    "traceId": "00-c364337733d3b64d929e8d84762c9f39-3f7c154984bb7147-00",
    "errors": {
        "id": [
            "The value '2147483648' is not valid."
        ],
        "$.id": [
            "The JSON value could not be converted to System.Int32. Path: $.id | LineNumber: 1 | BytePositionInLine: 19."
        ]
    }
}
```

## PUT/api/v1/Authors/{null}
- URL: **{{url глобал}}{{авторы все глобал}}/{{null}}**
- Ожидаемый результат: статус-код ответа **400**, тест не пройден
- Заголовки запроса: 
```javascript
{
    "content-type": "application/json",
    "user-agent": "PostmanRuntime/7.32.3",
    "accept": "*/*",
    "cache-control": "no-cache",
    "postman-token": "80faf737-5afa-4ea5-a449-0f6428e641fc",
    "host": "fakerestapi.azurewebsites.net",
    "accept-encoding": "gzip, deflate, br",
    "connection": "keep-alive"
  }
```
- Тело запроса:
```javascript
{
  "id": null,
  "idBook": 0,
  "firstName": "string",
  "lastName": "string"
}
```
- Заголовки ответа:
```javascript
 access-control-allow-origin: * 
 api-supported-versions: 1.0 
 content-type: application/json; charset=utf-8; v=1.0 
 date: Thu22 Jun 2023 14:50:21 GMT 
 server: Kestrel 
 transfer-encoding: chunked 
 ```
- Тело ответа: 
```javascript
{
    "type": "https://tools.ietf.org/html/rfc7231#section-6.5.1",
    "title": "One or more validation errors occurred.",
    "status": 400,
    "traceId": "00-38e50ff5b9c5ba4fb84f7f945d807c14-a48cac6390a92a41-00",
    "errors": {
        "id": [
            "The value 'null' is not valid."
        ],
        "$.id": [
            "The JSON value could not be converted to System.Int32. Path: $.id | LineNumber: 1 | BytePositionInLine: 12."
        ]
    }
}
```


## PUT/api/v1/Authors/{empty line}
- URL: **{{url глобал}}{{авторы все глобал}}/{{empty line}}**
- Ожидаемый результат: статус-код ответа **400**, тест не пройден
- Заголовки запроса: 
```javascript
{
    "content-type": "application/json",
    "user-agent": "PostmanRuntime/7.32.3",
    "accept": "*/*",
    "cache-control": "no-cache",
    "postman-token": "80faf737-5afa-4ea5-a449-0f6428e641fc",
    "host": "fakerestapi.azurewebsites.net",
    "accept-encoding": "gzip, deflate, br",
    "connection": "keep-alive"
}
```
- Тело запроса:
```javascript
{
  "id":
  "idBook": 0,
  "firstName": "string",
  "lastName": "string"
}
```
- Заголовки ответа:
```javascript
  access-control-allow-origin: * 
 api-supported-versions: 1.0 
 content-type: application/json; charset=utf-8; v=1.0 
 date: Thu22 Jun 2023 14:50:21 GMT 
 server: Kestrel 
 transfer-encoding: chunked 
 ```
- Тело ответа: 
```javascript
{
    "type": "https://tools.ietf.org/html/rfc7231#section-6.5.1",
    "title": "One or more validation errors occurred.",
    "status": 400,
    "traceId": "00-71cec0c5677a3d46bbe63e7296b6933b-51abbbfa5bfe5d4f-00",
    "errors": {
        "id": [
            "The value ' ' is invalid."
        ],
        "$.id": [
            "The JSON value could not be converted to System.Int32. Path: $.id | LineNumber: 2 | BytePositionInLine: 10."
        ]
    }
}
```

## PUT/api/v1/Books/{0}
- URL: **{{url глобал}}{{книги все глобал}}/{{0}}**
- Ожидаемый результат: статус-код ответа **200**, тест успешно пройден
- Заголовки запроса: 
```javascript
{
    "content-type": "application/json",
    "user-agent": "PostmanRuntime/7.32.3",
    "accept": "*/*",
    "cache-control": "no-cache",
    "postman-token": "7eaf77e4-8833-43ea-8ddf-0aa88f1978b4",
    "host": "fakerestapi.azurewebsites.net",
    "accept-encoding": "gzip, deflate, br",
    "connection": "keep-alive"
}
```
- Тело запроса:
```javascript
{
  "id": 0,
  "title": "string",
  "description": "string",
  "pageCount": 0,
  "excerpt": "string",
  "publishDate": "2023-06-22T11:01:09.584Z"
}
```
- Заголовки ответа:
```javascript
 access-control-allow-origin: * 
 api-supported-versions: 1.0 
 content-type: application/json; charset=utf-8; v=1.0 
 date: Thu22 Jun 2023 14:59:02 GMT 
 server: Kestrel 
 transfer-encoding: chunked 
 ```
- Тело ответа: 
```javascript
{
    "id": 0,
    "title": "string",
    "description": "string",
    "pageCount": 0,
    "excerpt": "string",
    "publishDate": "2023-06-22T11:01:09.584Z"
}
```

## PUT/api/v1/Books/{>int 32}
- URL: **{{url глобал}}{{книги все глобал}}/{{>int 32}}**
- Ожидаемый результат: статус-код ответа **400**, тест не пройден
- Заголовки запроса: 
```javascript
{
    "content-type": "application/json",
    "user-agent": "PostmanRuntime/7.32.3",
    "accept": "*/*",
    "cache-control": "no-cache",
    "postman-token": "7eaf77e4-8833-43ea-8ddf-0aa88f1978b4",
    "host": "fakerestapi.azurewebsites.net",
    "accept-encoding": "gzip, deflate, br",
    "connection": "keep-alive"
}
```
- Тело запроса:
```javascript
{
  "id": 12345678911,
  "title": "string",
  "description": "string",
  "pageCount": 0,
  "excerpt": "string",
  "publishDate": "2023-06-22T11:01:09.584Z"
}
```
- Заголовки ответа:
```javascript
access-control-allow-origin: * 
 api-supported-versions: 1.0 
 content-type: application/json; charset=utf-8; v=1.0 
 date: Thu22 Jun 2023 15:08:10 GMT 
 server: Kestrel 
 transfer-encoding: chunked 
 ```
- Тело ответа: 
```javascript
{
    "type": "https://tools.ietf.org/html/rfc7231#section-6.5.1",
    "title": "One or more validation errors occurred.",
    "status": 400,
    "traceId": "00-aa8d42909bd9b543be275ea9ec24c03b-6cacf6dd3495f643-00",
    "errors": {
        "id": [
            "The value '2147483648' is not valid."
        ],
        "$.id": [
            "The JSON value could not be converted to System.Int32. Path: $.id | LineNumber: 1 | BytePositionInLine: 19."
        ]
    }
}
```

## PUT/api/v1/Books/{null}
- URL: **{{url глобал}}{{книги все глобал}}/{{null}}**
- Ожидаемый результат: статус-код ответа **400**, тест не пройден
- Заголовки запроса: 
```javascript
{
    "content-type": "application/json",
    "user-agent": "PostmanRuntime/7.32.3",
    "accept": "*/*",
    "cache-control": "no-cache",
    "postman-token": "7eaf77e4-8833-43ea-8ddf-0aa88f1978b4",
    "host": "fakerestapi.azurewebsites.net",
    "accept-encoding": "gzip, deflate, br",
    "connection": "keep-alive"
}
```
- Тело запроса:
```javascript
{
  "id": null,
  "title": "string",
  "description": "string",
  "pageCount": 0,
  "excerpt": "string",
  "publishDate": "2023-06-22T11:01:09.584Z"
}
```
- Заголовки ответа:
```javascript
access-control-allow-origin: * 
 api-supported-versions: 1.0 
 content-type: application/json; charset=utf-8; v=1.0 
 date: Thu22 Jun 2023 15:08:10 GMT 
 server: Kestrel 
 transfer-encoding: chunked 
 ```
- Тело ответа: 
```javascript
{
    "type": "https://tools.ietf.org/html/rfc7231#section-6.5.1",
    "title": "One or more validation errors occurred.",
    "status": 400,
    "traceId": "00-a8c4d2d250e16b4c8866e40f74b73617-52c54fcde46f4941-00",
    "errors": {
        "id": [
            "The value 'null' is not valid."
        ],
        "$.id": [
            "The JSON value could not be converted to System.Int32. Path: $.id | LineNumber: 1 | BytePositionInLine: 12."
        ]
    }
}
```

## PUT/api/v1/Books/{empty line}
- URL: **{{url глобал}}{{книги все глобал}}/{{empty line}}**
- Ожидаемый результат: статус-код ответа **400**, тест не пройден
- Заголовки запроса: 
```javascript
{
    "content-type": "application/json",
    "user-agent": "PostmanRuntime/7.32.3",
    "accept": "*/*",
    "cache-control": "no-cache",
    "postman-token": "7eaf77e4-8833-43ea-8ddf-0aa88f1978b4",
    "host": "fakerestapi.azurewebsites.net",
    "accept-encoding": "gzip, deflate, br",
    "connection": "keep-alive"
}
```
- Тело запроса:
```javascript
{
  "id":
  "title": "string",
  "description": "string",
  "pageCount": 0,
  "excerpt": "string",
  "publishDate": "2023-06-22T11:01:09.584Z"
}
```
- Заголовки ответа:
```javascript
access-control-allow-origin: * 
 api-supported-versions: 1.0 
 content-type: application/json; charset=utf-8; v=1.0 
 date: Thu22 Jun 2023 15:08:10 GMT 
 server: Kestrel 
 transfer-encoding: chunked 
 ```
- Тело ответа: 
```javascript
{
    "type": "https://tools.ietf.org/html/rfc7231#section-6.5.1",
    "title": "One or more validation errors occurred.",
    "status": 400,
    "traceId": "00-945be9b6aa68744a9a307ff20889a3e5-72b6bf237e679041-00",
    "errors": {
        "id": [
            "The value ' ' is invalid."
        ],
        "$.id": [
            "The JSON value could not be converted to System.Int32. Path: $.id | LineNumber: 2 | BytePositionInLine: 9."
        ]
    }
}
```

## PUT/api/v1/CoverPhotos/{0}
- URL: **{{url глобал}}{{фото все глобал}}/{{0}}**
- Ожидаемый результат: статус-код ответа **200**, тест успешно пройден
- Заголовки запроса: 
```javascript
{
    "content-type": "application/json",
    "user-agent": "PostmanRuntime/7.32.3",
    "accept": "*/*",
    "cache-control": "no-cache",
    "postman-token": "bfc514de-ee2e-4d0c-9906-3b48edee9e0d",
    "host": "fakerestapi.azurewebsites.net",
    "accept-encoding": "gzip, deflate, br",
    "connection": "keep-alive"
  }
```
- Тело запроса:
```javascript
{
  "id": 0,
  "idBook": 0,
  "url": "string"
}
```
- Заголовки ответа:
```javascript
 access-control-allow-origin: * 
 api-supported-versions: 1.0 
 content-type: application/json; charset=utf-8; v=1.0 
 date: Thu22 Jun 2023 15:17:38 GMT 
 server: Kestrel 
 transfer-encoding: chunked 
 ```
- Тело ответа: 
```javascript
{
    "id": 0,
    "idBook": 0,
    "url": "string"
}
```


## PUT/api/v1/CoverPhotos/{>int 32}
- URL: **{{url глобал}}{{фото все глобал}}/{{>int 32}}**
- Ожидаемый результат: статус-код ответа **400**, тест не пройден
- Заголовки запроса: 
```javascript
{
    "content-type": "application/json",
    "user-agent": "PostmanRuntime/7.32.3",
    "accept": "*/*",
    "cache-control": "no-cache",
    "postman-token": "bfc514de-ee2e-4d0c-9906-3b48edee9e0d",
    "host": "fakerestapi.azurewebsites.net",
    "accept-encoding": "gzip, deflate, br",
    "connection": "keep-alive"
  }
```
- Тело запроса:
```javascript
{
  "id": 12345678911,
  "idBook": 0,
  "url": "string"
}
```
- Заголовки ответа:
```javascript
 access-control-allow-origin: * 
 api-supported-versions: 1.0 
 content-type: application/json; charset=utf-8; v=1.0 
 date: Thu22 Jun 2023 15:17:38 GMT 
 server: Kestrel 
 transfer-encoding: chunked 
 ```
- Тело ответа: 
```javascript
{
    "type": "https://tools.ietf.org/html/rfc7231#section-6.5.1",
    "title": "One or more validation errors occurred.",
    "status": 400,
    "traceId": "00-c3c3ee5da3bdc143b1ef67aa49282c04-57ade41fef26d646-00",
    "errors": {
        "id": [
            "The value '2147483648' is not valid."
        ],
        "$.id": [
            "The JSON value could not be converted to System.Int32. Path: $.id | LineNumber: 1 | BytePositionInLine: 19."
        ]
    }
}
```

## PUT/api/v1/CoverPhotos/{null}
- URL: **{{url глобал}}{{фото все глобал}}/{{null}}**
- Ожидаемый результат: статус-код ответа **400**, тест не пройден
- Заголовки запроса: 
```javascript
{
    "content-type": "application/json",
    "user-agent": "PostmanRuntime/7.32.3",
    "accept": "*/*",
    "cache-control": "no-cache",
    "postman-token": "bfc514de-ee2e-4d0c-9906-3b48edee9e0d",
    "host": "fakerestapi.azurewebsites.net",
    "accept-encoding": "gzip, deflate, br",
    "connection": "keep-alive"
  }
```
- Тело запроса:
```javascript
{
  "id": null,
  "idBook": 0,
  "url": "string"
}
```
- Заголовки ответа:
```javascript
 access-control-allow-origin: * 
 api-supported-versions: 1.0 
 content-type: application/json; charset=utf-8; v=1.0 
 date: Thu22 Jun 2023 15:17:38 GMT 
 server: Kestrel 
 transfer-encoding: chunked 
 ```
- Тело ответа: 
```javascript
{
    "type": "https://tools.ietf.org/html/rfc7231#section-6.5.1",
    "title": "One or more validation errors occurred.",
    "status": 400,
    "traceId": "00-9f1b5e3f4fb223468b0d6da9e2654563-2fc899ee04b95642-00",
    "errors": {
        "id": [
            "The value 'null' is not valid."
        ],
        "$.id": [
            "The JSON value could not be converted to System.Int32. Path: $.id | LineNumber: 1 | BytePositionInLine: 12."
        ]
    }
}
```

## PUT/api/v1/CoverPhotos/{empty line}
- URL: **{{url глобал}}{{фото все глобал}}/{{empty line}}**
- Ожидаемый результат: статус-код ответа **400**, тест не пройден
- Заголовки запроса: 
```javascript
{
    "content-type": "application/json",
    "user-agent": "PostmanRuntime/7.32.3",
    "accept": "*/*",
    "cache-control": "no-cache",
    "postman-token": "bfc514de-ee2e-4d0c-9906-3b48edee9e0d",
    "host": "fakerestapi.azurewebsites.net",
    "accept-encoding": "gzip, deflate, br",
    "connection": "keep-alive"
  }
```
- Тело запроса:
```javascript
{
  "id":
  "idBook": 0,
  "url": "string"
}
```
- Заголовки ответа:
```javascript
 access-control-allow-origin: * 
 api-supported-versions: 1.0 
 content-type: application/json; charset=utf-8; v=1.0 
 date: Thu22 Jun 2023 15:17:38 GMT 
 server: Kestrel 
 transfer-encoding: chunked 
 ```
- Тело ответа: 
```javascript
{
    "type": "https://tools.ietf.org/html/rfc7231#section-6.5.1",
    "title": "One or more validation errors occurred.",
    "status": 400,
    "traceId": "00-e5685e87bb7459439b3df90080df4cb9-2d07bc4aae37a44a-00",
    "errors": {
        "id": [
            "The value ' ' is invalid."
        ],
        "$.id": [
            "The JSON value could not be converted to System.Int32. Path: $.id | LineNumber: 2 | BytePositionInLine: 10."
        ]
    }
}
```

## PUT/api/v1/Users/{0}
- URL: **{{url глобал}}{{юзеры все глобал}}/{{0}}**
- Ожидаемый результат: статус-код ответа **200**, тест успешно пройден
- Заголовки запроса: 
```javascript
{
    "content-type": "application/json",
    "user-agent": "PostmanRuntime/7.32.3",
    "accept": "*/*",
    "cache-control": "no-cache",
    "postman-token": "4c8d065c-c177-42b9-bf0d-d3f7546143f3",
    "host": "fakerestapi.azurewebsites.net",
    "accept-encoding": "gzip, deflate, br",
    "connection": "keep-alive"
  }
```
- Тело запроса:
```javascript
{
  "id": 0,
  "userName": "string",
  "password": "string"
}
```
- Заголовки ответа:
```javascript
  access-control-allow-origin: * 
 api-supported-versions: 1.0 
 content-type: application/json; charset=utf-8; v=1.0 
 date: Thu22 Jun 2023 15:28:57 GMT 
 server: Kestrel 
 transfer-encoding: chunked 
 ```
- Тело ответа: 
```javascript
{
    "id": 0,
    "userName": "string",
    "password": "string"
}
```

## PUT/api/v1/Users/{>int 32}
- URL: **{{url глобал}}{{юзеры все глобал}}/{{>int 32}}**
- Ожидаемый результат: статус-код ответа **400**, тест не пройден
- Заголовки запроса: 
```javascript
{
    "content-type": "application/json",
    "user-agent": "PostmanRuntime/7.32.3",
    "accept": "*/*",
    "cache-control": "no-cache",
    "postman-token": "4c8d065c-c177-42b9-bf0d-d3f7546143f3",
    "host": "fakerestapi.azurewebsites.net",
    "accept-encoding": "gzip, deflate, br",
    "connection": "keep-alive"
  }
```
- Тело запроса:
```javascript
{
  "id": 12345678911,
  "userName": "string",
  "password": "string"
}
```
- Заголовки ответа:
```javascript
  access-control-allow-origin: * 
 api-supported-versions: 1.0 
 content-type: application/json; charset=utf-8; v=1.0 
 date: Thu22 Jun 2023 15:28:57 GMT 
 server: Kestrel 
 transfer-encoding: chunked 
 ```
- Тело ответа: 
```javascript
{
    "type": "https://tools.ietf.org/html/rfc7231#section-6.5.1",
    "title": "One or more validation errors occurred.",
    "status": 400,
    "traceId": "00-ce697945ab872343bb8e196962e1982a-1a6d9a2419005444-00",
    "errors": {
        "id": [
            "The value '2147483648' is not valid."
        ],
        "$.id": [
            "The JSON value could not be converted to System.Int32. Path: $.id | LineNumber: 1 | BytePositionInLine: 19."
        ]
    }
}
```

## PUT/api/v1/Users/{null}
- URL: **{{url глобал}}{{юзеры все глобал}}/{{null}}**
- Ожидаемый результат: статус-код ответа **400**, тест не пройден
- Заголовки запроса: 
```javascript
{
    "content-type": "application/json",
    "user-agent": "PostmanRuntime/7.32.3",
    "accept": "*/*",
    "cache-control": "no-cache",
    "postman-token": "4c8d065c-c177-42b9-bf0d-d3f7546143f3",
    "host": "fakerestapi.azurewebsites.net",
    "accept-encoding": "gzip, deflate, br",
    "connection": "keep-alive"
  }
```
- Тело запроса:
```javascript
{
  "id": null,
  "userName": "string",
  "password": "string"
}
```
- Заголовки ответа:
```javascript
  access-control-allow-origin: * 
 api-supported-versions: 1.0 
 content-type: application/json; charset=utf-8; v=1.0 
 date: Thu22 Jun 2023 15:28:57 GMT 
 server: Kestrel 
 transfer-encoding: chunked 
 ```
- Тело ответа: 
```javascript
{
    "type": "https://tools.ietf.org/html/rfc7231#section-6.5.1",
    "title": "One or more validation errors occurred.",
    "status": 400,
    "traceId": "00-5181ab20cfb98f4ab5c47f640fa6a4b9-992cb640f84a5744-00",
    "errors": {
        "id": [
            "The value 'null' is not valid."
        ],
        "$.id": [
            "The JSON value could not be converted to System.Int32. Path: $.id | LineNumber: 1 | BytePositionInLine: 12."
        ]
    }
}
```


## PUT/api/v1/Users/{empty line}
- URL: **{{url глобал}}{{юзеры все глобал}}/{{empty line}}**
- Ожидаемый результат: статус-код ответа **400**, тест не пройден
- Заголовки запроса: 
```javascript
{
    "content-type": "application/json",
    "user-agent": "PostmanRuntime/7.32.3",
    "accept": "*/*",
    "cache-control": "no-cache",
    "postman-token": "4c8d065c-c177-42b9-bf0d-d3f7546143f3",
    "host": "fakerestapi.azurewebsites.net",
    "accept-encoding": "gzip, deflate, br",
    "connection": "keep-alive"
  }
```
- Тело запроса:
```javascript
{
  "id":
  "userName": "string",
  "password": "string"
}
```
- Заголовки ответа:
```javascript
  access-control-allow-origin: * 
 api-supported-versions: 1.0 
 content-type: application/json; charset=utf-8; v=1.0 
 date: Thu22 Jun 2023 15:28:57 GMT 
 server: Kestrel 
 transfer-encoding: chunked 
 ```
- Тело ответа: 
```javascript
{
    "type": "https://tools.ietf.org/html/rfc7231#section-6.5.1",
    "title": "One or more validation errors occurred.",
    "status": 400,
    "traceId": "00-8de75999224efd468b4e60fe853b9c9d-f7b612b489d48241-00",
    "errors": {
        "id": [
            "The value ' ' is invalid."
        ],
        "$.id": [
            "The JSON value could not be converted to System.Int32. Path: $.id | LineNumber: 2 | BytePositionInLine: 12."
        ]
    }
}
```
## POST/api/v1/Activities/{0}
- URL: **{{url глобал}}{{вся активность глобал}}**
- Ожидаемый результат: статус-код ответа **200**, тест успешно пройден
- Заголовки запроса: 
```javascript
Content-Type: "application/json"
User-Agent: "PostmanRuntime/7.32.3"
Accept: "*/*"
Cache-Control: "no-cache"
Postman-Token: "d0db613d-59ed-4d10-a94c-5db233426daa"
Host: "fakerestapi.azurewebsites.net"
Accept-Encoding: "gzip, deflate, br"
Connection: "keep-alive"
```
- Тело запроса:
```javascript
{
"id": 0, 
"title": "string",
"dueDate": "2023-06-22T08:32:29.719Z", 
"completed": true 
}
```
- Заголовки ответа:
```javascript
 access-control-allow-origin: * 
 api-supported-versions: 1.0 
 content-type: application/json; charset=utf-8; v=1.0 
 date: Thu22 Jun 2023 14:17:08 GMT 
 server: Kestrel 
 transfer-encoding: chunked 
 ```
- Тело ответа: 
```javascript
{
  "id": 0,
  "title": "string",
  "dueDate": "2023-06-22T14:17:09.044Z",
  "completed": true
}
```

## POST/api​/v1​/Activities/{>int 32}
- URL: **{{url глобал}}{{вся активность глобал}}**
- Ожидаемый результат: статус-код ответа **400**, тест провален
- Заголовки запроса: 
```javascript
{
    "content-type": "application/json",
    "user-agent": "PostmanRuntime/7.32.3",
    "accept": "*/*",
    "cache-control": "no-cache",
    "postman-token": "e2aefa1a-208c-4494-8d35-24bf048384d0",
    "host": "fakerestapi.azurewebsites.net",
    "accept-encoding": "gzip, deflate, br",
    "connection": "keep-alive"
}
```
- Тело запроса:
```javascript
{
  "id": 12345678911,
  "title": "string",
  "dueDate": "2023-06-22T08:32:29.719Z",
  "completed": true
}
```
- Заголовки ответа:
```javascript
 access-control-allow-origin: * 
 api-supported-versions: 1.0 
 content-type: application/json; charset=utf-8; v=1.0 
 date: Thu22 Jun 2023 14:17:08 GMT 
 server: Kestrel 
 transfer-encoding: chunked 
 ```
- Тело ответа: 
```javascript
{
    "type": "https://tools.ietf.org/html/rfc7231#section-6.5.1",
    "title": "One or more validation errors occurred.",
    "status": 400,
    "traceId": "00-1606999409074341b3e6afbf7459789b-0a6572b607bb1b40-00",
    "errors": {
        "id": [
            "The value '2147483648' is not valid."
        ],
        "$.id": [
            "The JSON value could not be converted to System.Int32. Path: $.id | LineNumber: 1 | BytePositionInLine: 19."
        ]
    }
}
```

## POST/api​/v1​/Activities/{null}
- URL: **{{url глобал}}{{вся активность глобал}}**
- Ожидаемый результат: статус-код ответа **400**, тест провален
- Заголовки запроса: 
```javascript
{
    "content-type": "application/json",
    "user-agent": "PostmanRuntime/7.32.3",
    "accept": "*/*",
    "cache-control": "no-cache",
    "postman-token": "80faf737-5afa-4ea5-a449-0f6428e641fc",
    "host": "fakerestapi.azurewebsites.net",
    "accept-encoding": "gzip, deflate, br",
    "connection": "keep-alive"
  }
```
- Тело запроса:
```javascript
{
  "id": null,
  "title": "string",
  "dueDate": "2023-06-22T09:06:30.921Z",
  "completed": true
}
```
- Заголовки ответа:
```javascript
 access-control-allow-origin: * 
 api-supported-versions: 1.0 
 content-type: application/json; charset=utf-8; v=1.0 
 date: Thu22 Jun 2023 14:17:08 GMT 
 server: Kestrel 
 transfer-encoding: chunked 
 ```
- Тело ответа: 
```javascript
{
    "type": "https://tools.ietf.org/html/rfc7231#section-6.5.1",
    "title": "One or more validation errors occurred.",
    "status": 400,
    "traceId": "00-490ea5e29dde3540ac740c623a7e4d03-b831cc15d782c143-00",
    "errors": {
        "id": [
            "The value 'null' is not valid."
        ],
        "$.id": [
            "The JSON value could not be converted to System.Int32. Path: $.id | LineNumber: 1 | BytePositionInLine: 12."
        ]
    }
}
```

## POST/api​/v1​/Activities/{empty line}
- URL: **{{url глобал}}{{вся активность глобал}}**
- Ожидаемый результат: статус-код ответа **400**, тест провален
- Заголовки запроса: 
```javascript
{
    "content-type": "application/json",
    "user-agent": "PostmanRuntime/7.32.3",
    "accept": "*/*",
    "cache-control": "no-cache",
    "postman-token": "80faf737-5afa-4ea5-a449-0f6428e641fc",
    "host": "fakerestapi.azurewebsites.net",
    "accept-encoding": "gzip, deflate, br",
    "connection": "keep-alive"
  }
```
- Тело запроса:
```javascript
{
  "id": 
  "title": "string",
  "dueDate": "2023-06-22T09:06:30.921Z",
  "completed": true
}
```
- Заголовки ответа:
```javascript
 access-control-allow-origin: * 
 api-supported-versions: 1.0 
 content-type: application/json; charset=utf-8; v=1.0 
 date: Thu22 Jun 2023 14:17:08 GMT 
 server: Kestrel 
 transfer-encoding: chunked 
 ```
- Тело ответа: 
```javascript
{
    "type": "https://tools.ietf.org/html/rfc7231#section-6.5.1",
    "title": "One or more validation errors occurred.",
    "status": 400,
    "traceId": "00-3aeed29acb6ce24389aaf78f1dfd2d49-92b62470ec55b64a-00",
    "errors": {
        "id": [
            "The value ' ' is invalid."
        ],
        "$.id": [
            "The JSON value could not be converted to System.Int32. Path: $.id | LineNumber: 2 | BytePositionInLine: 9."
        ]
    }
}
```

## POST/api/v1/Authors/{0}
- URL: **{{url глобал}}{{авторы все глобал}}**
- Ожидаемый результат: статус-код ответа **200**, тест успешно пройден
- Заголовки запроса: 
```javascript
{
    "content-type": "application/json",
    "user-agent": "PostmanRuntime/7.32.3",
    "accept": "*/*",
    "cache-control": "no-cache",
    "postman-token": "80faf737-5afa-4ea5-a449-0f6428e641fc",
    "host": "fakerestapi.azurewebsites.net",
    "accept-encoding": "gzip, deflate, br",
    "connection": "keep-alive"
  }
```
- Тело запроса:
```javascript
{
  "id": 0,
  "idBook": 0,
  "firstName": "string",
  "lastName": "string"
}
```
- Заголовки ответа:
```javascript
  access-control-allow-origin: * 
 api-supported-versions: 1.0 
 content-type: application/json; charset=utf-8; v=1.0 
 date: Thu22 Jun 2023 14:50:21 GMT 
 server: Kestrel 
 transfer-encoding: chunked 
 ```
- Тело ответа: 
```javascript
{
    "id": 0,
    "idBook": 0,
    "firstName": "string",
    "lastName": "string"
}
```

## POST/api/v1/Authors/{>int 32}
- URL: **{{url глобал}}{{авторы все глобал}}**
- Ожидаемый результат: статус-код ответа **400**, тест не пройден
- Заголовки запроса: 
```javascript
{
    "content-type": "application/json",
    "user-agent": "PostmanRuntime/7.32.3",
    "accept": "*/*",
    "cache-control": "no-cache",
    "postman-token": "80faf737-5afa-4ea5-a449-0f6428e641fc",
    "host": "fakerestapi.azurewebsites.net",
    "accept-encoding": "gzip, deflate, br",
    "connection": "keep-alive"
  }
```
- Тело запроса:
```javascript
{
  "id": 12345678911,
  "idBook": 0,
  "firstName": "string",
  "lastName": "string"
}
```
- Заголовки ответа:
```javascript
 access-control-allow-origin: * 
 api-supported-versions: 1.0 
 content-type: application/json; charset=utf-8; v=1.0 
 date: Thu22 Jun 2023 14:50:21 GMT 
 server: Kestrel 
 transfer-encoding: chunked 
 ```
- Тело ответа: 
```javascript
{
    "type": "https://tools.ietf.org/html/rfc7231#section-6.5.1",
    "title": "One or more validation errors occurred.",
    "status": 400,
    "traceId": "00-c364337733d3b64d929e8d84762c9f39-3f7c154984bb7147-00",
    "errors": {
        "id": [
            "The value '2147483648' is not valid."
        ],
        "$.id": [
            "The JSON value could not be converted to System.Int32. Path: $.id | LineNumber: 1 | BytePositionInLine: 19."
        ]
    }
}
```

## POST/api/v1/Authors/{null}
- URL: **{{url глобал}}{{авторы все глобал}}**
- Ожидаемый результат: статус-код ответа **400**, тест не пройден
- Заголовки запроса: 
```javascript
{
    "content-type": "application/json",
    "user-agent": "PostmanRuntime/7.32.3",
    "accept": "*/*",
    "cache-control": "no-cache",
    "postman-token": "80faf737-5afa-4ea5-a449-0f6428e641fc",
    "host": "fakerestapi.azurewebsites.net",
    "accept-encoding": "gzip, deflate, br",
    "connection": "keep-alive"
  }
```
- Тело запроса:
```javascript
{
  "id": null,
  "idBook": 0,
  "firstName": "string",
  "lastName": "string"
}
```
- Заголовки ответа:
```javascript
 access-control-allow-origin: * 
 api-supported-versions: 1.0 
 content-type: application/json; charset=utf-8; v=1.0 
 date: Thu22 Jun 2023 14:50:21 GMT 
 server: Kestrel 
 transfer-encoding: chunked 
 ```
- Тело ответа: 
```javascript
{
    "type": "https://tools.ietf.org/html/rfc7231#section-6.5.1",
    "title": "One or more validation errors occurred.",
    "status": 400,
    "traceId": "00-38e50ff5b9c5ba4fb84f7f945d807c14-a48cac6390a92a41-00",
    "errors": {
        "id": [
            "The value 'null' is not valid."
        ],
        "$.id": [
            "The JSON value could not be converted to System.Int32. Path: $.id | LineNumber: 1 | BytePositionInLine: 12."
        ]
    }
}
```


## POST/api/v1/Authors/{empty line}
- URL: **{{url глобал}}{{авторы все глобал}}**
- Ожидаемый результат: статус-код ответа **400**, тест не пройден
- Заголовки запроса: 
```javascript
{
    "content-type": "application/json",
    "user-agent": "PostmanRuntime/7.32.3",
    "accept": "*/*",
    "cache-control": "no-cache",
    "postman-token": "80faf737-5afa-4ea5-a449-0f6428e641fc",
    "host": "fakerestapi.azurewebsites.net",
    "accept-encoding": "gzip, deflate, br",
    "connection": "keep-alive"
}
```
- Тело запроса:
```javascript
{
  "id":
  "idBook": 0,
  "firstName": "string",
  "lastName": "string"
}
```
- Заголовки ответа:
```javascript
  access-control-allow-origin: * 
 api-supported-versions: 1.0 
 content-type: application/json; charset=utf-8; v=1.0 
 date: Thu22 Jun 2023 14:50:21 GMT 
 server: Kestrel 
 transfer-encoding: chunked 
 ```
- Тело ответа: 
```javascript
{
    "type": "https://tools.ietf.org/html/rfc7231#section-6.5.1",
    "title": "One or more validation errors occurred.",
    "status": 400,
    "traceId": "00-71cec0c5677a3d46bbe63e7296b6933b-51abbbfa5bfe5d4f-00",
    "errors": {
        "id": [
            "The value ' ' is invalid."
        ],
        "$.id": [
            "The JSON value could not be converted to System.Int32. Path: $.id | LineNumber: 2 | BytePositionInLine: 10."
        ]
    }
}
```

## POST/api/v1/Books/{0}
- URL: **{{url глобал}}{{книги все глобал}}**
- Ожидаемый результат: статус-код ответа **200**, тест успешно пройден
- Заголовки запроса: 
```javascript
{
    "content-type": "application/json",
    "user-agent": "PostmanRuntime/7.32.3",
    "accept": "*/*",
    "cache-control": "no-cache",
    "postman-token": "7eaf77e4-8833-43ea-8ddf-0aa88f1978b4",
    "host": "fakerestapi.azurewebsites.net",
    "accept-encoding": "gzip, deflate, br",
    "connection": "keep-alive"
}
```
- Тело запроса:
```javascript
{
  "id": 0,
  "title": "string",
  "description": "string",
  "pageCount": 0,
  "excerpt": "string",
  "publishDate": "2023-06-22T11:01:09.584Z"
}
```
- Заголовки ответа:
```javascript
 access-control-allow-origin: * 
 api-supported-versions: 1.0 
 content-type: application/json; charset=utf-8; v=1.0 
 date: Thu22 Jun 2023 14:59:02 GMT 
 server: Kestrel 
 transfer-encoding: chunked 
 ```
- Тело ответа: 
```javascript
{
    "id": 0,
    "title": "string",
    "description": "string",
    "pageCount": 0,
    "excerpt": "string",
    "publishDate": "2023-06-22T11:01:09.584Z"
}
```

## POST/api/v1/Books/{>int 32}
- URL: **{{url глобал}}{{книги все глобал}}**
- Ожидаемый результат: статус-код ответа **400**, тест не пройден
- Заголовки запроса: 
```javascript
{
    "content-type": "application/json",
    "user-agent": "PostmanRuntime/7.32.3",
    "accept": "*/*",
    "cache-control": "no-cache",
    "postman-token": "7eaf77e4-8833-43ea-8ddf-0aa88f1978b4",
    "host": "fakerestapi.azurewebsites.net",
    "accept-encoding": "gzip, deflate, br",
    "connection": "keep-alive"
}
```
- Тело запроса:
```javascript
{
  "id": 12345678911,
  "title": "string",
  "description": "string",
  "pageCount": 0,
  "excerpt": "string",
  "publishDate": "2023-06-22T11:01:09.584Z"
}
```
- Заголовки ответа:
```javascript
access-control-allow-origin: * 
 api-supported-versions: 1.0 
 content-type: application/json; charset=utf-8; v=1.0 
 date: Thu22 Jun 2023 15:08:10 GMT 
 server: Kestrel 
 transfer-encoding: chunked 
 ```
- Тело ответа: 
```javascript
{
    "type": "https://tools.ietf.org/html/rfc7231#section-6.5.1",
    "title": "One or more validation errors occurred.",
    "status": 400,
    "traceId": "00-aa8d42909bd9b543be275ea9ec24c03b-6cacf6dd3495f643-00",
    "errors": {
        "id": [
            "The value '2147483648' is not valid."
        ],
        "$.id": [
            "The JSON value could not be converted to System.Int32. Path: $.id | LineNumber: 1 | BytePositionInLine: 19."
        ]
    }
}
```

## POST/api/v1/Books/{null}
- URL: **{{url глобал}}{{книги все глобал}}**
- Ожидаемый результат: статус-код ответа **400**, тест не пройден
- Заголовки запроса: 
```javascript
{
    "content-type": "application/json",
    "user-agent": "PostmanRuntime/7.32.3",
    "accept": "*/*",
    "cache-control": "no-cache",
    "postman-token": "7eaf77e4-8833-43ea-8ddf-0aa88f1978b4",
    "host": "fakerestapi.azurewebsites.net",
    "accept-encoding": "gzip, deflate, br",
    "connection": "keep-alive"
}
```
- Тело запроса:
```javascript
{
  "id": null,
  "title": "string",
  "description": "string",
  "pageCount": 0,
  "excerpt": "string",
  "publishDate": "2023-06-22T11:01:09.584Z"
}
```
- Заголовки ответа:
```javascript
access-control-allow-origin: * 
 api-supported-versions: 1.0 
 content-type: application/json; charset=utf-8; v=1.0 
 date: Thu22 Jun 2023 15:08:10 GMT 
 server: Kestrel 
 transfer-encoding: chunked 
 ```
- Тело ответа: 
```javascript
{
    "type": "https://tools.ietf.org/html/rfc7231#section-6.5.1",
    "title": "One or more validation errors occurred.",
    "status": 400,
    "traceId": "00-a8c4d2d250e16b4c8866e40f74b73617-52c54fcde46f4941-00",
    "errors": {
        "id": [
            "The value 'null' is not valid."
        ],
        "$.id": [
            "The JSON value could not be converted to System.Int32. Path: $.id | LineNumber: 1 | BytePositionInLine: 12."
        ]
    }
}
```

## POST/api/v1/Books/{empty line}
- URL: **{{url глобал}}{{книги все глобал}}**
- Ожидаемый результат: статус-код ответа **400**, тест не пройден
- Заголовки запроса: 
```javascript
{
    "content-type": "application/json",
    "user-agent": "PostmanRuntime/7.32.3",
    "accept": "*/*",
    "cache-control": "no-cache",
    "postman-token": "7eaf77e4-8833-43ea-8ddf-0aa88f1978b4",
    "host": "fakerestapi.azurewebsites.net",
    "accept-encoding": "gzip, deflate, br",
    "connection": "keep-alive"
}
```
- Тело запроса:
```javascript
{
  "id":
  "title": "string",
  "description": "string",
  "pageCount": 0,
  "excerpt": "string",
  "publishDate": "2023-06-22T11:01:09.584Z"
}
```
- Заголовки ответа:
```javascript
access-control-allow-origin: * 
 api-supported-versions: 1.0 
 content-type: application/json; charset=utf-8; v=1.0 
 date: Thu22 Jun 2023 15:08:10 GMT 
 server: Kestrel 
 transfer-encoding: chunked 
 ```
- Тело ответа: 
```javascript
{
    "type": "https://tools.ietf.org/html/rfc7231#section-6.5.1",
    "title": "One or more validation errors occurred.",
    "status": 400,
    "traceId": "00-945be9b6aa68744a9a307ff20889a3e5-72b6bf237e679041-00",
    "errors": {
        "id": [
            "The value ' ' is invalid."
        ],
        "$.id": [
            "The JSON value could not be converted to System.Int32. Path: $.id | LineNumber: 2 | BytePositionInLine: 9."
        ]
    }
}
```

## POST/api/v1/CoverPhotos/{0}
- URL: **{{url глобал}}{{фото все глобал}}**
- Ожидаемый результат: статус-код ответа **200**, тест успешно пройден
- Заголовки запроса: 
```javascript
{
    "content-type": "application/json",
    "user-agent": "PostmanRuntime/7.32.3",
    "accept": "*/*",
    "cache-control": "no-cache",
    "postman-token": "bfc514de-ee2e-4d0c-9906-3b48edee9e0d",
    "host": "fakerestapi.azurewebsites.net",
    "accept-encoding": "gzip, deflate, br",
    "connection": "keep-alive"
  }
```
- Тело запроса:
```javascript
{
  "id": 0,
  "idBook": 0,
  "url": "string"
}
```
- Заголовки ответа:
```javascript
 access-control-allow-origin: * 
 api-supported-versions: 1.0 
 content-type: application/json; charset=utf-8; v=1.0 
 date: Thu22 Jun 2023 15:17:38 GMT 
 server: Kestrel 
 transfer-encoding: chunked 
 ```
- Тело ответа: 
```javascript
{
    "id": 0,
    "idBook": 0,
    "url": "string"
}
```


## POST/api/v1/CoverPhotos/{>int 32}
- URL: **{{url глобал}}{{фото все глобал}}**
- Ожидаемый результат: статус-код ответа **400**, тест не пройден
- Заголовки запроса: 
```javascript
{
    "content-type": "application/json",
    "user-agent": "PostmanRuntime/7.32.3",
    "accept": "*/*",
    "cache-control": "no-cache",
    "postman-token": "bfc514de-ee2e-4d0c-9906-3b48edee9e0d",
    "host": "fakerestapi.azurewebsites.net",
    "accept-encoding": "gzip, deflate, br",
    "connection": "keep-alive"
  }
```
- Тело запроса:
```javascript
{
  "id": 12345678911,
  "idBook": 0,
  "url": "string"
}
```
- Заголовки ответа:
```javascript
 access-control-allow-origin: * 
 api-supported-versions: 1.0 
 content-type: application/json; charset=utf-8; v=1.0 
 date: Thu22 Jun 2023 15:17:38 GMT 
 server: Kestrel 
 transfer-encoding: chunked 
 ```
- Тело ответа: 
```javascript
{
    "type": "https://tools.ietf.org/html/rfc7231#section-6.5.1",
    "title": "One or more validation errors occurred.",
    "status": 400,
    "traceId": "00-c3c3ee5da3bdc143b1ef67aa49282c04-57ade41fef26d646-00",
    "errors": {
        "id": [
            "The value '2147483648' is not valid."
        ],
        "$.id": [
            "The JSON value could not be converted to System.Int32. Path: $.id | LineNumber: 1 | BytePositionInLine: 19."
        ]
    }
}
```

## POST/api/v1/CoverPhotos/{null}
- URL: **{{url глобал}}{{фото все глобал}}**
- Ожидаемый результат: статус-код ответа **400**, тест не пройден
- Заголовки запроса: 
```javascript
{
    "content-type": "application/json",
    "user-agent": "PostmanRuntime/7.32.3",
    "accept": "*/*",
    "cache-control": "no-cache",
    "postman-token": "bfc514de-ee2e-4d0c-9906-3b48edee9e0d",
    "host": "fakerestapi.azurewebsites.net",
    "accept-encoding": "gzip, deflate, br",
    "connection": "keep-alive"
  }
```
- Тело запроса:
```javascript
{
  "id": null,
  "idBook": 0,
  "url": "string"
}
```
- Заголовки ответа:
```javascript
 access-control-allow-origin: * 
 api-supported-versions: 1.0 
 content-type: application/json; charset=utf-8; v=1.0 
 date: Thu22 Jun 2023 15:17:38 GMT 
 server: Kestrel 
 transfer-encoding: chunked 
 ```
- Тело ответа: 
```javascript
{
    "type": "https://tools.ietf.org/html/rfc7231#section-6.5.1",
    "title": "One or more validation errors occurred.",
    "status": 400,
    "traceId": "00-9f1b5e3f4fb223468b0d6da9e2654563-2fc899ee04b95642-00",
    "errors": {
        "id": [
            "The value 'null' is not valid."
        ],
        "$.id": [
            "The JSON value could not be converted to System.Int32. Path: $.id | LineNumber: 1 | BytePositionInLine: 12."
        ]
    }
}
```

## POST/api/v1/CoverPhotos/{empty line}
- URL: **{{url глобал}}{{фото все глобал}}**
- Ожидаемый результат: статус-код ответа **400**, тест не пройден
- Заголовки запроса: 
```javascript
{
    "content-type": "application/json",
    "user-agent": "PostmanRuntime/7.32.3",
    "accept": "*/*",
    "cache-control": "no-cache",
    "postman-token": "bfc514de-ee2e-4d0c-9906-3b48edee9e0d",
    "host": "fakerestapi.azurewebsites.net",
    "accept-encoding": "gzip, deflate, br",
    "connection": "keep-alive"
  }
```
- Тело запроса:
```javascript
{
  "id":
  "idBook": 0,
  "url": "string"
}
```
- Заголовки ответа:
```javascript
 access-control-allow-origin: * 
 api-supported-versions: 1.0 
 content-type: application/json; charset=utf-8; v=1.0 
 date: Thu22 Jun 2023 15:17:38 GMT 
 server: Kestrel 
 transfer-encoding: chunked 
 ```
- Тело ответа: 
```javascript
{
    "type": "https://tools.ietf.org/html/rfc7231#section-6.5.1",
    "title": "One or more validation errors occurred.",
    "status": 400,
    "traceId": "00-e5685e87bb7459439b3df90080df4cb9-2d07bc4aae37a44a-00",
    "errors": {
        "id": [
            "The value ' ' is invalid."
        ],
        "$.id": [
            "The JSON value could not be converted to System.Int32. Path: $.id | LineNumber: 2 | BytePositionInLine: 10."
        ]
    }
}
```

## POST/api/v1/Users/{0}
- URL: **{{url глобал}}{{юзеры все глобал}}**
- Ожидаемый результат: статус-код ответа **200**, тест успешно пройден
- Заголовки запроса: 
```javascript
{
    "content-type": "application/json",
    "user-agent": "PostmanRuntime/7.32.3",
    "accept": "*/*",
    "cache-control": "no-cache",
    "postman-token": "4c8d065c-c177-42b9-bf0d-d3f7546143f3",
    "host": "fakerestapi.azurewebsites.net",
    "accept-encoding": "gzip, deflate, br",
    "connection": "keep-alive"
  }
```
- Тело запроса:
```javascript
{
  "id": 0,
  "userName": "string",
  "password": "string"
}
```
- Заголовки ответа:
```javascript
  access-control-allow-origin: * 
 api-supported-versions: 1.0 
 content-type: application/json; charset=utf-8; v=1.0 
 date: Thu22 Jun 2023 15:28:57 GMT 
 server: Kestrel 
 transfer-encoding: chunked 
 ```
- Тело ответа: 
```javascript
{
    "id": 0,
    "userName": "string",
    "password": "string"
}
```

## POST/api/v1/Users/{>int 32}
- URL: **{{url глобал}}{{юзеры все глобал}}**
- Ожидаемый результат: статус-код ответа **400**, тест не пройден
- Заголовки запроса: 
```javascript
{
    "content-type": "application/json",
    "user-agent": "PostmanRuntime/7.32.3",
    "accept": "*/*",
    "cache-control": "no-cache",
    "postman-token": "4c8d065c-c177-42b9-bf0d-d3f7546143f3",
    "host": "fakerestapi.azurewebsites.net",
    "accept-encoding": "gzip, deflate, br",
    "connection": "keep-alive"
  }
```
- Тело запроса:
```javascript
{
  "id": 12345678911,
  "userName": "string",
  "password": "string"
}
```
- Заголовки ответа:
```javascript
  access-control-allow-origin: * 
 api-supported-versions: 1.0 
 content-type: application/json; charset=utf-8; v=1.0 
 date: Thu22 Jun 2023 15:28:57 GMT 
 server: Kestrel 
 transfer-encoding: chunked 
 ```
- Тело ответа: 
```javascript
{
    "type": "https://tools.ietf.org/html/rfc7231#section-6.5.1",
    "title": "One or more validation errors occurred.",
    "status": 400,
    "traceId": "00-ce697945ab872343bb8e196962e1982a-1a6d9a2419005444-00",
    "errors": {
        "id": [
            "The value '2147483648' is not valid."
        ],
        "$.id": [
            "The JSON value could not be converted to System.Int32. Path: $.id | LineNumber: 1 | BytePositionInLine: 19."
        ]
    }
}
```

## POST/api/v1/Users/{null}
- URL: **{{url глобал}}{{юзеры все глобал}}**
- Ожидаемый результат: статус-код ответа **400**, тест не пройден
- Заголовки запроса: 
```javascript
{
    "content-type": "application/json",
    "user-agent": "PostmanRuntime/7.32.3",
    "accept": "*/*",
    "cache-control": "no-cache",
    "postman-token": "4c8d065c-c177-42b9-bf0d-d3f7546143f3",
    "host": "fakerestapi.azurewebsites.net",
    "accept-encoding": "gzip, deflate, br",
    "connection": "keep-alive"
  }
```
- Тело запроса:
```javascript
{
  "id": null,
  "userName": "string",
  "password": "string"
}
```
- Заголовки ответа:
```javascript
  access-control-allow-origin: * 
 api-supported-versions: 1.0 
 content-type: application/json; charset=utf-8; v=1.0 
 date: Thu22 Jun 2023 15:28:57 GMT 
 server: Kestrel 
 transfer-encoding: chunked 
 ```
- Тело ответа: 
```javascript
{
    "type": "https://tools.ietf.org/html/rfc7231#section-6.5.1",
    "title": "One or more validation errors occurred.",
    "status": 400,
    "traceId": "00-5181ab20cfb98f4ab5c47f640fa6a4b9-992cb640f84a5744-00",
    "errors": {
        "id": [
            "The value 'null' is not valid."
        ],
        "$.id": [
            "The JSON value could not be converted to System.Int32. Path: $.id | LineNumber: 1 | BytePositionInLine: 12."
        ]
    }
}
```


## POST/api/v1/Users/{empty line}
- URL: **{{url глобал}}{{юзеры все глобал}}**
- Ожидаемый результат: статус-код ответа **400**, тест не пройден
- Заголовки запроса: 
```javascript
{
    "content-type": "application/json",
    "user-agent": "PostmanRuntime/7.32.3",
    "accept": "*/*",
    "cache-control": "no-cache",
    "postman-token": "4c8d065c-c177-42b9-bf0d-d3f7546143f3",
    "host": "fakerestapi.azurewebsites.net",
    "accept-encoding": "gzip, deflate, br",
    "connection": "keep-alive"
  }
```
- Тело запроса:
```javascript
{
  "id":
  "userName": "string",
  "password": "string"
}
```
- Заголовки ответа:
```javascript
  access-control-allow-origin: * 
 api-supported-versions: 1.0 
 content-type: application/json; charset=utf-8; v=1.0 
 date: Thu22 Jun 2023 15:28:57 GMT 
 server: Kestrel 
 transfer-encoding: chunked 
 ```
- Тело ответа: 
```javascript
{
    "type": "https://tools.ietf.org/html/rfc7231#section-6.5.1",
    "title": "One or more validation errors occurred.",
    "status": 400,
    "traceId": "00-8de75999224efd468b4e60fe853b9c9d-f7b612b489d48241-00",
    "errors": {
        "id": [
            "The value ' ' is invalid."
        ],
        "$.id": [
            "The JSON value could not be converted to System.Int32. Path: $.id | LineNumber: 2 | BytePositionInLine: 12."
        ]
    }
}
```




## DELETE/api/v1/Activities/{1}
- URL: **{{url глобал}}{{вся активность глобал}}/{{1}}**
- Ожидаемый результат: статус-код ответа **200**, тест пройден
- Заголовки запроса: 
```javascript
{
    "user-agent": "PostmanRuntime/7.32.3",
    "accept": "*/*",
    "cache-control": "no-cache",
    "postman-token": "ff9ad3d0-d1aa-4488-b473-5ea27ed9dc2a",
    "host": "fakerestapi.azurewebsites.net",
    "accept-encoding": "gzip, deflate, br",
    "connection": "keep-alive"
  }
```
- Тело запроса:
```javascript
Отсутствует
```
- Заголовки ответа:
```javascript
access-control-allow-origin: * 
 api-supported-versions: 1.0 
 content-length: 0 
 date: Thu22 Jun 2023 18:01:00 GMT 
 server: Kestrel 
 ```
- Тело ответа: 
```c
Отсутствует
```

## DELETE/api/v1/Activities/{0}
- URL: **{{url глобал}}{{вся активность глобал}}/{{0}}**
- Ожидаемый результат: статус-код ответа **404**, тест не пройден
- Заголовки запроса: 
```javascript
{
    "user-agent": "PostmanRuntime/7.32.3",
    "accept": "*/*",
    "cache-control": "no-cache",
    "postman-token": "ff9ad3d0-d1aa-4488-b473-5ea27ed9dc2a",
    "host": "fakerestapi.azurewebsites.net",
    "accept-encoding": "gzip, deflate, br",
    "connection": "keep-alive"
  }
```
- Тело запроса:
```javascript
Отсутствует
```
- Заголовки ответа:
```javascript
access-control-allow-origin: * 
 api-supported-versions: 1.0 
 content-length: 0 
 date: Thu22 Jun 2023 18:14:58 GMT 
 server: Kestrel
 ```
- Тело ответа: 
```javascript
Отсутствует
```
## DELETE/api/v1/Activities/{31}
- URL: **{{url глобал}}{{вся активность глобал}}/{{31}}**
- Ожидаемый результат: статус-код ответа **404**, тест не пройден
- Заголовки запроса: 
```javascript
{
    "user-agent": "PostmanRuntime/7.32.3",
    "accept": "*/*",
    "cache-control": "no-cache",
    "postman-token": "ff9ad3d0-d1aa-4488-b473-5ea27ed9dc2a",
    "host": "fakerestapi.azurewebsites.net",
    "accept-encoding": "gzip, deflate, br",
    "connection": "keep-alive"
  }
```
- Тело запроса:
```javascript
Отсутствует
```
- Заголовки ответа:
```javascript
access-control-allow-origin: * 
 api-supported-versions: 1.0 
 content-length: 0 
 date: Thu22 Jun 2023 18:14:58 GMT 
 server: Kestrel
 ```
- Тело ответа: 
```javascript
Отсутствует
```

## DELETE/api/v1/Activities/{int>32}
- URL: **{{url глобал}}{{вся активность глобал}}/{{>int 32}}**
- Ожидаемый результат: статус-код ответа **400**, тест не пройден
- Заголовки запроса: 
```javascript
{
    "user-agent": "PostmanRuntime/7.32.3",
    "accept": "*/*",
    "cache-control": "no-cache",
    "postman-token": "ff9ad3d0-d1aa-4488-b473-5ea27ed9dc2a",
    "host": "fakerestapi.azurewebsites.net",
    "accept-encoding": "gzip, deflate, br",
    "connection": "keep-alive"
  }
```
- Тело запроса:
```javascript
Отсутствует
```
- Заголовки ответа:
```javascript
access-control-allow-origin: * 
 api-supported-versions: 1.0 
 content-length: 0 
 date: Thu22 Jun 2023 18:14:58 GMT 
 server: Kestrel
 ```
- Тело ответа: 
```javascript
{
    "type": "https://tools.ietf.org/html/rfc7231#section-6.5.1",
    "title": "One or more validation errors occurred.",
    "status": 400,
    "traceId": "00-469d8ff20c170f40a59475a9fbd074f4-7efd863690298d4b-00",
    "errors": {
        "id": [
            "The value '2147483648' is not valid."
        ]
    }
}
```

## DELETE/api/v1/Authors/{1}
- URL: **{{url глобал}}{{авторы все глобал}}/{{1}}**
- Ожидаемый результат: статус-код ответа **200**, тест пройден
- Заголовки запроса: 
```javascript
{
    "user-agent": "PostmanRuntime/7.32.3",
    "accept": "*/*",
    "cache-control": "no-cache",
    "postman-token": "cc770681-8588-4279-9852-66ce79f49070",
    "host": "fakerestapi.azurewebsites.net",
    "accept-encoding": "gzip, deflate, br",
    "connection": "keep-alive"
  }
```
- Тело запроса:
```javascript
Отсутствует
```
- Заголовки ответа:
```javascript
access-control-allow-origin: * 
 api-supported-versions: 1.0 
 content-length: 0 
 date: Thu22 Jun 2023 18:22:27 GMT 
 server: Kestrel
 ```
- Тело ответа: 
```javascript
Отсутствует
```


## DELETE/api/v1/Authors/{0}
- URL: **{{url глобал}}{{авторы все глобал}}/{{0}}**
- Ожидаемый результат: статус-код ответа **404**, тест не пройден
- Заголовки запроса: 
```javascript
{
    "user-agent": "PostmanRuntime/7.32.3",
    "accept": "*/*",
    "cache-control": "no-cache",
    "postman-token": "cc770681-8588-4279-9852-66ce79f49070",
    "host": "fakerestapi.azurewebsites.net",
    "accept-encoding": "gzip, deflate, br",
    "connection": "keep-alive"
  }
```
- Тело запроса:
```javascript
Отсутствует
```
- Заголовки ответа:
```javascript
access-control-allow-origin: * 
 api-supported-versions: 1.0 
 content-length: 0 
 date: Thu22 Jun 2023 18:22:27 GMT 
 server: Kestrel
 ```
- Тело ответа: 
```javascript
Отсутствует
```

## DELETE/api/v1/Authors/{int >32}
- URL: **{{url глобал}}{{авторы все глобал}}/{{>int 32}}**
- Ожидаемый результат: статус-код ответа **400**, тест не пройден
- Заголовки запроса: 
```javascript
{
    "user-agent": "PostmanRuntime/7.32.3",
    "accept": "*/*",
    "cache-control": "no-cache",
    "postman-token": "cc770681-8588-4279-9852-66ce79f49070",
    "host": "fakerestapi.azurewebsites.net",
    "accept-encoding": "gzip, deflate, br",
    "connection": "keep-alive"
  }
```
- Тело запроса:
```javascript
Отсутствует
```
- Заголовки ответа:
```javascript
access-control-allow-origin: * 
 api-supported-versions: 1.0 
 content-length: 0 
 date: Thu22 Jun 2023 18:22:27 GMT 
 server: Kestrel
 ```
- Тело ответа: 
```javascript
{
    "type": "https://tools.ietf.org/html/rfc7231#section-6.5.1",
    "title": "One or more validation errors occurred.",
    "status": 400,
    "traceId": "00-f217273d2dde8a42902d846529377632-d30747f4f959f94b-00",
    "errors": {
        "id": [
            "The value '2147483648' is not valid."
        ]
    }
}
```
## DELETE/api/v1/Authors/{700}
- URL: **{{url глобал}}{{авторы все глобал}}/{{700}}**
- Ожидаемый результат: статус-код ответа **404**, тест не пройден
- Заголовки запроса: 
```javascript
{
    "user-agent": "PostmanRuntime/7.32.3",
    "accept": "*/*",
    "cache-control": "no-cache",
    "postman-token": "cc770681-8588-4279-9852-66ce79f49070",
    "host": "fakerestapi.azurewebsites.net",
    "accept-encoding": "gzip, deflate, br",
    "connection": "keep-alive"
  }
```
- Тело запроса:
```javascript
Отсутствует
```
- Заголовки ответа:
```javascript
access-control-allow-origin: * 
 api-supported-versions: 1.0 
 content-length: 0 
 date: Thu22 Jun 2023 18:22:27 GMT 
 server: Kestrel
 ```
- Тело ответа: 
```javascript
Отсутствует
```

## DELETE/api/v1/Books/{0}
- URL: **{{url глобал}}{{книги все глобал}}/{{0}}**
- Ожидаемый результат: статус-код ответа **404**, тест не пройден
- Заголовки запроса: 
```javascript
{
    "user-agent": "PostmanRuntime/7.32.3",
    "accept": "*/*",
    "cache-control": "no-cache",
    "postman-token": "3e19e665-c01c-45b7-b99b-f70ccc5d52e3",
    "host": "fakerestapi.azurewebsites.net",
    "accept-encoding": "gzip, deflate, br",
    "connection": "keep-alive"
}
```
- Тело запроса:
```javascript
Отсутствует
```
- Заголовки ответа:
```javascript
access-control-allow-origin: * 
 api-supported-versions: 1.0 
 content-length: 0 
 date: Thu22 Jun 2023 18:32:12 GMT 
 server: Kestrel 
 ```
- Тело ответа: 
```javascript
Отсутствует
```

## DELETE/api/v1/Books/{1}
- URL: **{{url глобал}}{{книги все глобал}}/{{1}}**
- Ожидаемый результат: статус-код ответа **200**, тест пройден
- Заголовки запроса: 
```javascript
{
    "user-agent": "PostmanRuntime/7.32.3",
    "accept": "*/*",
    "cache-control": "no-cache",
    "postman-token": "3e19e665-c01c-45b7-b99b-f70ccc5d52e3",
    "host": "fakerestapi.azurewebsites.net",
    "accept-encoding": "gzip, deflate, br",
    "connection": "keep-alive"
}
```
- Тело запроса:
```javascript
Отсутствует
```
- Заголовки ответа:
```javascript
access-control-allow-origin: * 
 api-supported-versions: 1.0 
 content-length: 0 
 date: Thu22 Jun 2023 18:32:12 GMT 
 server: Kestrel 
 ```
- Тело ответа: 
```javascript
Отсутствует
```

## DELETE/api/v1/Books/{201}
- URL: **{{url глобал}}{{книги все глобал}}/{{201}}**
- Ожидаемый результат: статус-код ответа **404**, тест не пройден
- Заголовки запроса: 
```javascript
{
    "user-agent": "PostmanRuntime/7.32.3",
    "accept": "*/*",
    "cache-control": "no-cache",
    "postman-token": "3e19e665-c01c-45b7-b99b-f70ccc5d52e3",
    "host": "fakerestapi.azurewebsites.net",
    "accept-encoding": "gzip, deflate, br",
    "connection": "keep-alive"
}
```
- Тело запроса:
```javascript
Отсутствует
```
- Заголовки ответа:
```javascript
access-control-allow-origin: * 
 api-supported-versions: 1.0 
 content-length: 0 
 date: Thu22 Jun 2023 18:32:12 GMT 
 server: Kestrel 
 ```
- Тело ответа: 
```javascript
Отсутствует
```

## DELETE/api/v1/Books/{int >32}
- URL: **{{url глобал}}{{книги все глобал}}/{{>int 32}}**
- Ожидаемый результат: статус-код ответа **400**, тест не пройден
- Заголовки запроса: 
```javascript
{
    "user-agent": "PostmanRuntime/7.32.3",
    "accept": "*/*",
    "cache-control": "no-cache",
    "postman-token": "3e19e665-c01c-45b7-b99b-f70ccc5d52e3",
    "host": "fakerestapi.azurewebsites.net",
    "accept-encoding": "gzip, deflate, br",
    "connection": "keep-alive"
}
```
- Тело запроса:
```javascript
Отсутствует
```
- Заголовки ответа:
```javascript
access-control-allow-origin: * 
 api-supported-versions: 1.0 
 content-length: 0 
 date: Thu22 Jun 2023 18:32:12 GMT 
 server: Kestrel 
 ```
- Тело ответа: 
```javascript
{
    "type": "https://tools.ietf.org/html/rfc7231#section-6.5.1",
    "title": "One or more validation errors occurred.",
    "status": 400,
    "traceId": "00-2cb73f122b7a0e4fb62f63240917ce29-b0a2908a645ce344-00",
    "errors": {
        "id": [
            "The value '2147483648' is not valid."
        ]
    }
}
```

## DELETE/api/v1/CoverPhotos/{0}
- URL: **{{url глобал}}{{фото все глобал}}/{{0}}**
- Ожидаемый результат: статус-код ответа **404**, тест не пройден
- Заголовки запроса: 
```javascript
{
    "user-agent": "PostmanRuntime/7.32.3",
    "accept": "*/*",
    "cache-control": "no-cache",
    "postman-token": "eab11c3e-19cc-4e4d-ba8a-6c352d30815c",
    "host": "fakerestapi.azurewebsites.net",
    "accept-encoding": "gzip, deflate, br",
    "connection": "keep-alive"
}
```
- Тело запроса:
```javascript
Отсутствует
```
- Заголовки ответа:
```javascript
 access-control-allow-origin: * 
 api-supported-versions: 1.0 
 content-length: 0 
 date: Thu22 Jun 2023 18:40:43 GMT 
 server: Kestrel 
 ```
- Тело ответа: 
```javascript
Отсутствует
```

## DELETE/api/v1/CoverPhotos/{1}
- URL: **{{url глобал}}{{фото все глобал}}/{{1}}**
- Ожидаемый результат: статус-код ответа **200**, тест пройден
- Заголовки запроса: 
```javascript
{
    "user-agent": "PostmanRuntime/7.32.3",
    "accept": "*/*",
    "cache-control": "no-cache",
    "postman-token": "eab11c3e-19cc-4e4d-ba8a-6c352d30815c",
    "host": "fakerestapi.azurewebsites.net",
    "accept-encoding": "gzip, deflate, br",
    "connection": "keep-alive"
}
```
- Тело запроса:
```javascript
Отсутствует
```
- Заголовки ответа:
```javascript
 access-control-allow-origin: * 
 api-supported-versions: 1.0 
 content-length: 0 
 date: Thu22 Jun 2023 18:40:43 GMT 
 server: Kestrel 
 ```
- Тело ответа: 
```javascript
Отсутствует
```

## DELETE/api/v1/CoverPhotos/{201}
- URL: **{{url глобал}}{{фото все глобал}}/{{201}}**
- Ожидаемый результат: статус-код ответа **404**, тест не пройден
- Заголовки запроса: 
```javascript
{
    "user-agent": "PostmanRuntime/7.32.3",
    "accept": "*/*",
    "cache-control": "no-cache",
    "postman-token": "eab11c3e-19cc-4e4d-ba8a-6c352d30815c",
    "host": "fakerestapi.azurewebsites.net",
    "accept-encoding": "gzip, deflate, br",
    "connection": "keep-alive"
}
```
- Тело запроса:
```javascript
Отсутствует
```
- Заголовки ответа:
```javascript
 access-control-allow-origin: * 
 api-supported-versions: 1.0 
 content-length: 0 
 date: Thu22 Jun 2023 18:40:43 GMT 
 server: Kestrel 
 ```
- Тело ответа: 
```javascript
Отсутствует
```

## DELETE/api/v1/CoverPhotos/{int >32}
- URL: **{{url глобал}}{{фото все глобал}}/{{>int 32}}**
- Ожидаемый результат: статус-код ответа **400**, тест не пройден
- Заголовки запроса: 
```javascript
{
    "user-agent": "PostmanRuntime/7.32.3",
    "accept": "*/*",
    "cache-control": "no-cache",
    "postman-token": "eab11c3e-19cc-4e4d-ba8a-6c352d30815c",
    "host": "fakerestapi.azurewebsites.net",
    "accept-encoding": "gzip, deflate, br",
    "connection": "keep-alive"
}
```
- Тело запроса:
```javascript
Отсутствует
```
- Заголовки ответа:
```javascript

 ```
- Тело ответа: 
```javascript
{
    "type": "https://tools.ietf.org/html/rfc7231#section-6.5.1",
    "title": "One or more validation errors occurred.",
    "status": 400,
    "traceId": "00-0a650907d078184896ae9d3727e218be-a0b94abcda692f44-00",
    "errors": {
        "id": [
            "The value '2147483648' is not valid."
        ]
    }
}
```

## DELETE/api/v1/Users/{0}
- URL: **{{url глобал}}{{юзеры все глобал}}/{{0}}**
- Ожидаемый результат: статус-код ответа **404**, тест не пройден
- Заголовки запроса: 
```javascript
{
    "user-agent": "PostmanRuntime/7.32.3",
    "accept": "*/*",
    "cache-control": "no-cache",
    "postman-token": "038efe79-fb50-40e2-ab0e-477674c3b0cd",
    "host": "fakerestapi.azurewebsites.net",
    "accept-encoding": "gzip, deflate, br",
    "connection": "keep-alive"
}
```
- Тело запроса:
```javascript
Отсутствует
```
- Заголовки ответа:
```javascript
 access-control-allow-origin: * 
 api-supported-versions: 1.0 
 content-length: 0 
 date: Thu22 Jun 2023 18:45:50 GMT 
 server: Kestrel 
 ```
- Тело ответа: 
```javascript
Отсутствует
```

## DELETE/api/v1/Users/{1}
- URL: **{{url глобал}}{{юзеры все глобал}}/{{1}}**
- Ожидаемый результат: статус-код ответа **200**, тест пройден
- Заголовки запроса: 
```javascript
{
    "user-agent": "PostmanRuntime/7.32.3",
    "accept": "*/*",
    "cache-control": "no-cache",
    "postman-token": "038efe79-fb50-40e2-ab0e-477674c3b0cd",
    "host": "fakerestapi.azurewebsites.net",
    "accept-encoding": "gzip, deflate, br",
    "connection": "keep-alive"
}
```
- Тело запроса:
```javascript
Отсутствует
```
- Заголовки ответа:
```javascript
 access-control-allow-origin: * 
 api-supported-versions: 1.0 
 content-length: 0 
 date: Thu22 Jun 2023 18:45:50 GMT 
 server: Kestrel 
 ```
- Тело ответа: 
```javascript
Отсутствует
```

## DELETE/api/v1/Users/{11}
- URL: **{{url глобал}}{{юзеры все глобал}}/{{11}}**
- Ожидаемый результат: статус-код ответа **404**, тест не пройден
- Заголовки запроса: 
```javascript
{
    "user-agent": "PostmanRuntime/7.32.3",
    "accept": "*/*",
    "cache-control": "no-cache",
    "postman-token": "038efe79-fb50-40e2-ab0e-477674c3b0cd",
    "host": "fakerestapi.azurewebsites.net",
    "accept-encoding": "gzip, deflate, br",
    "connection": "keep-alive"
}
```
- Тело запроса:
```javascript
Отсутствует
```
- Заголовки ответа:
```javascript
 access-control-allow-origin: * 
 api-supported-versions: 1.0 
 content-length: 0 
 date: Thu22 Jun 2023 18:45:50 GMT 
 server: Kestrel 
 ```
- Тело ответа: 
```javascript
Отсутствует
```

## DELETE/api/v1/Users/{int >32}
- URL: **{{url глобал}}{{юзеры все глобал}}/{{>int 32}}**
- Ожидаемый результат: статус-код ответа **400**, тест не пройден
- Заголовки запроса: 
```javascript
{
    "user-agent": "PostmanRuntime/7.32.3",
    "accept": "*/*",
    "cache-control": "no-cache",
    "postman-token": "038efe79-fb50-40e2-ab0e-477674c3b0cd",
    "host": "fakerestapi.azurewebsites.net",
    "accept-encoding": "gzip, deflate, br",
    "connection": "keep-alive"
}
```
- Тело запроса:
```javascript
Отсутствует
```
- Заголовки ответа:
```javascript
 access-control-allow-origin: * 
 api-supported-versions: 1.0 
 content-length: 0 
 date: Thu22 Jun 2023 18:45:50 GMT 
 server: Kestrel 
 ```
- Тело ответа: 
```javascript
{
    "type": "https://tools.ietf.org/html/rfc7231#section-6.5.1",
    "title": "One or more validation errors occurred.",
    "status": 400,
    "traceId": "00-225d76ab87cc4a419b4a01eef6b54588-dae0595356168943-00",
    "errors": {
        "id": [
            "The value '2147483648' is not valid."
        ]
    }
}
```

## GET/api/v1/Activities
- URL: **{{url глобал}}{{вся активность глобал}}**
- Ожидаемый результат: статус-код ответа **200**, тест успешно пройден
- Заголовки запроса: 
```javascript
User-Agent: PostmanRuntime/7.32.3
Accept: */*
Cache-Control: no-cache
Postman-Token: 3290e940-7bc1-4779-96d0-92c16869a03f
Host: fakerestapi.azurewebsites.net
Accept-Encoding: gzip, deflate, br
Connection: keep-alive
```
- Тело запроса: none
- Заголовки ответа:
```javascript
Content-Type: application/json; charset=utf-8; v=1.0
Date: Thu, 22 Jun 2023 19:45:21 GMT
Server: Kestrel
Transfer-Encoding: chunked
api-supported-versions: 1.0
```
- Тело ответа: слишком большое, только часть
```javascript
[{"id":1,"title":"Activity 1","dueDate":"2023-06-22T20:45:22.4643039+00:00","completed":false},{"id":2,"title":"Activity 2","dueDate":"2023-06-22T21:45:22.4643061+00:00","completed":true},{"id":3,"title":"Activity 3","dueDate":"2023-06-22T22:45:22.4643064+00:00","completed":false},{"id":4,"title":"Activity 4","dueDate":"2023-06-22T23:45:22.4643067+00:00","completed":true},{"id":5,"title":"Activity 5","dueDate":"2023-06-23T00:45:22.464307+00:00","completed":false},{"id":6,"title":"Activity 6","dueDate":"2023-06-23T01:45:22.4643076+00:00","completed":true},{"id":7,"title":"Activity 7","dueDate":"2023-06-23T02:45:22.4643079+00:00","completed":false}]
```

## GET/api/v1/Activities/{0}
- URL: **{{url глобал}}{{вся активность глобал}}/{{0}}**
- Ожидаемый результат: статус-код ответа **404**, тест успешно пройден
- Заголовки запроса: 
```javascript
User-Agent: PostmanRuntime/7.32.3
Accept: */*
Cache-Control: no-cache
Postman-Token: 277fbc70-5759-4d6b-a0cc-4b440313aa8f
Host: fakerestapi.azurewebsites.net
Accept-Encoding: gzip, deflate, br
Connection: keep-alive
```
- Тело запроса: none
- Заголовки ответа:
```javascript
Content-Type: application/problem+json; charset=utf-8; v=1.0
Date: Thu, 22 Jun 2023 19:53:47 GMT
Server: Kestrel
Transfer-Encoding: chunked
api-supported-versions: 1.0
 ```
- Тело ответа: 
```javascript
{"type":"https://tools.ietf.org/html/rfc7231#section-6.5.4","title":"Not Found","status":404,"traceId":"00-c7a8dabf750114469242467572b85630-892f390602d4754e-00"}
```

## GET/api/v1/Activities/{1} 
- URL: **{{url глобал}}{{вся активность глобал}}/{{1}}**
- Ожидаемый результат: статус-код ответа **200**, тест успешно пройден
- Заголовки запроса: 
```javascript
User-Agent: PostmanRuntime/7.32.3
Accept: */*
Cache-Control: no-cache
Postman-Token: 2dfe33f7-4793-46f3-bbc5-fe66839841e1
Host: fakerestapi.azurewebsites.net
Accept-Encoding: gzip, deflate, br
Connection: keep-alive
```
- Тело запроса: none
- Заголовки ответа:
```javascript
Content-Type: application/json; charset=utf-8; v=1.0
Date: Thu, 22 Jun 2023 19:59:03 GMT
Server: Kestrel
Transfer-Encoding: chunked
api-supported-versions: 1.0 
 ```
- Тело ответа: 
```javascript
{"id":1,"title":"Activity 1","dueDate":"2023-06-22T20:59:04.9254343+00:00","completed":false}
```

## GET/api/v1/Activities/{31}
- URL: **{{url глобал}}{{вся активность глобал}}/{{31}}**
- Ожидаемый результат: статус-код ответа **404**, тест успешно пройден
- Заголовки запроса: 
```javascript
User-Agent: PostmanRuntime/7.32.3
Accept: */*
Cache-Control: no-cache
Postman-Token: 0e22275a-2d16-4425-bcb7-d18c3fc101da
Host: fakerestapi.azurewebsites.net
Accept-Encoding: gzip, deflate, br
Connection: keep-alive
```
- Тело запроса: none
- Заголовки ответа:
```javascript
Content-Type: application/problem+json; charset=utf-8; v=1.0
Date: Thu, 22 Jun 2023 20:02:25 GMT
Server: Kestrel
Transfer-Encoding: chunked
api-supported-versions: 1.0
 ```
- Тело ответа: 
```javascript
{"type":"https://tools.ietf.org/html/rfc7231#section-6.5.4","title":"Not Found","status":404,"traceId":"00-bb10edba97d1304eae9373a836066642-9862054a2091eb43-00"}
```

## GET/api/v1/Activities/{>int 32}
- URL: **{{url глобал}}{{вся активность глобал}}/{{2147483648}}**
- Ожидаемый результат: статус-код ответа **400**, тест успешно пройден
- Заголовки запроса: 
```javascript
User-Agent: PostmanRuntime/7.32.3
Accept: */*
Cache-Control: no-cache
Postman-Token: 1aa8830c-e5c0-4554-a64b-926bdf47bad7
Host: fakerestapi.azurewebsites.net
Accept-Encoding: gzip, deflate, br
Connection: keep-alive
```
- Тело запроса: none
- Заголовки ответа:
```javascript
Content-Type: application/problem+json; charset=utf-8
Date: Thu, 22 Jun 2023 20:05:46 GMT
Server: Kestrel
Transfer-Encoding: chunked 
 ```
- Тело ответа: 
```javascript
{"type":"https://tools.ietf.org/html/rfc7231#section-6.5.1","title":"One or more validation errors occurred.","status":400,"traceId":"00-ae8e9d880c16fb40af2c312f18a78962-cfc69c6123c1fb4d-00","errors":{"id":["The value '2147483648' is not valid."]}}
```

## GET/api/v1/Authors
- URL: **{{url глобал}}{{авторы все глобал}}**
- Ожидаемый результат: статус-код ответа **200**, тест успешно пройден
- Заголовки запроса: 
```javascript
User-Agent: PostmanRuntime/7.32.3
Accept: */*
Cache-Control: no-cache
Postman-Token: 1c328892-2ea1-4200-a3b4-880e101bf0e1
Host: fakerestapi.azurewebsites.net
Accept-Encoding: gzip, deflate, br
Connection: keep-alive
```
- Тело запроса: none
- Заголовки ответа:
```javascript
User-Agent: PostmanRuntime/7.32.3
Accept: */*
Cache-Control: no-cache
Postman-Token: 1c328892-2ea1-4200-a3b4-880e101bf0e1
Host: fakerestapi.azurewebsites.net
Accept-Encoding: gzip, deflate, br
Connection: keep-alive 
 ```
- Тело ответа: слишком большое, только часть
```javascript
[{"id":1,"idBook":1,"firstName":"First Name 1","lastName":"Last Name 1"},{"id":2,"idBook":1,"firstName":"First Name 2","lastName":"Last Name 2"},{"id":3,"idBook":1,"firstName":"First Name 3","lastName":"Last Name 3"},{"id":4,"idBook":1,"firstName":"First Name 4","lastName":"Last Name 4"},{"id":5,"idBook":2,"firstName":"First Name 5","lastName":"Last Name 5"},{"id":6,"idBook":2,"firstName":"First Name 6","lastName":"Last Name 6"},{"id":7,"idBook":2,"firstName":"First Name 7","lastName":"Last Name 7"}]
```

## GET​/api​/v1​/Authors​/{0}
- URL: **{{url глобал}}{{авторы все глобал}}/{{0}}**
- Ожидаемый результат: статус-код ответа **404**, тест успешно пройден
- Заголовки запроса: 
```javascript
User-Agent: PostmanRuntime/7.32.3
Accept: */*
Cache-Control: no-cache
Postman-Token: f64e588b-e3b3-4d7f-bc67-ddf90de5f257
Host: fakerestapi.azurewebsites.net
Accept-Encoding: gzip, deflate, br
Connection: keep-alive
```
- Тело запроса: none
- Заголовки ответа:
```javascript
Content-Type: application/problem+json; charset=utf-8; v=1.0
Date: Thu, 22 Jun 2023 20:12:17 GMT
Server: Kestrel
Transfer-Encoding: chunked
api-supported-versions: 1.0
 ```
- Тело ответа: 
```javascript
{"type":"https://tools.ietf.org/html/rfc7231#section-6.5.4","title":"Not Found","status":404,"traceId":"00-fc5a6ca5bbb24543af1820ca7b87c698-e3c9017830073a49-00"}
```


## GET​/api​/v1​/Authors​/{1}
- URL: **{{url глобал}}{{авторы все глобал}}/{{1}}**
- Ожидаемый результат: статус-код ответа **200**, тест успешно пройден
- Заголовки запроса: 
```javascript
User-Agent: PostmanRuntime/7.32.3
Accept: */*
Cache-Control: no-cache
Postman-Token: 20d36b65-8922-43ac-beb9-4458260a8843
Host: fakerestapi.azurewebsites.net
Accept-Encoding: gzip, deflate, br
Connection: keep-alive
```
- Тело запроса: none
- Заголовки ответа:
```javascript
Content-Type: application/json; charset=utf-8; v=1.0
Date: Thu, 22 Jun 2023 20:13:43 GMT
Server: Kestrel
Transfer-Encoding: chunked
api-supported-versions: 1.0 
 ```
- Тело ответа: 
```javascript
{"id":1,"idBook":1,"firstName":"First Name 1","lastName":"Last Name 1"}
```

## GET​/api​/v1​/Authors​/{700}
- URL: **{{url глобал}}{{авторы все глобал}}/{{700}}**
- Ожидаемый результат: статус-код ответа **404**, тест успешно пройден
- Заголовки запроса: 
```javascript
User-Agent: PostmanRuntime/7.32.3
Accept: */*
Cache-Control: no-cache
Postman-Token: be77ce40-9902-4bef-8596-8ac0ba279bbb
Host: fakerestapi.azurewebsites.net
Accept-Encoding: gzip, deflate, br
Connection: keep-alive
```
- Тело запроса: none
- Заголовки ответа:
```javascript
Content-Type: application/problem+json; charset=utf-8; v=1.0
Date: Thu, 22 Jun 2023 20:17:21 GMT
Server: Kestrel
Transfer-Encoding: chunked
api-supported-versions: 1.0 
 ```
- Тело ответа: 
```javascript
{"type":"https://tools.ietf.org/html/rfc7231#section-6.5.4","title":"Not Found","status":404,"traceId":"00-3a333735886cc94c865ec5830df06697-2ca44a0cc2e3244c-00"}
```

## GET​/api​/v1​/Authors​/{2147483648}
- URL: **{{url глобал}}{{авторы все глобал}}/{{>int 32}}**
- Ожидаемый результат: статус-код ответа **400**, тест успешно пройден
- Заголовки запроса: 
```javascript
User-Agent: PostmanRuntime/7.32.3
Accept: */*
Cache-Control: no-cache
Postman-Token: 5d3e499f-efa9-4c4a-9a0e-526667625760
Host: fakerestapi.azurewebsites.net
Accept-Encoding: gzip, deflate, br
Connection: keep-alive
```
- Тело запроса: none
- Заголовки ответа:
```javascript
Content-Type: application/problem+json; charset=utf-8
Date: Thu, 22 Jun 2023 20:21:12 GMT
Server: Kestrel
Transfer-Encoding: chunked 
 ```
- Тело ответа: 
```javascript
{"type":"https://tools.ietf.org/html/rfc7231#section-6.5.1","title":"One or more validation errors occurred.","status":400,"traceId":"00-7df389532cc5294fa705cd6b34cd499b-484399c1f7f5ef46-00","errors":{"id":["The value '2147483648' is not valid."]}}
```

## GET​/api​/v1​/Authors​/{012} БАГ
- URL: **{{url глобал}}{{авторы все глобал}}/{{012}}**
- Ожидаемый результат: статус-код ответа **404**, тест успешно пройден
- Фактический результат: статус-код ответа **200**
- Заголовки запроса: 
```javascript
User-Agent: PostmanRuntime/7.32.3
Accept: */*
Cache-Control: no-cache
Postman-Token: 0b5f7b18-8ea9-4021-8928-8e5b9859fb1e
Host: fakerestapi.azurewebsites.net
Accept-Encoding: gzip, deflate, br
Connection: keep-alive
```
- Тело запроса: none
- Заголовки ответа:
```javascript
Content-Type: application/json; charset=utf-8; v=1.0
Date: Thu, 22 Jun 2023 20:23:42 GMT
Server: Kestrel
Transfer-Encoding: chunked
api-supported-versions: 1.0
 ```
- Тело ответа: 
```javascript
{"id":12,"idBook":5,"firstName":"First Name 12","lastName":"Last Name 12"}
```

## GET​/api​/v1​/authors​/books​/{0} БАГ
- URL: **{{url глобал}}{{авторы все глобал}}/{{авторы/книги}}/{{0}}**
- Ожидаемый результат: статус-код ответа **404**, тест успешно пройден
- Фактический результат: статус-код ответа **200**
- Заголовки запроса: 
```javascript
User-Agent: PostmanRuntime/7.32.3
Accept: */*
Cache-Control: no-cache
Postman-Token: bf740286-5da9-41bc-881d-0d9ed10cf33f
Host: fakerestapi.azurewebsites.net
Accept-Encoding: gzip, deflate, br
Connection: keep-alive
```
- Тело запроса: none
- Заголовки ответа:
```javascript
Content-Type: application/json; charset=utf-8; v=1.0
Date: Thu, 22 Jun 2023 20:31:32 GMT
Server: Kestrel
Transfer-Encoding: chunked
api-supported-versions: 1.0 
 ```
- Тело ответа: 
```javascript
[]
```

## GET​/api​/v1​/authors​/books​/ {1} БАГ
- URL: **{{url глобал}}{{авторы все глобал}}/{{авторы/книги}}/{{1}}**
- Ожидаемый результат: статус-код ответа **200**, тест успешно пройден
- Тело ответа ожидаемый результат:
```javascript
{
    "id": 1,
    "idBook": 1,
    "firstName": "First Name 1",
    "lastName": "Last Name 1"
  },
  {
    "id": 2,
    "idBook": 1,
    "firstName": "First Name 2",
    "lastName": "Last Name 2"
  },
  {
    "id": 3,
    "idBook": 1,
    "firstName": "First Name 3",
    "lastName": "Last Name 3"
  },
  {
    "id": 4,
    "idBook": 1,
    "firstName": "First Name 4",
    "lastName": "Last Name 4"
  }
  ```
- Заголовки запроса: 
```javascript
User-Agent: PostmanRuntime/7.32.3
Accept: */*
Cache-Control: no-cache
Postman-Token: b3b39780-f221-4c2b-bd81-f87788eabdcb
Host: fakerestapi.azurewebsites.net
Accept-Encoding: gzip, deflate, br
Connection: keep-alive
```
- Тело запроса: none
- Заголовки ответа:
```javascript
Content-Type: application/json; charset=utf-8; v=1.0
Date: Thu, 22 Jun 2023 20:35:06 GMT
Server: Kestrel
Transfer-Encoding: chunked
api-supported-versions: 1.0 
 ```
- Тело ответа: 
```javascript
[{"id":1,"idBook":1,"firstName":"First Name 1","lastName":"Last Name 1"},{"id":2,"idBook":1,"firstName":"First Name 2","lastName":"Last Name 2"},{"id":3,"idBook":1,"firstName":"First Name 3","lastName":"Last Name 3"}]
```


## GET​/api​/v1​/authors​/books​/ {201} БАГ
- URL: **{{url глобал}}{{авторы все глобал}}/{{авторы/книги}}/{{201}}**
- Ожидаемый результат: статус-код ответа **404**, тест успешно пройден
- - Фактический результат: статус-код ответа **200**
- Заголовки запроса: 
```javascript
User-Agent: PostmanRuntime/7.32.3
Accept: */*
Cache-Control: no-cache
Postman-Token: 690bc820-636a-4122-9888-c74a667c42c9
Host: fakerestapi.azurewebsites.net
Accept-Encoding: gzip, deflate, br
Connection: keep-alive
```
- Тело запроса: none
- Заголовки ответа:
```javascript
Content-Type: application/json; charset=utf-8; v=1.0
Date: Thu, 22 Jun 2023 20:38:07 GMT
Server: Kestrel
Transfer-Encoding: chunked
api-supported-versions: 1.0
 ```
- Тело ответа: 
```javascript
[]
```

## GET​/api​/v1​/Authors​/{2147483648}
- URL: **{{url глобал}}{{авторы все глобал}}/{{авторы/книги}}/{{>int 32}}**
- Ожидаемый результат: статус-код ответа **400**, тест успешно пройден
- Заголовки запроса: 
```javascript
User-Agent: PostmanRuntime/7.32.3
Accept: */*
Cache-Control: no-cache
Postman-Token: b0d1011d-cf70-442e-952c-9bf04cc167e7
Host: fakerestapi.azurewebsites.net
Accept-Encoding: gzip, deflate, br
Connection: keep-alive
```
- Тело запроса: none
- Заголовки ответа:
```javascript
Content-Type: application/problem+json; charset=utf-8
Date: Thu, 22 Jun 2023 20:39:53 GMT
Server: Kestrel
Transfer-Encoding: chunked
 ```
- Тело ответа: 
```javascript
{"type":"https://tools.ietf.org/html/rfc7231#section-6.5.1","title":"One or more validation errors occurred.","status":400,"traceId":"00-2dd53606cac9f9458cc6380a8bbbf960-fb993010d276e345-00","errors":{"idBook":["The value '2147483648' is not valid."]}}
```

## GET​/api​/v1​/Authors​//books​/{012} БАГ
- URL: **{{url глобал}}{{авторы все глобал}}/{{авторы/книги}}/{{012}}**
- Ожидаемый результат: статус-код ответа **404**, тест успешно пройден
- Фактический результат: статус-код ответа **200**
- Заголовки запроса: 
```javascript
User-Agent: PostmanRuntime/7.32.3
Accept: */*
Cache-Control: no-cache
Postman-Token: 3f4e1eb0-10c6-4b89-ad98-956479047d80
Host: fakerestapi.azurewebsites.net
Accept-Encoding: gzip, deflate, br
Connection: keep-alive
```
- Тело запроса: none
- Заголовки ответа:
```javascript
Content-Type: application/json; charset=utf-8; v=1.0
Date: Thu, 22 Jun 2023 20:44:05 GMT
Server: Kestrel
Transfer-Encoding: chunked
api-supported-versions: 1.0 
 ```
- Тело ответа: 
```javascript
Content-Type: application/json; charset=utf-8; v=1.0
Date: Thu, 22 Jun 2023 20:44:05 GMT
Server: Kestrel
Transfer-Encoding: chunked
api-supported-versions: 1.0
```

## GET​/api​/v1​/Books
- URL: **{{url глобал}}{{книги все глобал}}**
- Ожидаемый результат: статус-код ответа **200**, тест успешно пройден
- Заголовки запроса: 
```javascript
User-Agent: PostmanRuntime/7.32.3
Accept: */*
Cache-Control: no-cache
Postman-Token: ebc41045-36b5-44c7-8c4e-3e675e56a0ef
Host: fakerestapi.azurewebsites.net
Accept-Encoding: gzip, deflate, br
Connection: keep-alive
```
- Тело запроса: none
- Заголовки ответа:
```javascript
Content-Type: application/json; charset=utf-8; v=1.0
Date: Thu, 22 Jun 2023 20:50:28 GMT
Server: Kestrel
Transfer-Encoding: chunked
api-supported-versions: 1.0 
 ```
- Тело ответа: 
```javascript
[{"id":1,"title":"Book 1","description":"Lorem lorem lorem. Lorem lorem lorem. Lorem lorem lorem.\n","pageCount":100,"excerpt":"Lorem lorem lorem. Lorem lorem lorem. Lorem lorem lorem.\nLorem lorem lorem. Lorem lorem lorem. Lorem lorem lorem.\nLorem lorem lorem. Lorem lorem lorem. Lorem lorem lorem.\nLorem lorem lorem. Lorem lorem lorem. Lorem lorem lorem.\nLorem lorem lorem. Lorem lorem lorem. Lorem lorem lorem.\n","publishDate":"2023-06-21T20:50:28.9546872+00:00"},{"id":2,"title":"Book 2","description":"Lorem lorem lorem. Lorem lorem lorem. Lorem lorem lorem.\n","pageCount":200,"excerpt":"Lorem lorem lorem. Lorem lorem lorem. Lorem lorem lorem.\nLorem lorem lorem. Lorem lorem lorem. Lorem lorem lorem.\nLorem lorem lorem. Lorem lorem lorem. Lorem lorem lorem.\nLorem lorem lorem. Lorem lorem lorem. Lorem lorem lorem.\nLorem lorem lorem. Lorem lorem lorem. Lorem lorem lorem.\n","publishDate":"2023-06-20T20:50:28.9547011+00:00"}]
```

## GET​/api​/v1​/Books​/{1} БАГ
- URL: **{{url глобал}}{{книги все глобал}}/{{1}}**
- Ожидаемый результат: статус-код ответа **200**, тест успешно пройден
Фактический результат: присутствуют различия в теле ответа в: 
```
"description"
"excerpt"
"publishDate"
```
- Заголовки запроса: 
```javascript
User-Agent: PostmanRuntime/7.32.3
Accept: */*
Cache-Control: no-cache
Postman-Token: 8db11ffb-5549-446a-87b4-61c8bb53283f
Host: fakerestapi.azurewebsites.net
Accept-Encoding: gzip, deflate, br
Connection: keep-alive
```
- Тело запроса: none
- Заголовки ответа:
```javascript
Content-Type: application/json; charset=utf-8; v=1.0
Date: Thu, 22 Jun 2023 20:56:35 GMT
Server: Kestrel
Transfer-Encoding: chunked
api-supported-versions: 1.0 
 ```
- Тело ответа: 
```javascript
{"id":1,"title":"Book 1","description":"Lorem lorem lorem. Lorem lorem lorem. Lorem lorem lorem.\n","pageCount":100,"excerpt":"Lorem lorem lorem. Lorem lorem lorem. Lorem lorem lorem.\nLorem lorem lorem. Lorem lorem lorem. Lorem lorem lorem.\nLorem lorem lorem. Lorem lorem lorem. Lorem lorem lorem.\nLorem lorem lorem. Lorem lorem lorem. Lorem lorem lorem.\nLorem lorem lorem. Lorem lorem lorem. Lorem lorem lorem.\n","publishDate":"2023-06-21T20:56:35.6683776+00:00"}
```

## GET​/api​/v1​/Books​/{201}
- URL: **{{url глобал}}{{книги все глобал}}/{{201}}**
- Ожидаемый результат: статус-код ответа **404**, тест успешно пройден
- Заголовки запроса: 
```javascript
User-Agent: PostmanRuntime/7.32.3
Accept: */*
Cache-Control: no-cache
Postman-Token: a50c3a20-72d4-46fc-a2ee-86efca44611a
Host: fakerestapi.azurewebsites.net
Accept-Encoding: gzip, deflate, br
Connection: keep-alive
```
- Тело запроса: none
- Заголовки ответа:
```javascript
Content-Type: application/problem+json; charset=utf-8; v=1.0
Date: Thu, 22 Jun 2023 20:58:32 GMT
Server: Kestrel
Transfer-Encoding: chunked
api-supported-versions: 1.0 
 ```
- Тело ответа: 
```javascript
{"type":"https://tools.ietf.org/html/rfc7231#section-6.5.4","title":"Not Found","status":404,"traceId":"00-c0465ed1fb1df64ba939e5b2c98cbfd7-42f082d4b7468842-00"}
```


## GET​/api​/v1​/Books​/{0} 
- URL: ****
- Ожидаемый результат: статус-код ответа ****, тест успешно пройден
- Заголовки запроса: 
```javascript
User-Agent: PostmanRuntime/7.32.3
Accept: */*
Cache-Control: no-cache
Postman-Token: e52c0ab3-c0b6-4502-a9b2-f87c28e13f33
Host: fakerestapi.azurewebsites.net
Accept-Encoding: gzip, deflate, br
Connection: keep-alive
```
- Тело запроса: none
- Заголовки ответа:
```javascript
Content-Type: application/problem+json; charset=utf-8; v=1.0
Date: Thu, 22 Jun 2023 20:59:49 GMT
Server: Kestrel
Transfer-Encoding: chunked
api-supported-versions: 1.0
 ```
- Тело ответа: 
```javascript
{"type":"https://tools.ietf.org/html/rfc7231#section-6.5.4","title":"Not Found","status":404,"traceId":"00-cbdaf6350a98ae43b71e0051eb093675-3fcc7dd0b3e9c14e-00"}
```

## GET​/api​/v1​/Books/{2147483648}
- URL: **{{url глобал}}{{книги все глобал}}/{{>int 32}}**
- Ожидаемый результат: статус-код ответа **400**, тест успешно пройден
- Заголовки запроса: 
```javascript
User-Agent: PostmanRuntime/7.32.3
Accept: */*
Cache-Control: no-cache
Postman-Token: b85f820b-c899-40d5-86d4-7d4c1b358039
Host: fakerestapi.azurewebsites.net
Accept-Encoding: gzip, deflate, br
Connection: keep-alive
```
- Тело запроса: none
- Заголовки ответа:
```javascript
Content-Type: application/problem+json; charset=utf-8
Date: Thu, 22 Jun 2023 21:01:26 GMT
Server: Kestrel
Transfer-Encoding: chunked
 ```
- Тело ответа: 
```javascript
{"type":"https://tools.ietf.org/html/rfc7231#section-6.5.1","title":"One or more validation errors occurred.","status":400,"traceId":"00-8473d7803dbfa74b9fc337f68d9782b2-21668144817be249-00","errors":{"id":["The value '2147483648' is not valid."]}}
```

## GET​/api​/v1​/CoverPhotos
- URL: **{{url глобал}}{{фото все глобал}}**
- Ожидаемый результат: статус-код ответа **200**, тест успешно пройден
- Заголовки запроса: 
```javascript
User-Agent: PostmanRuntime/7.32.3
Accept: */*
Cache-Control: no-cache
Postman-Token: 9920cb99-d919-488c-aa60-9ac32d76c5ab
Host: fakerestapi.azurewebsites.net
Accept-Encoding: gzip, deflate, br
Connection: keep-alive
```
- Тело запроса: none
- Заголовки ответа:
```javascript
Content-Type: application/json; charset=utf-8; v=1.0
Date: Thu, 22 Jun 2023 21:04:01 GMT
Server: Kestrel
Transfer-Encoding: chunked
api-supported-versions: 1.0 
 ```
- Тело ответа: 
```javascript
[{"id":1,"idBook":1,"url":"https://placeholdit.imgix.net/~text?txtsize=33&txt=Book 1&w=250&h=350"},{"id":2,"idBook":2,"url":"https://placeholdit.imgix.net/~text?txtsize=33&txt=Book 2&w=250&h=350"},{"id":3,"idBook":3,"url":"https://placeholdit.imgix.net/~text?txtsize=33&txt=Book 3&w=250&h=350"},{"id":4,"idBook":4,"url":"https://placeholdit.imgix.net/~text?txtsize=33&txt=Book 4&w=250&h=350"},{"id":5,"idBook":5,"url":"https://placeholdit.imgix.net/~text?txtsize=33&txt=Book 5&w=250&h=350"},{"id":6,"idBook":6,"url":"https://placeholdit.imgix.net/~text?txtsize=33&txt=Book 6&w=250&h=350"},{"id":7,"idBook":7,"url":"https://placeholdit.imgix.net/~text?txtsize=33&txt=Book 7&w=250&h=350"}]
```

## GET​/api​/v1​/CoverPhotos​/{0}
- URL: **{{url глобал}}{{фото все глобал}}/{{0}}**
- Ожидаемый результат: статус-код ответа **404**, тест успешно пройден
- Заголовки запроса: 
```javascript
User-Agent: PostmanRuntime/7.32.3
Accept: */*
Cache-Control: no-cache
Postman-Token: 00c38924-20c6-4a87-9c41-e877f38abb9a
Host: fakerestapi.azurewebsites.net
Accept-Encoding: gzip, deflate, br
Connection: keep-alive
```
- Тело запроса: none
- Заголовки ответа:
```javascript
Content-Type: application/problem+json; charset=utf-8; v=1.0
Date: Thu, 22 Jun 2023 21:05:31 GMT
Server: Kestrel
Transfer-Encoding: chunked
api-supported-versions: 1.0 
 ```
- Тело ответа: 
```javascript
{"type":"https://tools.ietf.org/html/rfc7231#section-6.5.4","title":"Not Found","status":404,"traceId":"00-b33285bdbd3c4e4bab575053402ff6bf-31b5d9fc9aad1445-00"}
```

## GET​/api​/v1​/CoverPhotos/{1}
- URL: **{{url глобал}}{{фото все глобал}}/{{1}}**
- Ожидаемый результат: статус-код ответа **200**, тест успешно пройден
- Заголовки запроса: 
```javascript
User-Agent: PostmanRuntime/7.32.3
Accept: */*
Cache-Control: no-cache
Postman-Token: 76e8ff7a-015b-48eb-b87f-cf33d3f9b41a
Host: fakerestapi.azurewebsites.net
Accept-Encoding: gzip, deflate, br
Connection: keep-alive
```
- Тело запроса: none
- Заголовки ответа:
```javascript
Content-Type: application/json; charset=utf-8; v=1.0
Date: Thu, 22 Jun 2023 21:07:18 GMT
Server: Kestrel
Transfer-Encoding: chunked
api-supported-versions: 1.0 
 ```
- Тело ответа: 
```javascript
{"id":1,"idBook":1,"url":"https://placeholdit.imgix.net/~text?txtsize=33&txt=Book 1&w=250&h=350"}
```

## GET​/api​/v1​/CoverPhotos​/{201}
- URL: **{{url глобал}}{{фото все глобал}}/{{201}}**
- Ожидаемый результат: статус-код ответа **404**, тест успешно пройден
- Заголовки запроса: 
```javascript
User-Agent: PostmanRuntime/7.32.3
Accept: */*
Cache-Control: no-cache
Postman-Token: d377fb93-ea5e-461d-ac15-dc31f227b766
Host: fakerestapi.azurewebsites.net
Accept-Encoding: gzip, deflate, br
Connection: keep-alive
```
- Тело запроса: none
- Заголовки ответа:
```javascript
Content-Type: application/problem+json; charset=utf-8; v=1.0
Date: Thu, 22 Jun 2023 21:08:57 GMT
Server: Kestrel
Transfer-Encoding: chunked
api-supported-versions: 1.0 
 ```
- Тело ответа: 
```javascript
{"type":"https://tools.ietf.org/html/rfc7231#section-6.5.4","title":"Not Found","status":404,"traceId":"00-f877e39559fa3047bfb7961dbd3a5787-a774e2ebcfe1e24d-00"}
```
## GET​/api​/v1​/CoverPhotos/{2147483648}
- URL: **{{url глобал}}{{фото все глобал}}/{{>int 32}}**
- Ожидаемый результат: статус-код ответа **400**, тест успешно пройден
- Заголовки запроса: 
```javascript
User-Agent: PostmanRuntime/7.32.3
Accept: */*
Cache-Control: no-cache
Postman-Token: 3a776f13-f4dd-44a8-9047-ccbe56ce6b32
Host: fakerestapi.azurewebsites.net
Accept-Encoding: gzip, deflate, br
Connection: keep-alive
```
- Тело запроса: none
- Заголовки ответа:
```javascript
Content-Type: application/problem+json; charset=utf-8
Date: Thu, 22 Jun 2023 21:11:56 GMT
Server: Kestrel
Transfer-Encoding: chunked 
 ```
- Тело ответа: 
```javascript
{"type":"https://tools.ietf.org/html/rfc7231#section-6.5.1","title":"One or more validation errors occurred.","status":400,"traceId":"00-9ed86e3c9475d14dbf42f5977dffc7f5-d4ee595ec157fc4e-00","errors":{"id":["The value '2147483648' is not valid."]}}
```  

## GET​/api​/v1​/CoverPhotos​/{012} БАГ
- URL: **{{url глобал}}{{фото все глобал}}/{{012}}**
- Ожидаемый результат: статус-код ответа **404**, тест успешно пройден
- Фактический результат: статус-код ответа **200**
- Заголовки запроса: 
```javascript
User-Agent: PostmanRuntime/7.32.3
Accept: */*
Cache-Control: no-cache
Postman-Token: 032dae99-dd3d-4619-9bab-4d1aa9138662
Host: fakerestapi.azurewebsites.net
Accept-Encoding: gzip, deflate, br
Connection: keep-alive
```
- Тело запроса: none
- Заголовки ответа:
```javascript
Content-Type: application/json; charset=utf-8; v=1.0
Date: Thu, 22 Jun 2023 21:14:33 GMT
Server: Kestrel
Transfer-Encoding: chunked
api-supported-versions: 1.0 
 ```
- Тело ответа: 
```javascript
{"id":12,"idBook":12,"url":"https://placeholdit.imgix.net/~text?txtsize=33&txt=Book 12&w=250&h=350"}
```  

## GET​/api​/v1​/CoverPhotos/books/covers​​/{0} БАГ
- URL: **{{url глобал}}{{фото все глобал}}/{{обложка книги}}/{{0}}**
- Ожидаемый результат: статус-код ответа **404**, тест успешно пройден
- Фактический результат: статус-код ответа **200**
- Заголовки запроса: 
```javascript
User-Agent: PostmanRuntime/7.32.3
Accept: */*
Cache-Control: no-cache
Postman-Token: 13bc346b-781b-46f8-876b-d34cca7e8f19
Host: fakerestapi.azurewebsites.net
Accept-Encoding: gzip, deflate, br
Connection: keep-alive
```
- Тело запроса: none
- Заголовки ответа:
```javascript
Content-Type: application/json; charset=utf-8; v=1.0
Date: Thu, 22 Jun 2023 21:31:09 GMT
Server: Kestrel
Transfer-Encoding: chunked
api-supported-versions: 1.0 
 ```
- Тело ответа: 
```javascript
[]
```   

## GET​/api​/v1​/CoverPhotos/books/covers/{1}
- URL: **{{url глобал}}{{фото все глобал}}/{{обложка книги}}/{{1}}**
- Ожидаемый результат: статус-код ответа **200**, тест успешно пройден
- Заголовки запроса: 
```javascript
User-Agent: PostmanRuntime/7.32.3
Accept: */*
Cache-Control: no-cache
Postman-Token: 500c46eb-a73c-4ef2-84a4-1e9767610f27
Host: fakerestapi.azurewebsites.net
Accept-Encoding: gzip, deflate, br
Connection: keep-alive
```
- Тело запроса: none
- Заголовки ответа:
```javascript
Content-Type: application/json; charset=utf-8; v=1.0
Date: Thu, 22 Jun 2023 21:34:35 GMT
Server: Kestrel
Transfer-Encoding: chunked
api-supported-versions: 1.0 
 ```
- Тело ответа: 
```javascript
[{"id":1,"idBook":1,"url":"https://placeholdit.imgix.net/~text?txtsize=33&txt=Book 1&w=250&h=350"}]
```    

## GET​/api​/v1​/CoverPhotos/books/covers​/{201} БАГ
URL: **{{url глобал}}{{фото все глобал}}/{{обложка книги}}/{{201}}** 
- Ожидаемый результат: статус-код ответа **404**, тест успешно пройден
- Фактический результат: статус-код ответа **200**
- Заголовки запроса: 
```javascript
User-Agent: PostmanRuntime/7.32.3
Accept: */*
Cache-Control: no-cache
Postman-Token: 3367b0eb-a0ee-4c2a-ba13-190287f2e5df
Host: fakerestapi.azurewebsites.net
Accept-Encoding: gzip, deflate, br
Connection: keep-alive
```
- Тело запроса: none
- Заголовки ответа:
```javascript
Content-Type: application/json; charset=utf-8; v=1.0
Date: Thu, 22 Jun 2023 21:37:33 GMT
Server: Kestrel
Transfer-Encoding: chunked
api-supported-versions: 1.0 
 ```
- Тело ответа: 
```javascript
[]
```   

## GET​/api​/v1​/CoverPhotos/books/covers​​/{2147483648}
- URL: **{{url глобал}}{{фото все глобал}}/{{обложка книги}}/{{>int 32}}**
- Ожидаемый результат: статус-код ответа **400**, тест успешно пройден
- Заголовки запроса: 
```javascript
User-Agent: PostmanRuntime/7.32.3
Accept: */*
Cache-Control: no-cache
Postman-Token: fde5a199-7ce5-4ef9-abb5-a3f8fe088ed2
Host: fakerestapi.azurewebsites.net
Accept-Encoding: gzip, deflate, br
Connection: keep-alive
```
- Тело запроса: none
- Заголовки ответа:
```javascript
Content-Type: application/problem+json; charset=utf-8
Date: Thu, 22 Jun 2023 21:38:58 GMT
Server: Kestrel
Transfer-Encoding: chunked 
 ```
- Тело ответа: 
```javascript
{"type":"https://tools.ietf.org/html/rfc7231#section-6.5.1","title":"One or more validation errors occurred.","status":400,"traceId":"00-660321dc4e1463419c13c2c7737cf379-2fab0baa0a1ddf43-00","errors":{"idBook":["The value '2147483648' is not valid."]}}
```    

## GET​/api​/v1​/CoverPhotos/books/covers​​/​/{012} БАГ
- URL: **{{url глобал}}{{фото все глобал}}/{{обложка книги}}/{{012}}**
- Ожидаемый результат: статус-код ответа **404**, тест успешно пройден
- Фактический результат: статус-код ответа **200** 
- Заголовки запроса: 
```javascript
User-Agent: PostmanRuntime/7.32.3
Accept: */*
Cache-Control: no-cache
Postman-Token: c65aa020-cae3-423f-813a-0e8ec77a2c73
Host: fakerestapi.azurewebsites.net
Accept-Encoding: gzip, deflate, br
Connection: keep-alive
```
- Тело запроса: none
- Заголовки ответа:
```javascript
Content-Type: application/json; charset=utf-8; v=1.0
Date: Thu, 22 Jun 2023 21:42:38 GMT
Server: Kestrel
Transfer-Encoding: chunked
api-supported-versions: 1.0 
 ```
- Тело ответа: 
```javascript
[{"id":12,"idBook":12,"url":"https://placeholdit.imgix.net/~text?txtsize=33&txt=Book 12&w=250&h=350"}]
```    

## GET​/api​/v1​/Users​
- URL: **{{url глобал}}{{юзеры все глобал}}**
- Ожидаемый результат: статус-код ответа **200**, тест успешно пройден
- Заголовки запроса: 
```javascript
User-Agent: PostmanRuntime/7.32.3
Accept: */*
Cache-Control: no-cache
Postman-Token: d334e223-3847-471d-90ca-f45cc76b7ae2
Host: fakerestapi.azurewebsites.net
Accept-Encoding: gzip, deflate, br
Connection: keep-alive
```
- Тело запроса: none
- Заголовки ответа:
```javascript
Content-Type: application/json; charset=utf-8; v=1.0
Date: Thu, 22 Jun 2023 21:44:12 GMT
Server: Kestrel
Transfer-Encoding: chunked
api-supported-versions: 1.0 
 ```
- Тело ответа: 
```javascript
Content-Type: application/json; charset=utf-8; v=1.0
Date: Thu, 22 Jun 2023 21:44:12 GMT
Server: Kestrel
Transfer-Encoding: chunked
api-supported-versions: 1.0
```     

## GET​/api​/v1​/Users​/{0}
- URL: **{{url глобал}}{{юзеры все глобал}}/{{0}}**
- Ожидаемый результат: статус-код ответа **404**, тест успешно пройден
- Заголовки запроса: 
```javascript
User-Agent: PostmanRuntime/7.32.3
Accept: */*
Cache-Control: no-cache
Postman-Token: 8db35033-e09c-4a4d-9cc6-5eed6be1bfeb
Host: fakerestapi.azurewebsites.net
Accept-Encoding: gzip, deflate, br
Connection: keep-alive
```
- Тело запроса: none
- Заголовки ответа:
```javascript
Content-Type: application/problem+json; charset=utf-8; v=1.0
Date: Thu, 22 Jun 2023 21:45:44 GMT
Server: Kestrel
Transfer-Encoding: chunked
api-supported-versions: 1.0 
 ```
- Тело ответа: 
```javascript
{"type":"https://tools.ietf.org/html/rfc7231#section-6.5.4","title":"Not Found","status":404,"traceId":"00-23cdda139c968d4c9ad3906aec1b5884-f027449fb9a1b843-00"}
```     

## GET​/api​/v1​/Users​/{1}
- URL: **{{url глобал}}{{юзеры все глобал}}/{{1}}**
- Ожидаемый результат: статус-код ответа **200**, тест успешно пройден
- Заголовки запроса: 
```javascript
User-Agent: PostmanRuntime/7.32.3
Accept: */*
Cache-Control: no-cache
Postman-Token: fb54f0b1-af1c-47b4-9ea6-7ae4c6dbb11b
Host: fakerestapi.azurewebsites.net
Accept-Encoding: gzip, deflate, br
Connection: keep-alive
```
- Тело запроса: none
- Заголовки ответа:
```javascript
Content-Type: application/json; charset=utf-8; v=1.0
Date: Thu, 22 Jun 2023 21:47:22 GMT
Server: Kestrel
Transfer-Encoding: chunked
api-supported-versions: 1.0 
 ```
- Тело ответа: 
```javascript
{"id":1,"userName":"User 1","password":"Password1"}
```   

## GET​/api​/v1​/Users​/{11}
- URL: **{{url глобал}}{{юзеры все глобал}}/{{11}}**
- Ожидаемый результат: статус-код ответа **404**, тест успешно пройден
- Заголовки запроса: 
```javascript
User-Agent: PostmanRuntime/7.32.3
Accept: */*
Cache-Control: no-cache
Postman-Token: 9a125b91-c00b-42b6-88f5-3fff0bdb8c57
Host: fakerestapi.azurewebsites.net
Accept-Encoding: gzip, deflate, br
Connection: keep-alive
```
- Тело запроса: none
- Заголовки ответа:
```javascript
Content-Type: application/problem+json; charset=utf-8; v=1.0
Date: Thu, 22 Jun 2023 21:48:42 GMT
Server: Kestrel
Transfer-Encoding: chunked
api-supported-versions: 1.0 
 ```
- Тело ответа: 
```javascript
{"type":"https://tools.ietf.org/html/rfc7231#section-6.5.4","title":"Not Found","status":404,"traceId":"00-66f32e676f27e24b91a0d0ff2e488ad7-5ca3f6d803d9a54b-00"}
```    

## GET​/api​/v1​/Users​/{2147483648}
- URL: **{{url глобал}}{{юзеры все глобал}}/{{>int 32}}**
- Ожидаемый результат: статус-код ответа **400**, тест успешно пройден
- Заголовки запроса: 
```javascript
User-Agent: PostmanRuntime/7.32.3
Accept: */*
Cache-Control: no-cache
Postman-Token: 001084ab-fb0d-41cb-9fbe-69288749c712
Host: fakerestapi.azurewebsites.net
Accept-Encoding: gzip, deflate, br
Connection: keep-alive
```
- Тело запроса: none
- Заголовки ответа:
```javascript
Content-Type: application/problem+json; charset=utf-8
Date: Thu, 22 Jun 2023 21:50:03 GMT
Server: Kestrel
Transfer-Encoding: chunked 
 ```
- Тело ответа: 
```javascript
{"type":"https://tools.ietf.org/html/rfc7231#section-6.5.1","title":"One or more validation errors occurred.","status":400,"traceId":"00-7daec3e60a25e74a82af6aad229478c3-b406db0cac265146-00","errors":{"id":["The value '2147483648' is not valid."]}}
```