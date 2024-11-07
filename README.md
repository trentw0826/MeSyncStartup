# _MeSync_ - Personal Journal and Reflection App
## Elevator Pitch
MeSync helps users connect with themselves through simple, clean, clear, and personalized journaling. With features like a relaxing UX, guided daily prompts, and a simple analytics system, MeSync uses simple journaling as a powerful tool for self-reflection and personal growth. Whether users are tracking daily moods and events or setting monthly intentions, MeSync offers meaningful insights to deepen their understanding and mindfulness.

## Features
### Guided Daily Prompts:
Encourages reflection with prompts based on past entries and mood trends.
### Daily Impressions
The virtual equivalent of a nightstand sticky-note, a simple way to get down those impressions that shouldn't be forgotten
### Personalized Analytics
Visualizes journaling trends and patterns for increased self-awareness.
### Prompt board
A live, interactive board where users share their favorite prompts and let learn from interactive brainstorming 
### Secure data
Personal data is encrypted and safe for the peace of mind that comes with private reflection

![MeSync Sketches](/assets/MeSync%20Sketches.png)

## Technological Demonstration
### HTML
Structures simple and powerful web pages, including the login, registration, and main journal dashboard. Uses semantic HTML to ensure accessibility and clear navigation.
### CSS
Provides styling optimized for different screen sizes (responsive design) with careful use of calming color palettes, a simplistic interface, and intuitive navigation to make the MeSync experience attractive and easy
### JavaScript
Handles user interactions such as login, journal entry creation, importing,  exporting, as well as backend API calls for saving and retrieving entries, interacting with the live prompt board, and user data.
### React
Builds the app as a single-page application with componentized views for each feature (e.g., journal entries, daily impressions, and analytics). React’s state management provides a smooth, dynamic user experience by updating components based on user actions.
### Node.js/Express
Backend service with endpoints for:
- Retrieving journal entries
- Submitting new entries
- Submitting new daily impressions
- Interaction with live prompt board
- User authentication and registration
### Voice-to-text API
Voice-to-text integration allows users to quickly and conveniently get their thoughts down
### Database
MongoDB stores user data, journal entries, and more. Authentication credentials are securely stored, and only logged-in users can access and modify their data.
### Websocket Communication
Real-Time prompt sharing allows users to share their favorite journaling prompts with each other in a live but quiet feed. Users could like prompts or mark them for later, and each prompt’s author would see an anonymous tally of how many people connected with it.
### JWT Authentication
Authenticates users via JSON Web Tokens (JWT), ensuring that only authenticated users can access and modify personal data in the app.

## Deliverables
# HTML
The main HTML commit includes the foundational structure for the MeSync web application. It encompasses the layout for the login and registration pages, as well as the main journal dashboard. Semantic HTML elements are used to ensure accessibility and clear navigation, providing a solid base for the app's user interface. Additionally, this commit added placeholders for all main service functionality, including but not limited to backend database calls, calls to a couple 3rd-party APIS, a live websocket prompt feed, and other backend services.