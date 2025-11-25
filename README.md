# 🎙️ SpeakUp – Voice-to-Blog Social Media Android Application

## Overview
SpeakUp is a modern, voice-first social blogging Android application that allows users to convert their spoken thoughts into blog-style posts. It provides a complete social media experience with voice-to-text post creation, user profiles, follows, likes, comments, real-time chat, post discovery, and notifications — all built using Java, Firebase, and Material Design.

## Features
- **Voice-to-Blog Creation:** Speech-to-text conversion using Android’s SpeechRecognizer API, real-time transcript generation, built-in text editor, and support for tags, mentions, and hashtags. Draft-saving system planned.
- **User Authentication:** Signup/Login using Firebase Authentication with email and password.
- **User Profiles:** Editable profile including username, display name, bio, and profile picture. View followers/following counts and manage connections.
- **Blog Feed & Posts:** Vertical home feed for personal posts and horizontal explore carousel for community posts. Post interactions include likes, comments, timestamps, and post analytics.
- **Social Features:** Like/unlike posts, add/delete comments, follow/unfollow users, send/accept/decline friend requests, and view other users' profiles and posts.
- **Real-Time Chat:** One-to-one messaging with Firestore snapshot listeners for instant updates. Optional typing indicators and FCM-based push notifications.
- **Search & Discovery:** Search users by username and search posts using keywords or tags. Firestore's indexed queries ensure fast and accurate results.
- **App Settings:** Light/Dark mode, manage linked accounts, logout, delete account, and clear local cache.

## Tech Stack
- **Language:** Java
- **IDE:** Android Studio
- **UI:** XML + Material Components
- **Backend:** Firebase Authentication, Firestore Database, Firebase Storage
- **Notifications:** Firebase Cloud Messaging (optional)
- **Image Loading:** Glide
- **Architecture:** MVVM-inspired modular design
- **Realtime Updates:** Firestore snapshot listeners
- **Utilities:** SharedPreferences, ViewModels, Repositories

## Architecture
- Modular package design with separate folders for: `activities/`, `adapters/`, `models/`, `repositories/`, `utils/`, `viewmodels/`
- RecyclerView adapters used throughout the app for dynamic lists (posts, messages, notifications)
- Clean separation of UI, data, and logic layers
- Firestore integration for real-time updates across: posts, comments, chat, followers, notifications

## Workflow Examples
- **Voice-to-Blog Flow:**
  1. User records voice → SpeechRecognizer transcribes audio.
  2. Transcribed text is displayed in the editor.
  3. User edits text and adds tags/mentions.
  4. Post is uploaded to Firestore under `/posts`.
  5. Home feed updates instantly via snapshot listener.
- **Chat Flow:**
  1. User opens `ChatActivity`.
  2. Messages are fetched from Firestore `/chats/{chatId}/messages`.
  3. Snapshot listener updates messages in real-time.
  4. Notification entry is created for the recipient (Firestore/FCM).
  5. Receiver gets an instant alert.

  <img width="500" height="1000" alt="1" src="https://github.com/user-attachments/assets/51ffb207-f6a8-42ed-b665-d7b8a09a0e90" />

  <img width="500" height="1000" alt="2" src="https://github.com/user-attachments/assets/a32425a5-a49a-46f8-aa1e-e70f4de001de" />

  <img width="500" height="1000" alt="3" src="https://github.com/user-attachments/assets/9bcb19aa-c981-4492-bee9-0af212a8836e" />

  <img width="500" height="1000" alt="4" src="https://github.com/user-attachments/assets/4d087770-1378-47e1-80c4-4c97d2c3d452" />

  <img width="500" height="1000" alt="5" src="https://github.com/user-attachments/assets/b195979a-c78f-43cb-a394-454f193cbce4" />

  <img width="500" height="1000" alt="6" src="https://github.com/user-attachments/assets/778b6f0e-2b2b-4bd4-a938-92d60ab530a5" />

  <img width="500" height="1000" alt="7" src="https://github.com/user-attachments/assets/cd159cbc-84d7-495c-a485-a1b078de0424" />

  <img width="500" height="1000" alt="8" src="https://github.com/user-attachments/assets/a0ac7464-c3eb-4273-96c9-05ad0f51b2cb" />

  <img width="500" height="1000" alt="9" src="https://github.com/user-attachments/assets/d11aa762-1ac1-4dd2-b634-4accccd095d9" />

  <img width="500" height="1000" alt="10" src="https://github.com/user-attachments/assets/2d0d7ffb-a0fb-4b79-98e5-c7c40d63ab93" />









