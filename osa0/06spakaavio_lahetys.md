#TEHTÄVÄ 0.5 - SPA - uuden muistiinpanon lähetys (Single Page Application)
```mermaid
  sequenceDiagram
  participant bc as browser client (HTTP Request)
  participant s as server (HTTP Response)  

  bc->>s: New SPA note coming up! POST https://studies.cs.helsinki.fi/exampleapp/new_note_spa
  Note over bc, s: content: "new spa note", date: "2023-07-07T10:07:50.414Z"
  Note left of bc: It's so great I dont' need to request all the UI stuff again.
  bc->>bc: JS tells me to reload the notes with the latest addition.
  Note right of s: Great! New clients will now be able GET this new note too.

```
### In this solution, all clients wont' be in sync without refreshing the page
If there are multiple clients posting new notes, they will see only the contents they received in the json file they loaded last.
They will see their own new posts, but not others' who are posting at the same time.
To see the latest posts, a new GET request to the web server is required.
