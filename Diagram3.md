sequenceDiagram
    participant browser
    participant server

    Note right of browser: The User writes a note and clicks the Save button

    browser->>server: POST https://studies.cs.helsinki.fi/exampleapp/new_note_spa
    activate server
    server-->>browser: It confirms that the note has been saved
    deactivate server
