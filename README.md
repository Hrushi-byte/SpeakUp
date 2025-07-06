# 🎙️ SpeakUp – Voice to Blog Android App

**SpeakUp** is a voice-first social blogging Android application that transforms spoken thoughts into blog-style posts using speech recognition. Built in **Java** with **Firebase** backend integration, the app encourages self-expression and creativity through voice.

---

## 📲 Features

### 🗣️ Voice-to-Blog
- Convert your voice into blog text using Android’s `SpeechRecognizer`
- Edit and polish before publishing

### 👤 User System
- Sign up / log in with Firebase Authentication (email + phone)
- Custom profile with bio, profile picture, username
- Edit profile, privacy settings, delete account

### 📰 Blog Feed
- See your own posts and a **carousel of posts** from other users
- Posts support likes, comments, and timestamps

### ❤️ Social Features
- Like, comment, and follow other users
- View profiles, followers/following stats
- Send and accept friend requests

### 💬 Chat & Notifications
- One-on-one messaging via Firebase Realtime Chat
- Notifications for likes, comments, requests (via Firestore + optional FCM)

### 🔎 Search & Discovery
- Search users by username
- Filter posts by tags or content

### 🔐 Trust & Safety
- Block or report inappropriate users/posts
- Privacy controls: who can see your posts

### ⚙️ Settings
- Theme switching (light/dark)
- Linked accounts (e.g., phone/email)
- Logout / delete account

---

## 🛠️ Tech Stack

| Layer         | Tech                                           |
|--------------|------------------------------------------------|
| Language      | Java                                           |
| UI            | XML + Material Design Components               |
| Backend       | Firebase (Firestore, Auth, Storage, FCM)       |
| Image Handling| Glide                                          |
| Architecture  | Modular Activity-based (with MVVM elements)   |

---



