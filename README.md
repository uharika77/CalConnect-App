## CalConnect 📅

CalConnect is a full-stack web application that integrates Google Calendar to help users manage their events efficiently. It allows users to log in via Google, fetch their upcoming events, and filter them by date.

## 🚀 Features

- Google OAuth 2.0 Authentication – Secure login using Google accounts.
  
- Fetch Google Calendar Events – Displays upcoming events from the user's calendar.
  
- Date Filtering – Users can filter events by selecting a date.
  
- Seamless Frontend-Backend Communication – React-based frontend with an Express.js backend.
  
# 🛠️ Tech Stack

- Frontend: React, Axios, React DatePicker
  
- Backend: Node.js, Express.js, Google Calendar API
  
- Authentication: Google OAuth 2.0
  
- Other Tools: dotenv for environment variables, CORS for handling cross-origin requests
  
# 📂 Project Structure

CalConnect/

│── calendar-app-frontend/ # Frontend (React)

│── calendar-app-backend/    # Backend (Node.js, Express)

│── README.md

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
- 
node server.js 

3️⃣ Frontend Setup

cd ../calendar-app-frontend 

npm install

npm start 

# 🎯 Usage
1. Open http://localhost:3000 in your browser.

2. Click Login with Google to authenticate.

3. View and filter your Google Calendar events.

# 📌 To-Do & Future Enhancements

- Add event creation functionality

- Improve UI/UX with better styling

- Deploy the application for public access
