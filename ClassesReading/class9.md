# Class Nine Reading

## What are the five steps in the HTTP Request Lifecycle?

- Local Processing
- Resolve an IP
- Establish a TCP Connection
- Send an HTTP Request
- Tearing Down and Cleaning Up

## What are the two things the client needs before it can make an HTTP Request?

- URL (Uniform Resource Locator)
- Server's IP Address or Domain Name

## Explain the four way handshake and what it does

The process begins with the client initiating connection termination by sending a TCP segment with the "FIN" (Finish) flag set to the server. This signifies that the client has completed sending data and intends to conclude the connection. The server promptly acknowledges the client's request by sending an acknowledgment ("ACK") back to the client. Subsequently, the server takes its turn in initiating the connection termination by transmitting a "FIN" segment to the client, indicating its own data transmission completion. The client, upon receiving the server's "FIN" segment, acknowledges the server's request with another acknowledgment. This final acknowledgment confirms that both the client and the server are in agreement about the termination of the connection. 

## True or False: When making an HTTP request, you MUST follow any redirect returned by the request. Back up your answer

True, This is important for maintaining the integrity of the communication process and ensuring that the desired resource is properly accessed. 

## Which built-in Java class can be used to perform an HTTP request?

the HttpURLConnection class to perform HTTP requests.

## What HTTP status codes represent a successful response? A redirect? A client error?

Successful Response: 200 OK

Redirect:
- 301 Moved Permanently
- 302 Found (or 303 See Other)
- 307 Temporary Redirect

Client Error:
- 400 Bad Request
- 401 Unauthorized
- 403 Forbidden
- 404 Not Found
- 405 Method Not Allowed
