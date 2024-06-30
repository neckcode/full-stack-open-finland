```mermaid
sequenceDiagram
    participant browser
    participant server

    browser->>server: POST https://studies.cs.helsinki.fi/exampleapp/new_note_spa {"content":"sd", "date": "2024-06-30T22:48:18490Z"}

    activate server
    server-->>browser: HTML document
    deactivate server

    Note right of browser: The browser executes the callback function that renders the notes

```