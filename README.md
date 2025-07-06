🎙️ SpeakUp – Voice to Blog Android App
SpeakUp is a feature-rich, voice-first social blogging app for Android. It empowers users to turn their spoken thoughts into blog-style posts, connect with others, and build a community.

Built using Java, Firebase, and Material Design, SpeakUp demonstrates a complete end-to-end modern Android application.

✨ Features
🗣️ Voice-to-Blog Creation
Speech-to-Text: Use Android’s SpeechRecognizer API to dictate your blog.

Edit & Polish: Refine transcribed text before publishing.

Drafts: Save unfinished posts (planned).

👤 User Management
Authentication:

Email/password sign-up.

Phone number verification via Firebase.

Profile:

Display Name, Username, Bio, Profile Picture.

Followers / Following counts.

Privacy Settings:

Control who can see your posts.

Block/report users.

📰 Blog Feed & Content
Home Feed:

Vertical list of your posts.

Carousel of community posts.

Post Features:

Likes and Comments.

Timestamp display.

Tags and mentions.

Daily Writing Prompts:

Get inspired with fresh ideas.

❤️ Social Features
Likes & Comments:

Engage with posts.

Moderate own comments.

Followers & Following:

Follow users to see their content.

Friend Requests:

Send/accept friend requests.

Profile Viewing:

View others’ profiles and posts.

💬 Real-Time Chat & Notifications
Chat:

One-to-one messaging.

Realtime updates using Firebase.

Notifications:

Likes, comments, and friend requests.

Built with Firestore and optional FCM.

🔎 Search & Discovery
Search Users:

By username.

Search Posts:

By keywords or tags.

⚙️ App Settings
Theme Switching:

Light & Dark mode.

Linked Accounts:

Manage phone/email login.

Logout & Account Deletion:


Full account lifecycle management.

🛠️ Tech Stack
Layer	Details
Language	Java
UI	XML + Material Components
Backend	Firebase Firestore, Auth, Storage, Messaging
Image Handling	Glide
Architecture	MVVM-inspired, modular Activities
Notifications	Firestore + optional FCM


🧭 Data Flow & Architecture
Example Flow: Posting a Blog
User records voice in RecordingActivity.

SpeechRecognizer transcribes audio to text.

User edits text in CreatePostActivity.

Post saved to Firestore under posts collection.

Feed updates dynamically via snapshot listener in HomeActivity.

Example Flow: Chat
User opens chat in ChatActivity.

Messages loaded from Firestore chats collection.

Realtime updates with snapshot listener.

Notifications created in Firestore for recipients.

🚀 Getting Started
Clone the repository:

bash
Copy
Edit
git clone https://github.com/yourusername/SpeakUp.git
Open in Android Studio.

Create google-services.json from Firebase Console and place in /app.

Build and run on an emulator or device.

✉️ Contact
For any questions or feedback:

📧 your.email@example.com
📱 LinkedIn Profile

📄 License
This project is licensed under the MIT License.

🙏 Acknowledgments
Special thanks to:

Google Firebase

Android Developers documentation

Open source libraries (Glide, Material Components)

If you like this project, please ⭐ it and share!

