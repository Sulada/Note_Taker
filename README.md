# Note Taker

## Description

* This application can write, save, and delete notes. And use an express backend and save and retrieve note data from a JSON file.

* This application have a `db.json` file on the backend that will be used to store and retrieve notes using the `fs` module.

* The following HTML routes should be created:

  * GET `/notes` - Return the `notes.html` file.

  * GET `*` - Return the `index.html` file


* The following API routes should be created:

  * GET `/api/notes` - Read the `db.json` file and return all saved notes as JSON.

  * POST `/api/notes` - Receive a new note to save on the request body, add it to the `db.json` file, and then return the new note to the client.

  * DELETE `/api/notes/:id` - Receive a query parameter containing the id of a note to delete. This means you'll need to find a way to give each note a unique `id` when it's saved. In order to delete a note, you'll need to read all notes from the `db.json` file, remove the note with the given `id` property, and then rewrite the notes to the `db.json` file.

## User Story

  * AS A user, I want to be able to write and save notes

  * I WANT to be able to delete notes I've written before

  * SO THAT I can organize my thoughts and keep track of tasks I need to complete

## Acceptance Criteria

  * Application allow users to create and save notes.

  * Application allow users to view previously saved notes.

  * Application allow users to delete previously saved notes.