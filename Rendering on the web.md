# Rendering on the web

## **Rendering techniques**

- SSR: Server-Side Rendering - rendering a client-side or universal app to HTML on the server.
- CSR: Client-side Rendering -  rendering an app in a browser, generally using the DOM.
- SR: Static Rendering - rendering an HTML page that has been build ahead of time (at built time).
- Prerendering: Running a client-side application at build time to capture its initial state as static HTML.

## **Performance parameters**

- TTFB: Time to first Byte - time between clicking a link and the first bit of content coming in.
- FP: First Paint - the first time any pixels gets becomes visible to the user.
- FCP: First Contentful Paint - the time when requested content becomes visible.
- TTI: Time to Interactive - the time at which the page becomes interactive.

## Server Rendering

Server rendering generates the full HTML for a page on the server in response to navigation, this helps reduce data fetching and templating on the client.

| Performance parameter | Performance |
| --------------------- | ----------- |
| TTFB                  | Low         |
| FP                    | High        |
| FCP                   | High        |
| TTI                   | High        |

## Static Rendering

Producing a separate HTML file for each URL ahead of time, this hence gives really high performance, static renders can be deployed to multiple CDNs to take advantage of edge-caching. A drawback of this approach however is each URL requires individual HTML file.

| Performance parameter | Performance |
| --------------------- | ----------- |
| TTFB                  | High        |
| FP                    | High        |
| FCP                   | High        |
| TTI                   | High        |

## Client-Side Rendering

Client-Side rendering means rendering pages directly in the browser using JavaScript. All logic, data fetching, templating and routing are handled on the client rather than the server.

