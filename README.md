## Status Code

- 1XX : informational
  - 100: Continue
  - 102: Processing
- 2XX : Successful
  - 200: OK
  - 201: Created
  - 204: No Content
- 3XX : Redirection
  - 301: Moved Permanently
  - 302: Found
  - 303: See Other(get)
  - 307: Temporary Redirect(same methods)
  - 308: Permanent Redirect(same methods)
- 4XX : Client error
  - 400: Bad Request (쿼리,api 문제)
  - 401: Unauthorized
  - 403: Forbidden(admin)
  - 404: Not Found
  - 405: Method Not Allowed
  - 409: Conflict
- 5XX : Server error
  - 500: Internal Server Error
  - 502: Bad Gateway
  - 503: Service Unavailable

## Request Methods

- Kind of methods
  - GET: get (200, 401, 403, 404, 405)
  - POST: create (401, 403, 404, 409)
  - PUT: replace (200, 204, 403, 404, 405)
  - DELETE: delete ()
  - PATCH: replace partially ()
  - HEAD: get without body (200, 401,403,404,405)
  - OPTIONS: all supported methods for URL ()
  - TRACE: echoes the received request ()
- Read Only: GET HEAD OPTIONS TRACE
- Modify Server data: POST, PUT, DELETE, PATCH

## Session & Cookies

- Cookies
  - client가 server에 데이터를 요청하고 그에 대한 응답으로 server가 response에 header에 쿠키토큰을 같이 보낸다.
  - client는 받은 쿠키 토큰을 잠시 브라우저에 저장한다(쿠키는 브라우저의 임시저장공간)
  - 추후 서버에 데이터 요청시 쿠키 토큰을 함께 보낸다
