```mermaid
sequenceDiagram

participant Browser
participant Server

 Note right of Browser: User enters a new note and clicks "Save"

 Browser->>Server: Post https://studies.cs.helsinki.fi/exampleapp/new_note_spa

 activate Server
 Server->>Browser: JSON responds with success message
 deactivate Server

  Note right of Browser: JavaScript adds the new note  dynamically

  Note right of Browser: Browser updates notes list without reloading page







```
