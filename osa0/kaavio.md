#Notes-sivun lataus ja uuden muistiinpanon lähetys
```mermaid
  Kaaviotesti TD
  participant A
  participant B
    A [selaimesta kysellään] --> B [web-palvelin vastailee]
    B [eka vastaus/HTML] --> A [odotellaan lisää]
    B [toka vastaus/CSS] --> A [odotellaan vielä]   
    B [kolmas vastaus/JS] --> A [ok, nyt avataan sivu]

```
