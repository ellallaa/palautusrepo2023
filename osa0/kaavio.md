#Notes-sivun lataus ja uuden muistiinpanon lähetys
```mermaid
  sequenceDiagram
  participant s as selain
  participant p as palvelin   

  s->>p: Can I GET this site open? "https://studies.cs.helsinki.fi/exampleapp/notes"
  p->>s: Here is the HTML file.
  s->>p: Can I GET the CSS too? https://studies.cs.helsinki.fi/exampleapp/main.css"
  p->>s: Here you go! All the colors, font types etc. can be read from this CSS."
  s->>p: Oh! This is not just a static page. Can I GET the JS too? https://studies.cs.helsinki.fi/exampleapp/main.js
  p->>s: JavaScript is on its way!
  s->>p: I ran the JS code, could you GET me this data.json file contents, please?
  p->>s: Content coming up! [{ "content": "This is so fun!", "date": "2023-7-5" }, ... ]
  S: Great! No I can render the page and the all the latest notes!  
```
