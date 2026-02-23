```mermaid
sequenceDiagram
  participant browser
  participant server

  browser->>server: POST https://studies.cs.helsinki.fi/exampleapp/new_note_spa
  activate server
  server-->>browser: 201 Crated | HTML document
  deactivate server

  activate browser
  note right of browser: The browser adds a new note to the list.
  deactivate browser
```
