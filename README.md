🎙️ SpeakUp – Voice-to-Blog Android Application

SpeakUp is a modern, voice-first social blogging platform built for Android. It transforms spoken ideas into polished blog posts, helping users express themselves effortlessly while connecting with a thriving community.

Designed with Java, Firebase, and Material Design, SpeakUp showcases a fully functional, real-world Android application with modular architecture, powerful social features, and smooth UI/UX.

✨ Key Features
🗣️ Voice-to-Blog Creation

Speech-to-Text: Uses Android’s SpeechRecognizer API to convert user speech into text.

Live Transcription: Real-time text generation as the user speaks.

Smart Editing: Users can refine, edit, and format the generated text before publishing.

Draft Mode (Upcoming): Save incomplete posts for later editing.

👤 User Management
🔐 Authentication

Email/password registration & login.

Phone number OTP verification via Firebase Authentication.

🧑 Profile Management

Display Name, Username, Bio, Profile Picture.

Followers and Following counts.

Profile editing with real-time sync.

🔒 Privacy & Safety

Control post visibility (public / followers only).

Block and report users for safety.

📰 Blog Feed & Content System
Home Feed

Vertical feed showing user’s posts.

Horizontal carousel displaying community posts.

Post Capabilities

Like and Comment functionality.

Timestamp display (e.g., "10 mins ago").

Hashtags, mentions, and categorization.

✍️ Daily Writing Prompts

Automatically refreshed prompts to inspire users.

❤️ Social Features
Engagement

Like/unlike posts.

Add, delete, and moderate comments.

Connections

Follow / Unfollow users.

Friend Request system with accept/reject options.

Profiles

View other users’ profiles, their posts, followers, and following list.

💬 Real-Time Chat & Notifications
Realtime Chat

One-to-one messaging using Firestore.

Live typing and message updates via snapshot listeners.

Notifications

Triggered for likes, comments, follows, and friend requests.

Built using Firestore triggers and optional Firebase Cloud Messaging (FCM).

🔎 Search & Discovery

User Search: Find users by username.

Post Search: Search posts via keywords, tags, or hashtags.

Instant suggestions and fast lookup with Firestore indexing.

⚙️ App Settings

Theme Switching: Toggle between Light Mode and Dark Mode.

Linked Accounts: Manage email & phone-linked logins.

Session Management: Logout, deactivate, or permanently delete account.

🛠️ Tech Stack & Architecture
Language:

Java

UI:

XML layouts with Material Components, RecyclerViews, BottomNavigation, and modern UI patterns.

Backend Services:

Firebase Authentication – User login/registration

Cloud Firestore – Posts, users, chats, notifications

Firebase Storage – Images, profile pictures

Firebase Cloud Messaging (optional) – Push notifications

Image Loading:

Glide (optimized caching and async loading)

Architecture Pattern:

MVVM-inspired modular structure

Clean separation of Activities, ViewModels, Repositories & Utils

Real-time data with Firestore snapshot listeners

🧭 Workflow Examples
🔄 Blog Creation Flow

User records audio in RecordingActivity.

Audio is processed via SpeechRecognizer → converted into text.

User edits text in CreatePostActivity.

Post is uploaded to Firestore under /posts/.

Home feed auto-updates due to snapshot listeners in HomeActivity.

💬 Chat Flow

User opens ChatActivity.

App loads message history from /chats/.

Firestore snapshot listener streams new messages instantly.

Notification entry created for the receiver via Firestore/FCM.
