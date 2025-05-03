# Hypertext Transfer Protocol (HTTP)

HTTP (Hypertext Transfer Protocol) is a protocol used for communication between web clients (like browsers) and web servers. It defines how clients request data and how servers respond.

## HTTP Status Codes

HTTP status codes are three-digit numbers returned by a server in response to a client's request. They indicate the outcome of the request. The first digit of the status code defines the class of response.

### Classes of HTTP Status Codes:

- **1xx Informational:** The server has received the request and is continuing to process it.
- **2xx Successful:** The request was successfully received, understood, and accepted.
- **3xx Redirection:** Further action needs to be taken by the client to complete the request.
- **4xx Client Error:** The request contains bad syntax or cannot be fulfilled, indicating a problem on the client side.
- **5xx Server Error:** The server failed to fulfill an apparently valid request due to an issue on the server side.

### Examples of HTTP Status Codes and Their Meanings:

Here are some common HTTP status codes and their descriptions:

- **200 OK:** The standard response for successful HTTP requests. The request was fulfilled.
- **201 Created:** The request has been fulfilled, resulting in the creation of a new resource.
- **202 Accepted:** The request has been accepted for processing, but the processing is not complete.
- **204 No Content:** The server successfully processed the request, but is not returning any content.
- **301 Moved Permanently:** The requested data has been permanently moved to a new URL.
- **302 Found:** The requested data resides temporarily under a different URL.
- **303 See Other:** The response to the request can be found under a different URI and should be retrieved using a GET method.
- **304 Not Modified:** The resource has not been modified since the version specified by the request headers.
- **400 Bad Request:** The server did not understand the request due to incorrect syntax.
- **401 Unauthorized:** The request requires user authentication.
- **403 Forbidden:** The server understood the request but refuses to authorize it.
- **404 Not Found:** The requested resource could not be found on the server.
- **405 Method Not Allowed:** The request method is not supported for the requested resource.
- **500 Internal Server Error:** The server encountered an unexpected condition that prevented it from fulfilling the request.
- **501 Not Implemented:** The server does not support the functionality required to fulfill the request.
- **502 Bad Gateway:** The server, while acting as a gateway or proxy, received an invalid response from an upstream server.
- **503 Service Unavailable:** The server is temporarily unable to handle the request, often due to maintenance or high traffic.

## Examples Related to HTTPS

HTTPS (Hypertext Transfer Protocol Secure) is the secure version of HTTP, where communication is encrypted. While most HTTP status codes apply to both HTTP and HTTPS, some status codes or error messages can be specific to issues encountered within the secure connection process (SSL/TLS handshake).

Examples of status indicators or error codes you might encounter in an HTTPS context include:

- **497 HTTP Request Sent to HTTPS Port (nginx-specific):** This indicates that a client sent a standard HTTP request to a port configured for HTTPS.
- **525 SSL Handshake Failed (Cloudflare-specific):** This error means that the SSL/TLS handshake between Cloudflare and the origin web server failed.
- **526 Invalid SSL Certificate (Cloudflare-specific):** This indicates that Cloudflare could not validate the SSL certificate on the origin web server.

These examples highlight issues that can occur specifically when establishing or maintaining a secure HTTPS connection.
