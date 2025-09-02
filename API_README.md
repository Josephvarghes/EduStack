# EduStack Backend API Documentation

This document describes all available API endpoints, their request/response formats, and authentication requirements.

---

## Authentication APIs

### Register
- **POST** `/api/auth/register`
- **Description:** Register a new user.
- **Request Body:**
```json
{
  "name": "string",
  "email": "string",
  "password": "string"
}
```
- **Response:**
```json
{
  "success": true,
  "token": "jwt_token",
  "user": { "id": "...", "name": "...", "email": "...", "role": "..." }
}
``` 

### Login
- **POST** `/api/auth/login`
- **Description:** Login with email and password.
- **Request Body:**
```json
{
  "email": "string",
  "password": "string"
}
```
- **Response:**
```json
{
  "success": true,
  "token": "jwt_token",
  "user": { "id": "...", "name": "...", "email": "...", "role": "..." }
}
``` 
### Update Profile
- **PUT** `/api/profile`
- **Auth:** Bearer JWT
- **Request Body:**
```json
{ "name": "string", "email": "string" }
```
- **Response:**
```json
{ "success": true, "message": "Profile updated successfully", "data": { ...user fields... } } 
``` 

