# Notes API (Express + MongoDB)

Backend API for managing notes.

## Features
- Pagination for `GET /notes` via query params `page` and `perPage`
- Filtering notes by `tag`
- Full-text search by `search` (MongoDB text index on `title` and `content`)
- Request validation with `celebrate`:
  - `GET /notes` query validation
  - `GET/DELETE /notes/:noteId` params validation (ObjectId)
  - `POST /notes` body validation
  - `PATCH /notes/:noteId` params + body validation (non-empty body)

---

## Tech stack

- Node.js
- Express
- MongoDB Atlas
- Mongoose
- pino-http (logging)
- cors
- dotenv
- http-errors
- celebrate

---
