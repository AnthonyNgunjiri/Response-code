<!-- START doctoc generated TOC please keep comment here to allow auto update -->
<!-- DON'T EDIT THIS SECTION, INSTEAD RE-RUN doctoc TO UPDATE -->
**Table of Contents**  *generated with [DocToc](https://github.com/thlorenz/doctoc)*

  - [HTTP RESPONSE STATUS CODE](#http-response-status-code)
- [Informational Responses (100 – 199)**:](#informational-responses-100--199)
- [Successful Responses (200 – 299)**:](#successful-responses-200--299)
- [Server Error Responses (500 – 599)**:](#server-error-responses-500--599)

<!-- END doctoc generated TOC please keep comment here to allow auto update -->



### HTTP RESPONSE STATUS CODE

HTTP response status codes indicate the result of an HTTP request. They are grouped into five categories:

 ## Informational Responses (100 – 199)**: 
 Indicates the request was received and understood. The client may continue the process.
   - **100 Continue**: The client should continue the request.
   - **101 Switching Protocols**: The server is switching protocols.
   - **102 Processing**: The request is being processed, but no response is available yet.
   - **103 Early Hints**: The server sends preliminary responses to facilitate preloading resources.

 ## Successful Responses (200 – 299)**: 
The request was successfully received, understood, and accepted.
   - **200 OK**: The request succeeded.
   - **201 Created**: A new resource was created.
   - **202 Accepted**: The request has been accepted but not yet processed.
   - **203 Non-Authoritative Information**: The response comes from a third party or a local copy.
   - **204 No Content**: The request succeeded but there is no content to return.
   - **205 Reset Content**: Tells the client to reset the document view.
   - **206 Partial Content**: Only part of the resource is delivered.
   - **207 Multi-Status**: Provides status for multiple independent operations.
   - **208 Already Reported**: The members of a DAV binding are already enumerated.
   - **226 IM Used**: The response is a result of instance manipulations.

3. ## Redirection Messages (300 – 399)**: 
Further action needs to be taken by the user agent to fulfill the request.
   - **300 Multiple Choices**: Multiple options for the resource.
   - **301 Moved Permanently**: The resource has been permanently moved to a new URI.
   - **302 Found**: The resource is temporarily located at a different URI.
   - **303 See Other**: Directs the client to retrieve the resource at another URI using a GET request.
   - **304 Not Modified**: The resource has not been modified.
   - **305 Use Proxy**: Deprecated. Indicates the resource must be accessed through a proxy.
   - **307 Temporary Redirect**: The resource resides temporarily under a different URI; use the same method.
   - **308 Permanent Redirect**: The resource is permanently located at a different URI; use the same method.

4. ## Client Error Responses (400 – 499)**:
 The request contains bad syntax or cannot be fulfilled.
   - **400 Bad Request**: The server cannot process the request due to client error.
   - **401 Unauthorized**: Authentication is required.
   - **402 Payment Required**: Reserved for future use.
   - **403 Forbidden**: The server refuses to authorize the request.
   - **404 Not Found**: The requested resource could not be found.
   - **405 Method Not Allowed**: The request method is not supported.
   - **406 Not Acceptable**: The server cannot produce a response matching the accept headers.
   - **407 Proxy Authentication Required**: Authentication is required through a proxy.
   - **408 Request Timeout**: The server timed out waiting for the request.
   - **409 Conflict**: The request conflicts with the current state of the server.
   - **410 Gone**: The resource is permanently gone.
   - **411 Length Required**: The server requires a valid Content-Length header.
   - **412 Precondition Failed**: The server does not meet one of the preconditions specified by the client.
   - **413 Payload Too Large**: The request is larger than the server can handle.
   - **414 URI Too Long**: The URI is too long for the server to process.
   - **415 Unsupported Media Type**: The media type is not supported by the server.
   - **416 Range Not Satisfiable**: The range specified cannot be satisfied.
   - **417 Expectation Failed**: The server cannot meet the expectations of the request header.
   - **418 I'm a teapot**: A playful status code indicating that the server refuses to brew coffee.
   - **421 Misdirected Request**: The request was directed to a server not able to produce a response.
   - **422 Unprocessable Content**: The server understands the content type and syntax, but the request is unprocessable.
   - **423 Locked**: The resource is locked.
   - **424 Failed Dependency**: The request failed due to another request failure.
   - **425 Too Early**: The server is unwilling to risk processing a request that might be replayed.
   - **426 Upgrade Required**: The client should switch protocols.
   - **428 Precondition Required**: The origin server requires the request to be conditional.
   - **429 Too Many Requests**: The user has sent too many requests in a given time.
   - **431 Request Header Fields Too Large**: The header fields are too large.
   - **451 Unavailable For Legal Reasons**: The resource is unavailable for legal reasons.

 ## Server Error Responses (500 – 599)**: 
The server failed to fulfill a valid request.
   - **500 Internal Server Error**: The server encountered an error and could not complete the request.
   - **501 Not Implemented**: The server does not support the functionality required to fulfill the request.
   - **502 Bad Gateway**: The server, while acting as a gateway, received an invalid response.
   - **503 Service Unavailable**: The server is currently unavailable.
   - **504 Gateway Timeout**: The server, while acting as a gateway, did not receive a timely response.
   - **505 HTTP Version Not Supported**: The HTTP version is not supported.
   - **506 Variant Also Negotiates**: The server has an internal configuration error.
   - **507 Insufficient Storage**: The server is unable to store the representation needed to complete the request.
   - **508 Loop Detected**: The server detected an infinite loop.
   - **510 Not Extended**: Further extensions to the request are required.
   - **511 Network Authentication Required**: The client needs to authenticate to gain network access.

These status codes help communicate the result of the HTTP request between the client and server.