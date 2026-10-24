# Sound Wave API

A backend application for a sound wave platform built using Node.js, Express.js, and MongoDB. It provides user authentication, role-based access control, music uploads, and album management.

## Features

- **User Authentication:** User registration and login.
- **Password Hashing:** Secure password hashing using bcrypt.
- **JWT Authentication:** Token-based authentication using JSON Web Tokens and cookies.
- **Role-Based Authorization:** Separate access permissions for users and artists.
- **Music Upload:** Upload music files using Multer and ImageKit.
- **Album Management:** Create albums and associate music tracks with artists.
- **MongoDB Integration:** Store user, music, and album information using Mongoose.

## Tech Stack

- Node.js
- Express.js
- MongoDB
- Mongoose
- JSON Web Token (JWT)
- bcryptjs
- Multer
- ImageKit
- Cookie Parser

## Project Structure

```text
backend/
├── src/
│   ├── controllers/
│   ├── middleware/
│   ├── models/
│   ├── routes/
│   └── services/
├── .env
├── .gitignore
├── package.json
├── package-lock.json
└── server.js
```

The server will run on the configured port, for example `http://localhost:3000`.

## API Endpoints

| Method | Endpoint | Description |
|---|---|---|
| POST | `/api/auth/register` | Register a new user |
| POST | `/api/auth/login` | Log in |
| POST | `/api/auth/logout` | Log out |
| POST | `/api/music/upload` | Upload music |
| POST | `/api/music/album` | Create an album |


## Authentication and Authorization

- Users register and log in using their credentials.
- Passwords are hashed before being stored in MongoDB.
- JWT tokens are used to authenticate requests.
- Cookies carry authentication tokens.
- Artist-only operations require the appropriate role.

## Future Improvements

- Retrieve and stream music tracks.
- Fetch albums and their associated tracks.
- Add music and album deletion or update functionality.
- Improve request validation and error handling.
- Implement token blacklisting for logout.
- Add automated API tests.

## Learning Goals

This project was built as part of my backend development learning journey to practise REST APIs, authentication, authorization, database modelling, file uploads, and integration with external storage services.



****   Developed as a backend learning project.....*****
