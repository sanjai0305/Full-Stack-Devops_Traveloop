🌍 Traveloop – Smart Collaborative Travel Planner

Traveloop is a full-stack collaborative travel planning platform designed to help travelers organize trips, manage budgets, collaborate with friends, track expenses, share itineraries, maintain travel journals, and communicate in real time — all from a single application.

Built with modern web and mobile technologies, Traveloop combines trip planning, budget management, collaboration tools, AI-powered assistance, and real-time synchronization into one seamless travel experience.

✨ Features
🗺️ Trip Planning
Create and manage trips
Day-wise itinerary planning
Destination management
Activity scheduling
Trip status tracking
Public trip sharing
👥 Collaboration System
Invite collaborators via email
Role-based access control
Owner
Editor
Viewer
Real-time collaboration updates
Activity logs
Collaboration notifications
💬 Real-Time Group Chat
Firebase Firestore powered
Offline support
Message replies
Emoji reactions
Voice messages
Location sharing
Share itinerary items
Search messages
Pinned messages
Presence indicators
Typing indicators
Unread message counters
💰 Smart Budget Management
Multi-budget support
Trip-specific budgets
Expense tracking
Budget forecasting
Split expense calculations
Settlement tracking
Currency conversion
Planned vs Actual analytics
Automatic itinerary budget synchronization
Budget validation engine
✈️ Flight Tracking
Flight management
Flight status monitoring
Gate updates
Delay tracking
Timeline integration
📒 Travel Journal
Journal entries
Photo memories
Offline synchronization
Real-time collaboration support
📝 Smart Notes
Shared trip notes
Real-time updates
Offline-first architecture
🎒 Packing Checklist
Collaborative checklist management
Offline support
Auto synchronization
🏆 Achievement & XP System
Travel achievements
XP rewards
User levels
Planning streaks
Progress tracking
Badge unlocks
🤖 AI Travel Assistant

Powered by Google Gemini

Ask:

What should I pack?
Budget recommendations
Restaurant suggestions
Emergency travel advice
Local travel tips
Day plan generation
📤 Public Sharing

Generate public trip links:

https://traveloop.app/share/{token}

View:

Itinerary
Budget Summary
Journal Highlights
Flights

Read-only mode for guests.

🚀 Tech Stack
Frontend
React.js
Vite
Capacitor
React Router
Firebase SDK
Firestore
Realtime Database
Firebase Storage
Chart.js
CSS3
Backend
Node.js
Express.js
MongoDB
Mongoose
JWT Authentication
Nodemailer
Gmail OAuth2
Cloud Services
Firebase Firestore
Firebase Realtime Database
Firebase Storage
Google Maps API
Gemini AI API
🏗️ Architecture
Frontend (React + Capacitor)
           │
           ▼
      Express API
           │
 ┌─────────┼─────────┐
 ▼         ▼         ▼
MongoDB  Firebase  Gemini
           │
           ▼
 Firestore + RTDB
🔐 Authentication

Supported methods:

Email Authentication
Register
Login
JWT Session Management
Google Authentication
Google Sign-In
OAuth Integration
Secure Token Validation
🔄 Real-Time Features

Powered by Firebase.

Firestore

Used for:

Chat Messages
Reactions
Replies
Read Status
Notes
Journal
Checklist
Expenses
Realtime Database

Used for:

Online Presence
Typing Status
Live Indicators
📱 Mobile Support

Traveloop supports:

Android

Built using:

Capacitor Android

Features:

Native App Experience
Offline Mode
Push Notification Ready
Zoom Disabled
Optimized Navigation
📊 Budget System
Budget Overview

Shows:

Total Budget
Planned Budget
Actual Expenses
Remaining Budget
Budget Utilization
Smart Validation

Example:

Trip Budget = ₹150,000

Expense = ₹200,000

Validation:

Expense exceeds available trip budget.

Save button disabled until corrected.

🏅 Achievement System

Users can unlock:

Achievement	Requirement
First Trip Created	Create first trip
Explorer	5 trips
Planner Pro	10 trips
Collaboration Pro	Collaborate on trips
Budget Master	Add expenses
Journal Keeper	Create journals
Flight Tracker	Track flights
Chat Starter	Send messages
🌐 Offline Support

Offline-first architecture powered by Firebase.

Supported Offline Modules:

Chat
Notes
Checklist
Journal
Budget

Features:

Read Offline
Write Offline
Auto Sync
Pending Sync Detection
📧 Email System

Powered by:

Google Gmail API
OAuth2
Nodemailer

Used for:

Collaboration Invites
Support Requests
User Notifications
🔒 Security Features
JWT Authentication
Route Protection
Role-Based Authorization
Backend Validation
Input Sanitization
Rate Limiting
Firebase Security Rules
Secure Token Verification
📂 Project Structure
Traveloop
│
├── Backend
│   ├── controllers
│   ├── models
│   ├── routes
│   ├── middleware
│   ├── services
│   ├── utils
│   └── server.js
│
├── traveloop
│   ├── src
│   │   ├── components
│   │   ├── pages
│   │   ├── context
│   │   ├── services
│   │   ├── hooks
│   │   ├── utils
│   │   └── assets
│   │
│   ├── public
│   ├── android
│   └── capacitor.config.json
│
└── README.md
⚙️ Installation
Clone Repository
git clone https://github.com/yourusername/traveloop.git

cd traveloop
Backend Setup
cd Backend

npm install

npm run dev
Frontend Setup
cd traveloop

npm install

npm run dev
Android Setup
npm run build

npx cap sync android

npx cap open android
🔑 Environment Variables
Backend
MONGO_URI=

JWT_SECRET=

GOOGLE_CLIENT_ID=

GOOGLE_CLIENT_SECRET=

GOOGLE_REFRESH_TOKEN=

GOOGLE_SENDER_EMAIL=

SUPPORT_EMAIL=

GEMINI_API_KEY=
Frontend
VITE_FIREBASE_API_KEY=

VITE_FIREBASE_AUTH_DOMAIN=

VITE_FIREBASE_PROJECT_ID=

VITE_FIREBASE_STORAGE_BUCKET=

VITE_FIREBASE_MESSAGING_SENDER_ID=

VITE_FIREBASE_APP_ID=
🧪 Testing

Run:

node verify_apis.js

node verify_collaboration.js

node verify_firebase_chat.js

node verify_flight.js

Frontend:

npm run build

Android:

npx cap sync android
🎯 Roadmap
V2.2
Push Notifications
AI Trip Cost Prediction
AI Auto Itinerary Builder
Smart Travel Alerts
Weather Forecast Integration
V2.3
Hotel Booking Integration
Flight Booking Integration
Travel Marketplace
Community Trip Discovery
V3.0
AI Travel Copilot
Voice Assistant
Social Travel Feed
Smart Recommendation Engine
👨‍💻 Developer

Sanjai R

Traveloop is built to simplify travel planning through collaboration, automation, budgeting, and real-time communication.

📜 License

This project is licensed under the MIT License.

Copyright (c) 2026 Traveloop

Permission is hereby granted, free of charge,
to any person obtaining a copy of this software
and associated documentation files....