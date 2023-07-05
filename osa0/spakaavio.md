#SPA - uuden muistiinpanon lähetys (Single Page Application)
```mermaid
  sequenceDiagram
  participant bc as browser client (HTTP Request)
  participant s as server (HTTP Response)  

  bc->>s: New SPA note coming up! POST
  Note left of bc: testing how this looks like 
  s->>bc: Great! HTTP Status Code: 201 Created.

```
