YourParkguide is a mobile application designed to help users save their parking location and navigate back to it easily. The system is built on top of existing map and location technologies, particularly Google Maps and GPS services. The architecture is simple, lightweight, and focused on reliability and ease of use.

Main Components

Component	Description

Mobile App (Frontend)	Interface the user interacts with. Displays map, save button, reminders and AR navigation.

Backend Service	Handles saving and retrieving parking location data, user alerts, and optional cloud sync.

Database	Stores saved parking locations, parking history, and user preferences.

Location and Maps API	Provides GPS data and map navigation features.

AR Navigation Engine	Uses ARCore to guide users visually back to their car.



Technology Stack

Layer	Technology

Frontend	Flutter or React Native (Cross-platform mobile app)

Backend	Node.js or Python (Fast and simple API service)

Database	Firebase Firestore or PostgreSQL (Lightweight and scalable)

Maps & Navigation	Google Maps API

AR	ARCore SDK (Android) / ARKit (iOS)


How Components Communicate

•	User parks their car.

•	The app uses GPS to detect the location.

•	Frontend sends the location to the backend.

•	The backend stores it securely in the database.

•	User later opens the app to find the car.

•	The frontend requests the stored location.

•	The app shows two navigation options:

•	Standard map directions

•	AR visual guidance

Optional: The user can share the parking location with someone else or review previous parking history.

Why This Architecture Works

•	It uses existing and reliable map technology instead of creating new ones.

•	The backend is minimal, keeping the system light and cost-friendly.

•	AR navigation enhances user experience without complicating the workflow.

•	The structure is scalable and can later include notifications, security alerts and offline storage.

