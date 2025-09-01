# EduStack Backend

EduStack is a lightweight and scalable backend for an educational platform (LMS) MVP.  
Built with **Node.js**, **Express**, and **MongoDB Atlas**, it provides APIs for user management, course hosting, and basic file/video handling.  

---

## 🚀 Features

- 🔑 **User Authentication** (JWT-based login & signup)  
- 📚 **Course Management** (Add, edit, list courses)  
- 🎬 **Video & File Handling** (Stored locally for MVP; easy to scale to cloud storage)  
- 🗄️ **MongoDB Atlas** as the primary database  
- ⚡ **RESTful API** with clear structure and error handling  

---

## 📂 Project Structure

``` bash
├── src/
│ ├── config/ # Database & environment config
│ ├── controllers/ # Route logic
│ ├── models/ # Mongoose schemas
│ ├── routes/ # Express routes
│ ├── middleware/ # Auth middleware
│ └── app.js # Main app entry
├── uploads/ # Local file/video storage (MVP)
├── .env # Environment variables
├── package.json
└── README.md ``` 


---

## 🛠️ Tech Stack

| Tech             | Purpose                         |
|------------------|--------------------------------|
| **Node.js**      | Server runtime                 |
| **Express.js**   | API framework                  |
| **MongoDB Atlas**| Database                       |
| **Mongoose**     | ODM for MongoDB               |
| **JWT**          | User authentication           |
| **Multer**       | File & video upload handling  |

---

## 🔧 Installation

1. **Clone the repository:**
   ```bash
   git clone https://github.com/your-username/EduStack.git
   cd EduStack
