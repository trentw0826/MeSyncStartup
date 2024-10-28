# _MeSync_ - Personal Journal and Reflection App
## Elevator Pitch
MeSync helps users connect with themselves through structured, clean, clarifying, personalized, and simple journaling. With features like guided prompts, mood tracking, and an analytics dashboard, MeSync transforms simple journaling into a powerful tool for self-reflection and personal growth. Whether users are tracking daily moods or setting monthly intentions, MeSync offers meaningful insights to deepen their understanding and mindfulness.

## Features
### Guided Daily Prompts: 
Encourages reflection with prompts based on past entries and mood trends.
### Mood Tracking and Sentiment Analysis: 
Tracks daily moods and provides insights via sentiment analysis.
### Personalized Analytics Dashboard: 
Visualizes mood trends and journaling patterns for self-awareness.
### Gratitude and Achievements Highlights: 
Recaps positive moments each week for perspective and mindfulness.
### Monthly Reflection and Goal Setting: 
Guides users through reviewing past entries and setting future intentions.

## Technological Demonstration
### HTML
Structures the web pages, including the login, registration, and main journal dashboard. Uses semantic HTML to ensure accessibility and clear navigation.
### CSS
Provides styling optimized for different screen sizes (responsive design) with careful use of whitespace, color contrast, and typography to enhance readability and a calming aesthetic suitable for a journaling app.
### JavaScript
Handles user interactions such as login, journal entry creation, and submitting moods, as well as backend API calls for saving and retrieving entries, moods, and user data.
### React
Builds the app as a single-page application with componentized views for each feature (e.g., journal entries, mood tracker, and analytics). React’s state management provides a smooth, dynamic user experience by updating components based on user actions.
### Node.js/Express
Backend service with endpoints for:
- Retrieving journal entries
- Submitting new entries
- Retrieving and updating mood tracking data
- User authentication and registration
### Sentiment Analysis API
Uses an external sentiment analysis API to analyze the tone of journal entries, giving users insights into emotional patterns.
### Database
MongoDB stores user data, journal entries, and mood information. Authentication credentials are securely stored, and only logged-in users can access and modify their data.
### JWT Authentication
Authenticates users via JSON Web Tokens (JWT), ensuring that only authenticated users can access and modify personal data in the app.
WebSocket (Socket.IO) - Supports real-time updates to the mood analytics dashboard. As users add entries or modify mood information, updates are broadcasted to all active sessions for seamless data synchronization across devices.
