## CalConnect 📅

A full-stack Google Calendar integration app using React, Node.js, and Express.js

## Overview

CalConnect is a full-stack web application that integrates with Google Calendar, allowing users to authenticate via Google OAuth 2.0, view their upcoming events, and filter them by date. The project is built using React for the frontend and Node.js with Express.js for the backend, leveraging the Google Calendar API for event retrieval.

## 🚀 Features

✅ Google OAuth 2.0 authentication
✅ Fetch and display Google Calendar events
✅ Date-based event filtering
✅ Seamless frontend-backend communication with Axios
✅ Responsive and user-friendly UI
  
## 🛠️ Tech Stack

- Frontend: React, Axios, React DatePicker
  
- Backend: Node.js, Express.js, Google Calendar API
  
- Authentication: Google OAuth 2.0
  
- Other Tools: dotenv for environment variables, CORS for handling cross-origin requests

# ⚙️ Setup Instructions

1️⃣ Clone the Repository

git clone https://github.com/uharika77/CalConnect.git 

cd CalConnect 

2️⃣ Backend Setup

cd calendar-app-backend 

npm install  

- Create a .env file in the calendar-app-backend directory and add the following:

GOOGLE_CLIENT_ID=your_client_id

GOOGLE_CLIENT_SECRET=your_client_secret

REDIRECT_URI=your_redirect_uri

PORT=5001

- Start the backend server:
   
node server.js 

3️⃣ Frontend Setup

cd ../calendar-app-frontend 

npm install

npm start 

# Demo Video 🎥

Check out how the project works in this video recording:

📌 Watch the [DEMO](https://drive.google.com/file/d/14i1QAWU3QGTyjM9zp6U1mVOtx2BUEoTn/view)

# 🎯 Usage

1. Open http://localhost:3000 in your browser.

2. Click Login with Google to authenticate.

3. View and filter your Google Calendar events.


