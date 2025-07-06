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


some UI images :
![Screenshot_20250706-213309](https://github.com/user-attachments/assets/598345f2-64e4-4742-b23f-e64b7a674c31)
![Screenshot_20250706-213253](https://github.com/user-attachments/assets/8044d2e2-5f6b-4d68-b7bb-dfbc7a82f2a9)
![Screenshot_20250706-213244](https://github.com/user-attachments/assets/b4f0f891-eaf5-4475-b272-eb803401ffc1)
![Screenshot_20250706-213239](https://github.com/user-attachments/assets/98e39409-2539-4780-bab6-4b31935b1b7f)
![Screenshot_20250706-213226](https://github.com/user-attachments/assets/e25fc4bc-071d-4242-a5bf-ecd1499bd898)
![Screenshot_20250706-213208](https://github.com/user-attachments/assets/2e64306c-8767-4206-a598-87bbb883ac2c)
![Screenshot_20250706-213204](https://github.com/user-attachments/assets/d770cbca-f6c6-449f-b8c7-9d768c372f45)
![Screenshot_20250706-213156 (1)](https://github.com/user-attachments/assets/95e60e13-4a98-4096-9f17-ca73cdac1f3f)
![Screenshot_20250706-213153 (1)](https://github.com/user-attachments/assets/21659196-4e76-4fc8-8a83-556ac86c3690)
![Screenshot_20250706-213128](https://github.com/user-attachments/assets/f8314e74-fc79-451e-9d7d-d02d664ed782)

Full account lifecycle management.

🛠️ Tech Stack
Layer	Details
Language	Java
UI	XML + Material Components
Backend	Firebase Firestore, Auth, Storage, Messaging
Image Handling	Glide
Architecture	MVVM-inspired, modular Activities
Notifications	Firestore + optional FCM

📂 Project Structure (Detailed)
bash
Copy
Edit
/app/src/main/java/com/example/speakup/

├── activities/
│   ├── ChatActivity                 # Single chat conversation
│   ├── ChatListActivity             # List of user conversations
│   ├── CommentsActivity             # Post comments
│   ├── CreatePostActivity           # Voice-to-blog creation
│   ├── DailyPromptActivity          # Daily writing prompt
│   ├── EditProfileActivity          # Edit profile screen
│   ├── EntryDetailsActivity         # Detailed post view
│   ├── FriendRequestsActivity       # Manage friend requests
│   ├── HomeActivity                 # Main feed & navigation
│   ├── LoginActivity                # User login
│   ├── NotificationsActivity        # Notification center
│   ├── PhoneAuthActivity            # Phone number login
│   ├── ProfileActivity              # User profile display
│   ├── RecordingActivity            # Speech recording
│   ├── SearchActivity               # General search
│   ├── SearchUserActivity           # Search users
│   ├── SettingsActivity             # Preferences & themes
│   ├── SignUpActivity               # Registration
│   ├── SplashActivity               # App splash screen
│   ├── SupportActivity              # Help & support
│   └── TagUserActivity              # Tag users in posts
│
├── adapters/
│   ├── AllUserAdapter               # All users list
│   ├── CarouselAdapter              # Carousel of posts
│   ├── ChatAdapter                  # Chat messages
│   ├── CommentsAdapter              # Post comments
│   ├── EntriesAdapter               # Blog entries
│   ├── FriendRequestsAdapter        # Friend request items
│   ├── NotificationsAdapter         # Notifications
│   ├── SearchUserAdapter            # Search results
│   └── UserTagAdapter               # Tagging
│
├── models/
│   ├── Chat                         # Chat message model
│   ├── Friend                       # Friendship model
│   ├── FriendRequest                # Friend request data
│   ├── NotificationItem             # Notification data
│   ├── Post                         # Blog post model
│   ├── PromptModel                  # Daily prompt
│   ├── User                         # User profile
│   └── UserChatSummary              # Chat summaries
│
├── utils/
│   └── FirebaseUtils                # Firebase helper utilities
│
├── SpeakUpApp.java                  # Application entry point
📁 Resources
pgsql
Copy
Edit
/res/
├── layout/
│   ├── activity_*.xml               # Activity layouts
│   ├── item_*.xml                   # RecyclerView items
│   ├── chat_item_*.xml              # Chat bubbles
│
├── menu/
│   ├── bottom_nav_menu.xml
│   ├── home_menu.xml
│   └── top_app_bar_menu.xml
│
├── values/
│   ├── colors.xml
│   ├── strings.xml
│   ├── styles.xml
│   └── themes/
│
├── mipmap/                          # Icons
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

