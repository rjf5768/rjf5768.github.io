---
title: "SportConnect – AI-Assisted Sports Social Networking App"
excerpt: "Personal Project<br/><br/>A full-stack mobile application that connects sports enthusiasts based on geographic proximity, featuring AI-powered form analysis, real-time messaging, media sharing, and privacy-controlled location discovery.<br/><br/><b>Tech:</b> React Native, TypeScript, AWS (DynamoDB, S3, AppSync), Expo, Computer Vision<br/><b>Focus:</b> AI for sports, real-time systems, cloud architecture, mobile development<br/><br/><img src='/images/555.jpg' style='width:24%; margin-right:5px;'><img src='/images/666.jpg' style='width:24%; margin-right:5px;'><img src='/images/777.jpg' style='width:24%; margin-right:5px;'><img src='/images/888.jpg' style='width:24%;'>"
collection: portfolio
---

## Project Overview

**SportConnect** is a location-based social networking mobile application built with React Native. The app enables users to connect with other sports enthusiasts based on geographic proximity, share posts with images and videos, and communicate through real-time messaging.

**Key Highlights:**
- **AI-powered form analysis** for sports technique feedback
- Fully deployed on AWS US (us-east-1)
- Real-time chat with AWS AppSync GraphQL subscriptions
- Video upload and playback with automatic compression
- Privacy-first location sharing with multiple visibility modes
- Offline-first architecture with smart caching

## Technology Stack

### Frontend
- **Framework:** React Native with Expo
- **Language:** TypeScript (strict mode)
- **UI:** React Navigation 7.x, React Native Maps
- **State Management:** React Context API with useReducer

### Backend & Cloud Services
- **AWS DynamoDB** – NoSQL database (10 tables)
- **AWS S3** – Image and video storage
- **AWS AppSync** – GraphQL API with real-time subscriptions
- **AWS Amplify** – Client library for AppSync integration

## Core Features

### User Authentication & Profiles
- User registration with username/email/password
- Password hashing (SHA256 via expo-crypto)
- Session persistence with AsyncStorage
- Profile picture upload to S3
- Sport ratings and preferences

### Social Networking
- Follow/unfollow users
- Activity feed with posts from all users
- Like/unlike and comment on posts
- Create posts with text, images, and videos
- Location tagging and sport category tags

### Location-Based Discovery
- Nearby users discovery with configurable radius
- Haversine formula for accurate distance calculation
- Privacy-controlled location sharing:
  - **Exact:** Real coordinates
  - **Approximate:** ±1km random offset
  - **Custom:** Manual location pinning
  - **Hidden:** Location not visible
- Interactive map view with user markers

### Real-time Chat
- 1-on-1 private messaging via AWS AppSync
- WebSocket subscriptions for instant delivery (<100ms)
- Conversation list with last message preview
- Auto-scroll and duplicate prevention

### Media Management
- Camera and gallery image/video picking
- Instagram-style compression (75-90% size reduction for images, 80-95% for videos)
- Signed URL generation with 24-hour validity
- Multi-layer caching with automatic expiration

### AI-Powered Form Analysis
- Users upload videos of their sports technique (tennis serve, golf swing, etc.)
- AI analyzes body positioning, movement patterns, and timing
- Generates detailed feedback on form with improvement suggestions
- Highlights areas of strength and areas needing correction
- Enables athletes to track progress over time
- *Currently actively improving analysis accuracy and expanding supported sports*