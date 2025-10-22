# 🧠 Thinkify — A Collaborative Space for Thought and Productivity

Thinkify is a dynamic web platform that brings together students and thinkers from all backgrounds to exchange ideas, manage tasks, and share knowledge in an engaging, community-driven environment. It empowers users to create, edit, and organize posts, express their thoughts publicly or privately, and connect through meaningful discussions.

Built with a focus on simplicity and collaboration, Thinkify helps users stay organized, inspired, and connected — making it not just a productivity tool, but a hub for creativity and shared learning.

# Preview

<img src="/preview.png">
<a href="https://thinkify.vercel.app" target="_blank">Live Preview</a> | <a href="https://thinkify-server.vercel.app" target="_blank">Live API</a> | <a href="https://documenter.getpostman.com/view/27027258/2sA3dxEXJh" target="_blank">Postman</a>

# Requirements

[Install Node On Your Device](https://nodejs.org/)

# How to Run

```
git clone https://github.com/PrithviElancherran/Thinkify-Website.git

# BACKEND
cd server
npm install
npx nodemon index.js

# FRONTEND
cd ../client
npm install
npm run dev
```

# Environment Variables

## Frontend

```
VITE_SERVER_ENDPOINT = https://thinkify-server.vercel.app:3000/api
VITE_TOKEN_KEY = thinkify
VITE_USER_ROLE = role
VITE_COOKIE_EXPIRES = 1
```

## Backend

```
PORT = 3000
DATABASE_URL = mongodb://localhost:27017/
DATABASE_NAME = thinkify
BCRYPT_GEN_SALT_NUMBER = 10
JWT_SECRET_KEY = abcdefghijklmnopqrstuvwxyz
COOKIE_EXPIRES = 5d
COOKIE_KEY = thinkify
UPLOAD_DIRECTORY = uploads
```

# Features

## Admin

- Profile
  - Last Month User Activity
  - Role Based User Distribution
- Users Management
- Sign Out

## Student

- Profile
- Add Post
- My Posts
- Add Product
- My Products
- Task Manager
- Setting
  - Change Password
- Sign Out

# Contribution Ideas

- Continue with Google signup/signin
- Single Product Sell Page
- View Task Details
- View User Details(public)
- Edit user, post, product
- Loading View

## Institution/Teacher

- post(text, image)
  - by admin/institution
  - by teacher
- assignments
- poll
- resource sharing
- test

### Design Idea

```
|----------------------------------------------------------------
|                 |                                |  Analytics |
|-----------------|                                |------------|
|                 |          ----------            |  Teachers  |
|-----------------|          | Create |            |  Students  |
|   Institution   |          ----------            |  Courses   |
|-----------------|                                |    Posts   |
|                 |                                |    ....    |
|-----------------|--------------------------------|------------|
```

### Assignments

- title
- description
- subject
- deadline
- total marks
- status
- audience

### Polls

- title
- description
- type(singl, multiple)
- options
- deadline
- status
- anonymous member
- audience

### Resource

- title
- description
- visibility
- url
- audience
