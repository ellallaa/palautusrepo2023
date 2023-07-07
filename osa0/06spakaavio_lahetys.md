#TEHTÄVÄ 0.5 - SPA - uuden muistiinpanon lähetys (Single Page Application)
```mermaid
  sequenceDiagram
  participant bc as browser client (HTTP Request)
  participant s as server (HTTP Response)  

  bc->>s: New SPA note coming up! POST https://studies.cs.helsinki.fi/exampleapp/new_note_spa {content: "new spa note", date: "2023-07-07T10:07:50.414Z"}
  Note left of bc: It's so great I dont' need to request all the UI stuff again. I just POST to server and reload the notes with the latest addition.
  Note right of s: Gret! New clients connecting https://studies.cs.helsinki.fi/exampleapp/SPA will now be able to see this new content too. All clients wont' be in sync without refreshing the page though.

```
