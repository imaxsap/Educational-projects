## 1. GET api​/v1​/Activities
   * HTTP-метод: **GET**
   * Полный URL запроса: https://fakerestapi.azurewebsites.net/api/v1/Activities
   * Заголовки запроса:**-H  "accept: text/plain; v=1.0"**
   * Тело запроса (при наличии):
   * Статус-код ответа: **200**
   * Тело ответа (при наличии):
   ```Java Script
[
  {
    "id": 1,
    "title": "Activity 1",
    "dueDate": "2023-06-13T13:12:01.2720476+00:00",
    "completed": false
  },
  {
    "id": 30,
    "title": "Activity 30",
    "dueDate": "2023-06-14T18:12:01.2720584+00:00",
    "completed": true
  }
]
   ```

## 2. POST ​/api​/v1​/Activities
   * HTTP-метод: **POST**
   * Полный URL запроса: https://fakerestapi.azurewebsites.net/api/v1/Activities
   * Заголовки запроса: **-H  "Content-Type: application/json; v=1.0"**
   * Тело запроса (при наличии):
   * Статус-код ответа: **200**
   * Тело ответа (при наличии):
  ```Java Script
{
  "id": 0,
  "title": "string",
  "dueDate": "2023-06-13T12:16:16.644Z",
  "completed": true
}
   ```
   
   ## 3 GET ​/api​/v1​/Activities/28
   * HTTP-метод: **GET**
   * Полный URL запроса: https://fakerestapi.azurewebsites.net/api/v1/Activities/28
   * Заголовки запроса:**-H  "accept: text/plain; v=1.0"**
   * Тело запроса (при наличии):
   * Статус-код ответа: **200**
   * Тело ответа (при наличии):
```javascript
{
  "id": 28,
  "title": "Activity 28",
  "dueDate": "2023-06-14T16:52:28.712071+00:00",
  "completed": true
}
```

   ## 4. GET ​/api​/v1​/Activities/777
   * HTTP-метод: **GET**
   * Полный URL запроса: https://fakerestapi.azurewebsites.net/api/v1/Activities/777
   * Заголовки запроса: **-H  "accept: text/plain; v=1.0"**
   * Тело запроса (при наличии):
   * Статус-код ответа: **404**
   * Тело ответа (при наличии):
```Java Script
{
  "type": "https://tools.ietf.org/html/rfc7231#section-6.5.4",
  "title": "Not Found",
  "status": 404,
  "traceId": "00-bad3884c46508c428c95071a7f4bce2f-da0461a25975c840-00"
}
```
   
## 5. PUT ​/api​/v1​/Activities​/636
   * HTTP-метод: **PUT**
   * Полный URL запроса: https://fakerestapi.azurewebsites.net/api/v1/Activities/636
   * Заголовки запроса: **-H "Content-Type: application/json; v=1.0"**
   * Тело запроса (при наличии):
   * Статус-код ответа: **200**
   * Тело ответа (при наличии):
```Java Script
{
  "id": 0,
  "title": "string",
  "dueDate": "2023-06-13T13:15:43.85Z",
  "completed": true
}
```

## 6. PUT ​/api​/v1​/Activities​/89801234567890
   * HTTP-метод: **PUT**
   * Полный URL запроса: https://fakerestapi.azurewebsites.net/api/v1/Activities/89801234567890
   * Заголовки запроса: **-H  "Content-Type: application/json; v=1.0"**
   * Тело запроса (при наличии):
   * Статус-код ответа: **400**
   * Тело ответа (при наличии):
  ```Java Script
{
  "type": "https://tools.ietf.org/html/rfc7231#section-6.5.1",
  "title": "One or more validation errors occurred.",
  "status": 400,
  "traceId": "00-faf6630db59596489b4a6096590274d5-37cfdb640446ec4a-00",
  "errors": {
    "id": [
      "The value '89801234567890' is not valid."
    ]
  }
}
   ```
   
   ## 7. DELETE api​/v1​/Activities​/330
   * HTTP-метод: **DELETE**
   * Полный URL запроса: https://fakerestapi.azurewebsites.net/api/v1/Activities/330
   * Заголовки запроса: **-H  "accept: /"**
   * Тело запроса (при наличии):
   * Статус-код ответа: **200**
   * Тело ответа (при наличии):
  

   ## 8. DELETE api​/v1​/Activities​/89781001010111
   * HTTP-метод: **DELETE**
   * Полный URL запроса: https://fakerestapi.azurewebsites.net/api/v1/Activities/89781001010111
   * Заголовки запроса: **-H  "accept: /"**
   * Тело запроса (при наличии):
   * Статус-код ответа: **400**
   * Тело ответа (при наличии):
  ```Java Script
{
  "type": "https://tools.ietf.org/html/rfc7231#section-6.5.1",
  "title": "One or more validation errors occurred.",
  "status": 400,
  "traceId": "00-79b823704c18be40b547f56d23a148b8-54f6725c8ebce342-00",
  "errors": {
    "id": [
      "The value '89781001010111' is not valid."
    ]
  }
}
   ```
   
   ## 9. GET ​/api​/v1​/Authors
   * HTTP-метод: **GET**
   * Полный URL запроса: https://fakerestapi.azurewebsites.net/api/v1/Authors
   * Заголовки запроса: **-H  "accept: text/plain; v=1.0"**
   * Тело запроса (при наличии):
   * Статус-код ответа: **200**
   * Тело ответа (при наличии):
   ```Java Script
[
  {
    "id": 1,
    "idBook": 1,
    "firstName": "First Name 1",
    "lastName": "Last Name 1"
  },
  {
    "id": 602,
    "idBook": 200,
    "firstName": "First Name 602",
    "lastName": "Last Name 602"
  }
]
   ```

   ## 10. POST ​/api​/v1​/Authors
   * HTTP-метод: **POST**
   * Полный URL запроса: https://fakerestapi.azurewebsites.net/api/v1/Authors
   * Заголовки запроса: **-H  "Content-Type: application/json; v=1.0" -d "**
   * Тело запроса (при наличии):
   * Статус-код ответа: **200**
   * Тело ответа (при наличии):
  ```Java Script
{
  "id": 0,
  "idBook": 0,
  "firstName": "string",
  "lastName": "string"
}
   ```
   
   ## 11. GET ​/api​/v1​/Authors​/authors​/books​/92
   * HTTP-метод: **GET**
   * Полный URL запроса: https://fakerestapi.azurewebsites.net/api/v1/Authors/authors/books/92
   * Заголовки запроса: **H  "accept: text/plain; v=1.0"**
   * Тело запроса (при наличии):
   * Статус-код ответа: **200**
   * Тело ответа (при наличии):
   ```Java Script
[
  {
    "id": 265,
    "idBook": 92,
    "firstName": "First Name 265",
    "lastName": "Last Name 265"
  },
  {
    "id": 268,
    "idBook": 92,
    "firstName": "First Name 268",
    "lastName": "Last Name 268"
  }
]
   ```

   ## 12. GET ​/api​/v1​/Authors​/authors​/books​/12345678910
   * HTTP-метод: **GET**
   * Полный URL запроса: https://fakerestapi.azurewebsites.net/api/v1/Authors/authors/books/12345678910
   * Заголовки запроса: **-H  "accept: text/plain; v=1.0"**
   * Тело запроса (при наличии):
   * Статус-код ответа: **400**
   * Тело ответа (при наличии):
  ```Java Script
{
  "type": "https://tools.ietf.org/html/rfc7231#section-6.5.1",
  "title": "One or more validation errors occurred.",
  "status": 400,
  "traceId": "00-5d78e199344f0c4e8cad2e532f40ec57-134b0e9fd50be74a-00",
  "errors": {
    "idBook": [
      "The value '12345678910' is not valid."
    ]
  }
}
   ```
   
   ## 13. GET ​/api​/v1​/Authors​/21
   * HTTP-метод: **GET**
   * Полный URL запроса: https://fakerestapi.azurewebsites.net/api/v1/Authors/21
   * Заголовки запроса: **-H  "accept: text/plain; v=1.0"**
   * Тело запроса (при наличии):
   * Статус-код ответа: **200**
   * Тело ответа (при наличии):
   ```Java Script
{
  "id": 21,
  "idBook": 7,
  "firstName": "First Name 21",
  "lastName": "Last Name 21"
}
   ```

   ## 14. GET ​/api​/v1​/Authors​/888
   * HTTP-метод: **GET**
   * Полный URL запроса: https://fakerestapi.azurewebsites.net/api/v1/Authors/888
   * Заголовки запроса: **-H  "accept: text/plain; v=1.0"**
   * Тело запроса (при наличии):
   * Статус-код ответа: **404**
   * Тело ответа (при наличии):
  ```Java Script
{
  "type": "https://tools.ietf.org/html/rfc7231#section-6.5.4",
  "title": "Not Found",
  "status": 404,
  "traceId": "00-552faa681a4969429ea59f03845a1520-b6884f83a3c1cd40-00"
}
   ```
   
   ## 15. PUT ​/api​/v1​/Authors​/43
   * HTTP-метод: **PUT**
   * Полный URL запроса: https://fakerestapi.azurewebsites.net/api/v1/Authors/43
   * Заголовки запроса: **-H  "Content-Type: application/json; v=1.0"**
   * Тело запроса (при наличии):
   * Статус-код ответа: **200**
   * Тело ответа (при наличии):
   ```Java Script
{
  "id": 0,
  "idBook": 0,
  "firstName": "string",
  "lastName": "string"
}
   ```

   ## 16. PUT ​/api​/v1​/Authors​/10987654321
   * HTTP-метод: **PUT**
   * Полный URL запроса: https://fakerestapi.azurewebsites.net/api/v1/Authors/10987654321
   * Заголовки запроса: **-H  "Content-Type: application/json; v=1.0"**
   * Тело запроса (при наличии):
   ```Java Script
   {
  "id": 0,
  "idBook": 0,
  "firstName": "string",
  "lastName": "string"
}
```
   * Статус-код ответа: **400**
   * Тело ответа (при наличии):
  ```Java Script
{
  "type": "https://tools.ietf.org/html/rfc7231#section-6.5.1",
  "title": "One or more validation errors occurred.",
  "status": 400,
  "traceId": "00-9665af750a873745ab0d73405ea10bf0-f10ae75af890de46-00",
  "errors": {
    "id": [
      "The value '10987654321' is not valid."
    ]
  }
}
   ```
   
   ## 17. DELETE ​/api​/v1​/Authors​/121
   * HTTP-метод: **DELETE**
   * Полный URL запроса: https://fakerestapi.azurewebsites.net/api/v1/Authors/121
   * Заголовки запроса: **-H  "accept: /"**
   * Тело запроса (при наличии):
   * Статус-код ответа: **200**
   * Тело ответа (при наличии):
   ```Java Script

   ```

## 18. DELETE ​/api​/v1​/Authors​/111222333444
   * HTTP-метод: **DELETE**
   * Полный URL запроса: https://fakerestapi.azurewebsites.net/api/v1/Authors/111222333444
   * Заголовки запроса: **-H  "accept: */*"**
   * Тело запроса (при наличии): 
   * Статус-код ответа: **400**
   * Тело ответа (при наличии):
```Java Script
{
  "type": "https://tools.ietf.org/html/rfc7231#section-6.5.1",
  "title": "One or more validation errors occurred.",
  "status": 400,
  "traceId": "00-f382dd0548aa154a8058c2b26beafd09-130a24617dc8c24e-00",
  "errors": {
    "id": [
      "The value '111222333444' is not valid."
    ]
  }
}
```

   ## 19. GET ​/api​/v1​/Books
   * HTTP-метод: **GET**
   * Полный URL запроса: https://fakerestapi.azurewebsites.net/api/v1/Books
   * Заголовки запроса: **-H  "accept: text/plain; v=1.0"**
   * Тело запроса (при наличии): 
   * Статус-код ответа: **200**
   * Тело ответа (при наличии): 
   ```Java Script
  {
    "id": 1,
    "title": "Book 1",
    "description": "Lorem lorem lorem. Lorem lorem lorem. 
    Lorem lorem lorem.\n",
    "pageCount": 100,
    "excerpt": "Lorem lorem lorem. Lorem lorem lorem.
    Lorem lorem lorem.\nLorem lorem lorem. Lorem lorem lorem. 
    Lorem lorem lorem.\nLorem lorem lorem. Lorem lorem lorem. 
    Lorem lorem lorem.\nLorem lorem lorem. Lorem lorem lorem. 
    Lorem lorem lorem.\nLorem lorem lorem. Lorem lorem lorem. 
    Lorem lorem lorem.\n",
    "publishDate": "2023-06-12T17:29:22.263389+00:00"
  }
   ```

   ## 20. POST ​/api​/v1​/Books
   * HTTP-метод: **POST**
   * Полный URL запроса: https://fakerestapi.azurewebsites.net/api/v1/Books
   * Заголовки запроса: **-H  "Content-Type: application/json; v=1.0"**
   * Тело запроса (при наличии): 
   * Статус-код ответа: **200**
   * Тело ответа (при наличии): 
  ```Java Script
{
  "id": 0,
  "title": "string",
  "description": "string",
  "pageCount": 0,
  "excerpt": "string",
  "publishDate": "2023-06-13T17:38:29.741Z"
}
   ```
   
   ## 21. GET ​/api​/v1​/Books​/93
   * HTTP-метод: **GET**
   * Полный URL запроса: https://fakerestapi.azurewebsites.net/api/v1/Books/93
   * Заголовки запроса: **-H  "accept: text/plain; v=1.0"**
   * Тело запроса (при наличии):
   * Статус-код ответа: **200**
   * Тело ответа (при наличии):
   ```Java Script
{
    "id": 93,
    "title": "Book 93",
    "description": "Lorem lorem lorem. Lorem lorem lorem. 
Lorem lorem lorem.\n",
    "pageCount": 9300,
    "excerpt": "Lorem lorem lorem. Lorem lorem lorem. 
Lorem lorem lorem.\nLorem lorem lorem. Lorem lorem lorem. 
Lorem lorem lorem.\nLorem lorem lorem. Lorem lorem lorem. 
Lorem lorem lorem.\nLorem lorem lorem. Lorem lorem lorem. 
Lorem lorem lorem.\nLorem lorem lorem. Lorem lorem lorem. 
Lorem lorem lorem.\n",
  "publishDate": "2023-03-12T17:41:57.1343778+00:00"
}
   ```

   ## 22. GET ​/api​/v1​/Books​/559
   * HTTP-метод: **GET**
   * Полный URL запроса: https://fakerestapi.azurewebsites.net/api/v1/Books/559
   * Заголовки запроса: **-H  "accept: text/plain; v=1.0"**
   * Тело запроса (при наличии): 
   * Статус-код ответа: **404**
   * Тело ответа (при наличии): 
  ```Java Script
{
  "type": "https://tools.ietf.org/html/rfc7231#section-6.5.4",
  "title": "Not Found",
  "status": 404,
  "traceId": "00-9cfed99fe475a14797c455c3cd5bd009-9e9205b19e239645-00"
}
   ```
   
   ## 23. PUT ​/api​/v1​/Books​/57
   * HTTP-метод: **PUT**
   * Полный URL запроса: https://fakerestapi.azurewebsites.net/api/v1/Books/57
   * Заголовки запроса: **-H  "Content-Type: application/json; v=1.0"**
   * Тело запроса (при наличии):
   * Статус-код ответа: **200**
   * Тело ответа (при наличии):
   ```Java Script
{
  "id": 0,
  "title": "string",
  "description": "string",
  "pageCount": 0,
  "excerpt": "string",
  "publishDate": "2023-06-13T17:56:58.226Z"
}
   ```

   ## 24. PUT ​/api​/v1​/Books​/130620232059
   * HTTP-метод: **PUT**
   * Полный URL запроса: https://fakerestapi.azurewebsites.net/api/v1/Books/130620232059
   * Заголовки запроса: **-H  "Content-Type: application/json; v=1.0"**
   * Тело запроса (при наличии):
   * Статус-код ответа: **400**
   * Тело ответа (при наличии):
  ```Java Script
{
  "type": "https://tools.ietf.org/html/rfc7231#section-6.5.1",
  "title": "One or more validation errors occurred.",
  "status": 400,
  "traceId": "00-3f91728270018d459b041f4fe62fe6a1-0fc035b107c56a43-00",
  "errors": {
    "id": [
      "The value '130620232059' is not valid."
    ]
  }
}
   ```
   
   ## 25. DELETE​/api​/v1​/Books​/33
   * HTTP-метод: **DELETE**
   * Полный URL запроса: https://fakerestapi.azurewebsites.net/api/v1/Books/33
   * Заголовки запроса: **-H  "accept: /"**
   * Тело запроса (при наличии):
   * Статус-код ответа: **200**
   * Тело ответа (при наличии):

   ## 26. DELETE​/api​/v1​/Books​/200120022003
   * HTTP-метод: **DELETE**
   * Полный URL запроса: https://fakerestapi.azurewebsites.net/api/v1/Books/200120022003
   * Заголовки запроса: **-H  "accept: /"**
   * Тело запроса (при наличии):
   * Статус-код ответа: **400**
   * Тело ответа (при наличии):
  ```Java Script
{
"type": "https://tools.ietf.org/html/rfc7231#section-6.5.1",
  "title": "One or more validation errors occurred.",
  "status": 400,
  "traceId": "00-0ef561ee4e7b434a870e5e070c6539f8-d798b9b6e2ab464d-00",
  "errors": {
    "id": [
      "The value '200120022003' is not valid."
    ]
  }
}
   ```
   
   ## 27. GET ​/api​/v1​/CoverPhotos
   * HTTP-метод: **GET**
   * Полный URL запроса: https://fakerestapi.azurewebsites.net/api/v1/CoverPhotos
   * Заголовки запроса: **-H  "accept: text/plain; v=1.0"**
   * Тело запроса (при наличии):
   * Статус-код ответа: **200**
   * Тело ответа (при наличии):
  ```Java Script
[
  {
    "id": 1,
    "idBook": 1,
    "url": "https://placeholdit.imgix.net/~text?txtsize=33&txt=Book 1&w=250&h=350"
  },
  {
    "id": 200,
    "idBook": 200,
    "url": "https://placeholdit.imgix.net/~text?txtsize=33&txt=Book 200&w=250&h=350"
  }
]
   ```

   ## 28. POST ​/api​/v1​/CoverPhotos
   * HTTP-метод: **POST**
   * Полный URL запроса: https://fakerestapi.azurewebsites.net/api/v1/CoverPhotos
   * Заголовки запроса: **-H  "Content-Type: application/json; v=1.0"**
   * Тело запроса (при наличии):
   * Статус-код ответа: **200**
   * Тело ответа (при наличии):
   ```Java Script
{
  "id": 0,
  "idBook": 0,
  "url": "string"
}
   ```
   
   ## 29. GET ​/api​/v1​/CoverPhotos​/books​/covers​/195
   * HTTP-метод: **GET**
   * Полный URL запроса: https://fakerestapi.azurewebsites.net/api/v1/CoverPhotos/books/covers/195
   * Заголовки запроса: **-H  "accept: text/plain; v=1.0"**
   * Тело запроса (при наличии):
   * Статус-код ответа: **200**
   * Тело ответа (при наличии):
   ```Java Script
[
  {
    "id": 195,
    "idBook": 195,
    "url": "https://placeholdit.imgix.net/~text?txtsize=33&txt=Book 195&w=250&h=350"
  }
]
   ```

   ## 30. GET ​/api​/v1​/CoverPhotos​/books​/covers​/3214569871
   * HTTP-метод: **GET**
   * Полный URL запроса: https://fakerestapi.azurewebsites.net/api/v1/CoverPhotos/books/covers/3214569871
   * Заголовки запроса: **-H  "accept: text/plain; v=1.0"**
   * Тело запроса (при наличии):
   * Статус-код ответа: **400**
   * Тело ответа (при наличии):
  ```Java Script
{
  "type": "https://tools.ietf.org/html/rfc7231#section-6.5.1",
  "title": "One or more validation errors occurred.",
  "status": 400,
  "traceId": "00-5fcdd8b81a26364ca6815675694f5953-759e30197f39214d-00",
  "errors": {
    "idBook": [
      "The value '3214569871' is not valid."
    ]
  }
}
   ```
   
   ## 31. GET ​/api​/v1​/CoverPhotos​/111
   * HTTP-метод: **GET**
   * Полный URL запроса: https://fakerestapi.azurewebsites.net/api/v1/CoverPhotos/111
   * Заголовки запроса: **-H  "accept: text/plain; v=1.0"**
   * Тело запроса (при наличии):
   * Статус-код ответа: **200**
   * Тело ответа (при наличии):
   ```Java Script
{
  "id": 111,
  "idBook": 111,
  "url": "https://placeholdit.imgix.net/~text?txtsize=33&txt=Book 111&w=250&h=350"
}
   ```

   ## 32. GET ​/api​/v1​/CoverPhotos​/808
   * HTTP-метод: **GET**
   * Полный URL запроса: https://fakerestapi.azurewebsites.net/api/v1/CoverPhotos/808
   * Заголовки запроса: **-H  "accept: text/plain; v=1.0"**
   * Тело запроса (при наличии):
   * Статус-код ответа: **404**
   * Тело ответа (при наличии):
  ```Java Script
{
  "type": "https://tools.ietf.org/html/rfc7231#section-6.5.4",
  "title": "Not Found",
  "status": 404,
  "traceId": "00-7d0f9e33e549fb4fa0f084df3f3a2f5c-840fa8cfd8660748-00"
}
   ```
   
   ## 33. PUT ​/api​/v1​/CoverPhotos​/99
   * HTTP-метод: **PUT**
   * Полный URL запроса: https://fakerestapi.azurewebsites.net/api/v1/CoverPhotos/99
   * Заголовки запроса: **-H  "Content-Type: application/json; v=1.0"**
   * Тело запроса (при наличии):
   * Статус-код ответа: **200**
   * Тело ответа (при наличии):
   ```Java Script
{
  "id": 0,
  "idBook": 0,
  "url": "string"
}
   ```

   ## 34. PUT ​/api​/v1​/CoverPhotos​/202320242025
   * HTTP-метод: **PUT**
   * Полный URL запроса: https://fakerestapi.azurewebsites.net/api/v1/CoverPhotos/202320242025
   * Заголовки запроса: **-H  "Content-Type: application/json; v=1.0"**
   * Тело запроса (при наличии):
   * Статус-код ответа: **400**
   * Тело ответа (при наличии):
  ```Java Script
{
  "type": "https://tools.ietf.org/html/rfc7231#section-6.5.1",
  "title": "One or more validation errors occurred.",
  "status": 400,
  "traceId": "00-6a5cd256a072244ca3964dc89f8d5c26-139826581e886d49-00",
  "errors": {
    "id": [
      "The value '202320242025' is not valid."
    ]
  }
}
   ```
   
   ## 35. DELETE ​/api​/v1​/CoverPhotos​/999
   * HTTP-метод: **DELETE**
   * Полный URL запроса: https://fakerestapi.azurewebsites.net/api/v1/CoverPhotos/999
   * Заголовки запроса: **-H  "accept: /"**
   * Тело запроса (при наличии):
   * Статус-код ответа: **200**
   * Тело ответа (при наличии):

   ## 36. DELETE ​/api​/v1​/CoverPhotos​/160620231147
   * HTTP-метод: **DELETE**
   * Полный URL запроса: https://fakerestapi.azurewebsites.net/api/v1/CoverPhotos/160620231147
   * Заголовки запроса: **-H  "accept: /"**
   * Тело запроса (при наличии):
   * Статус-код ответа: **400**
   * Тело ответа (при наличии):
  ```Java Script
{
  "type": "https://tools.ietf.org/html/rfc7231#section-6.5.1",
  "title": "One or more validation errors occurred.",
  "status": 400,
  "traceId": "00-cdddd0062cfcd44eb317d5df8ee1cefb-d236f8585b937346-00",
  "errors": {
    "id": [
      "The value '160620231147' is not valid."
    ]
  }
}
   ```
   
   ## 37. GET ​/api​/v1​/Users
   * HTTP-метод: **GET**
   * Полный URL запроса: https://fakerestapi.azurewebsites.net/api/v1/Users
   * Заголовки запроса: **-H  "accept: text/plain; v=1.0"**
   * Тело запроса (при наличии):
   * Статус-код ответа: **200**
   * Тело ответа (при наличии):
   ```Java Script
[
  {
    "id": 1,
    "userName": "User 1",
    "password": "Password1"
  },
  {
    "id": 10,
    "userName": "User 10",
    "password": "Password10"
  }
]
   ```

   ## 38. POST ​/api​/v1​/Users
   * HTTP-метод: **POST**
   * Полный URL запроса: https://fakerestapi.azurewebsites.net/api/v1/Users
   * Заголовки запроса: **-H  "Content-Type: application/json; v=1.0"**
   * Тело запроса (при наличии):
   * Статус-код ответа: **200**
   * Тело ответа (при наличии):
  ```Java Script
{
  "id": 0,
  "userName": "string",
  "password": "string"
}
   ```
   
   ## 39. GET ​/api​/v1​/Users​/5
   * HTTP-метод: **GET**
   * Полный URL запроса: https://fakerestapi.azurewebsites.net/api/v1/Users/5
   * Заголовки запроса: **-H  "accept: /"**
   * Тело запроса (при наличии):
   * Статус-код ответа: **200**
   * Тело ответа (при наличии):
   ```Java Script
{
  "id": 5,
  "userName": "User 5",
  "password": "Password5"
}
   ```

   ## 40. GET ​/api​/v1​/Users​/264
   * HTTP-метод: **GET**
   * Полный URL запроса: https://fakerestapi.azurewebsites.net/api/v1/Users/264
   * Заголовки запроса: **-H  "accept: /"**
   * Тело запроса (при наличии):
   * Статус-код ответа: **404**
   * Тело ответа (при наличии):
  ```Java Script
{
  "type": "https://tools.ietf.org/html/rfc7231#section-6.5.4",
  "title": "Not Found",
  "status": 404,
  "traceId": "00-bf7ca3e128964c4594d665a24ffe4c9e-41df7d8c71c63d45-00"
}
   ```
   
   ## 41. GET ​/api​/v1​/Users​/951357852654
   * HTTP-метод: **GET**
   * Полный URL запроса:https://fakerestapi.azurewebsites.net/api/v1/Users/951357852654
   * Заголовки запроса: **-H  "accept: /"**
   * Тело запроса (при наличии):
   * Статус-код ответа: **400**
   * Тело ответа (при наличии):
   ```Java Script
{
  "type": "https://tools.ietf.org/html/rfc7231#section-6.5.1",
  "title": "One or more validation errors occurred.",
  "status": 400,
  "traceId": "00-7fabc09d13c3fd4ab62aab4f5e36a2df-481ea616b0062e4e-00",
  "errors": {
    "id": [
      "The value '951357852654' is not valid."
    ]
  }
}
   ```

   ## 42. PUT ​/api​/v1​/Users​/27
   * HTTP-метод: **PUT**
   * Полный URL запроса: https://fakerestapi.azurewebsites.net/api/v1/Users/27
   * Заголовки запроса: **-H  "Content-Type: application/json; v=1.0" -d "**
   * Тело запроса (при наличии):
   * Статус-код ответа: **200**
   * Тело ответа (при наличии):
  ```Java Script
{
  "id": 0,
  "userName": "string",
  "password": "string"
}
   ```
   
   ## 43. PUT ​/api​/v1​/Users​/43
   * HTTP-метод: **PUT**
   * Полный URL запроса: https://fakerestapi.azurewebsites.net/api/v1/Users/135406162023
   * Заголовки запроса: **-H  "Content-Type: application/json; v=1.0" -d "**
   * Тело запроса (при наличии):
   * Статус-код ответа: **400**
   * Тело ответа (при наличии):
   ```Java Script
{
  "type": "https://tools.ietf.org/html/rfc7231#section-6.5.1",
  "title": "One or more validation errors occurred.",
  "status": 400,
  "traceId": "00-69c125da7ab8de4bb8f92d6c0379ab40-0e09b8947d6d0d49-00",
  "errors": {
    "id": [
      "The value '135406162023' is not valid."
    ]
  }
}
   ```

   ## 44. DELETE ​/api​/v1​/Users​/22
   * HTTP-метод: **DELETE**
   * Полный URL запроса: https://fakerestapi.azurewebsites.net/api/v1/Users/22
   * Заголовки запроса: **-H  "accept: /"**
   * Тело запроса (при наличии):
   * Статус-код ответа: **200**
   * Тело ответа (при наличии):
   
   ## 45. DELETE ​/api​/v1​/Users​/2221232524
   * HTTP-метод: **DELETE**
   * Полный URL запроса: https://fakerestapi.azurewebsites.net/api/v1/Users/2221232524
   * Заголовки запроса: **-H  "accept: /"**
   * Тело запроса (при наличии):
   * Статус-код ответа: **400**
   * Тело ответа (при наличии):
   ```Java Script
{
  "type": "https://tools.ietf.org/html/rfc7231#section-6.5.1",
  "title": "One or more validation errors occurred.",
  "status": 400,
  "traceId": "00-1496d9fae5fa2e4881caed8b9ca9f649-48dbe8f2f8e5a140-00",
  "errors": {
    "id": [
      "The value '2221232524' is not valid."
    ]
  }
}
   ```
---
