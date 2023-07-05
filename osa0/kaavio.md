#Notes-sivun lataus ja uuden muistiinpanon lähetys
```mermaid
  sequenceDiagram
  participant s as selain
  participant p as palvelin   

  s->>p: Can I open this site?
  p->>s: Here is the HTML file.
  p->>s: And here are the font types etc. in CSS.
  p->>s: And last but not least, the JS. Your turn!

```
