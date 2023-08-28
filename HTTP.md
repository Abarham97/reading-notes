 ## HTTP Request Lifecycle and HTTP Status Codes

The process of making an HTTP request involves several steps in the HTTP Request Lifecycle:

URL Parsing: The client extracts components from the URL, such as protocol, domain, port, path, and query parameters. This information is used to establish a connection with the server.

DNS Resolution: If the domain is not an IP address, the client performs DNS resolution to translate the domain name into an IP address, helping locate the server on the internet.

TCP/IP Connection: The client establishes a TCP connection with the server's IP address using a three-way handshake process to ensure reliability.

##  HTTP Request Sending: The client sends an HTTP request to the server, comprising a request line, headers, and optionally a message in the body.

Server Processing and Response: The server receives the request, processes it, and generates an HTTP response containing a status line, headers, and response body.

For the client to make an HTTP request, it requires two main components:

URL: The URL specifies the resource's location, including protocol, domain, port, path, and query parameters.

HTTP Method (HTTP Verb): The HTTP method indicates the action the client wants to perform on the resource. Common methods include GET (retrieve data), POST (send data to create a resource), PUT (send data to update a resource), DELETE (request resource deletion), and PATCH (send partial update).

The "Four-Way Handshake" refers to the process of gracefully closing a TCP connection, involving segments with FIN (Finish) flags sent by both parties to signal termination. This helps prevent data loss during connection termination.

## HTTP status codes are divided into ranges with distinct meanings:

1xx - Informational Responses: Server processing continues.
2xx - Successful Responses: Request successfully received and processed.
3xx - Redirection Responses: Further client action required for resource location.
4xx - Client Error Responses: Client-related errors prevent request fulfillment.
5xx - Server Error Responses: Server-side errors prevent request fulfillment.

Some common status codes include 200 OK (successful), 301 Moved Permanently (resource permanently moved), 404 Not Found (resource not found), and 500 Internal Server Error (server encountered an error).

It's important to follow redirects returned by requests for better user experience, SEO, caching, security, and data integrity. In Java, the java.net.HttpURLConnection class is used to perform HTTP requests.