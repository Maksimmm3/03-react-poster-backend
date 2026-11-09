# React Poster — Backend

Simple Express REST API that powers the [React Poster](https://github.com/Maksimmm3/04-react-poster) frontend. Provides endpoints for fetching, creating and viewing posts.

## Tech Stack

- Node.js
- Express
- body-parser (JSON request parsing)
- JSON file storage (`data/posts.json`)

## Endpoints

| Method | Path         | Description             |
| ------ | ------------ | ----------------------- |
| GET    | `/posts`     | Get all posts           |
| GET    | `/posts/:id` | Get a single post by id |
| POST   | `/posts`     | Create a new post       |

### POST `/posts` — request body

```json
{
  "author": "Anna",
  "body": "Post content"
}
```

The server generates a unique `id` for each new post and returns `201 Created`.

## Getting Started

```bash
npm install
npm start
```

The server runs on `http://localhost:8080`.

## Related

- Frontend: [04-react-poster](https://github.com/Maksimmm3/04-react-poster)
