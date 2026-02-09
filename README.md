# nodejs-hw

Simple Express server for working with notes.  
This project is created as a homework assignment to demonstrate basic Express server setup, middleware usage, routing, and error handling.

## 🚀 Features

- Express server
- Environment variables with dotenv
- CORS enabled
- JSON body parsing
- HTTP request logging with pino-http
- Basic routing
- 404 and 500 error handling

## 📁 Project Structure

```
nodejs-hw/
├── src/
│   └── server.js
├── .env
├── package.json
├── README.md
```

## ⚙️ Environment Variables

Create a `.env` file in the root directory and add:

```
PORT=3000
```

## ▶️ Scripts

```bash
npm run dev   # start server with nodemon
npm start     # start server in production mode
```

## 📌 API Endpoints

### Get all notes
```
GET /notes
```

Response:
```json
{
  "message": "Retrieved all notes"
}
```

### Get note by ID
```
GET /notes/:noteId
```

Response:
```json
{
  "message": "Retrieved note with ID: noteId"
}
```

### Test error handling
```
GET /test-error
```

Throws a simulated server error.

## 🧪 Error Handling

- **404** — Route not found
- **500** — Server error with error message

## 🌍 Deployment

The application is deployed on **Render**.  
Make sure environment variables are configured correctly in the Render dashboard.
