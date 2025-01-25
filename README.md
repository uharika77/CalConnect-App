# Google Calendar Integration with Firebase Authentication

This project is a simple React application that integrates with the Google Calendar API and Firebase Authentication. It allows users to sign in with their Google account and view their upcoming Google Calendar events.

## Features

- **Google Sign-In**: Users can sign in with their Google account using Firebase Authentication.
- **Google Calendar Integration**: Once signed in, users can view their upcoming events from Google Calendar.
- **Filter Events**: Filter events by their name, start time, and end time.

## Prerequisites

Before you begin, make sure you have the following installed:

- [Node.js](https://nodejs.org/)
- [npm](https://www.npmjs.com/)
- [Google Cloud Console API Key](https://console.cloud.google.com/)
- [Firebase Project Setup](https://console.firebase.google.com/)

## Setup

1. **Clone the Repository**:

   git clone https://github.com/your-username/google-calendar-integration.git
   cd google-calendar-integration
   
2. **Install Dependencies**:
   
   Run the following command to install the required dependencies:

   npm install

3. **Set up Firebase Authentication**:

i.Create a Firebase project from Firebase Console.

ii. Go to Authentication in the Firebase Console and enable Google Sign-In under the Sign-In method tab.

iii.Get your Firebase config (API key, project ID, etc.) from the Firebase Console.

4. **Configure Firebase in the App**:
   
Create a firebase.js file in the src directory and initialize Firebase with your credentials:
import firebase from 'firebase/app';
import 'firebase/auth';

const firebaseConfig = {
  apiKey: "YOUR_API_KEY",
  authDomain: "YOUR_AUTH_DOMAIN",
  projectId: "YOUR_PROJECT_ID",
  storageBucket: "YOUR_STORAGE_BUCKET",
  messagingSenderId: "YOUR_MESSAGING_SENDER_ID",
  appId: "YOUR_APP_ID",
};

const firebaseApp = firebase.initializeApp(firebaseConfig);

export default firebaseApp;

5. **Set Up Google Calendar API**:
   
   Go to the Google Cloud Console.
   Create a new project and enable the Google Calendar API.
   Create OAuth 2.0 credentials for your project.
   Use the Client ID and API key in your code to authenticate and access the Google Calendar API.

6. **Set Up Google API Client**:
   Make sure you have included the Google API client script in your public/index.html file:
   <script async defer src="https://apis.google.com/js/api.js"></script>

7. **Run the App**:

   Once the setup is complete, you can start the development server:

   npm start
   Visit http://localhost:3000 in your browser, and you should be able to sign in with your Google account and see your Google Calendar events.

## How It Works

**Firebase Authentication**: The app uses Firebase Authentication to handle Google Sign-In. Once a user signs in, Firebase provides the necessary authentication token to access Google APIs.

**Google Calendar API**: After the user is authenticated, the app loads the Google API client and makes requests to the Google Calendar API to fetch events.
Event Display: The events are displayed in a table format, and the user can filter events by their name, start time, and end time.
Troubleshooting

**CORS Errors**: If you encounter CORS issues, ensure your app is running on HTTPS, as Google APIs require it.
API Key/Client ID Issues: Double-check your API key and Client ID in the Google Cloud Console to ensure they are correct.
Google API Authorization: Make sure the user has granted access to their Google Calendar by checking the authorization scopes.

## Future Enhancements

**Add More Filters**: 
Implement more filters like event location, description, etc. 

**Event Management**: 
Add functionality to create, update, and delete events on Google Calendar.

**Styling Improvements**: 
Improve the design and user interface for a more polished look.

## License

This project is licensed under the MIT License - see the LICENSE file for details.

