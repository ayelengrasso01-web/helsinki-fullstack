
sequenceDiagram
    participant browser
    participant server

    Note right of browser: El JavaScript añade la nueva nota a la lista local y la dibuja en la pantalla inmediatamente

    browser->>server: POST https://studies.cs.helsinki.fi/exampleapp/new_note_spa
    activate server
    server-->>browser: HTTP 201 Created
    deactivate server