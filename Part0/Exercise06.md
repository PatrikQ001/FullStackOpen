```mermaid
sequenceDiagram
    participant user
    participant browser
    participant server

    user->>browser: Send a note

    browser->>server: POST https://studies.cs.helsinki.fi/exampleapp/new_note_spa

    server-->>browser: [{"message":"note created"}]

    Note right of browser: The browser updates the note list dynamically without reloadin the page
```