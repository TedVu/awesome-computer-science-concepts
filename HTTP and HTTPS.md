# HTTP and HTTPS

## What is HTTP ?

- Stands for Hyptertext Transfer Protocol.
- An application layer protocol designed to transfer information between networked devices.
- Run at the top most layer of the network protocol stack (layer 7 application layer).

## Components of a HTTP request

- HTTP version type.
- a URL
- an HTTP method
- HTTP request headers
- Optional HTTP body

## Components of a URL

- Scheme => HTTP or HTTPS
- Domain
- Path
- Resource

## What happens when you type in the URL in web browser ?

- Browser performs a DNS lookup.
  - First it looks in the browser and OS cache.
  - If it cannot find in both browser and OS cache, it make a query to the DNS resolvers.
  - DNS resolvers then will make a chain of request until the URL is resolved, this is process is recursive.
- Browser establishes TCP connection with the server.
  - This process involves multiple round trips.
  - To make this process efficient, the web server and browser use a concept of keep-alive to reuse established connection.
- To establish a HTTPS connection there will be a process of SSL/TLS handshake involved, and the browser use tricks like SSL session resumption to lower the cost.
- After establishing the connection, the client will send a HTTP request to the server and server sends back HTTP response. If there is additional resources such as JavaScript bundles and images then the client repeats the process above.