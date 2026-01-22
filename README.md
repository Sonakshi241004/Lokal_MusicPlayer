🎵 Lokal Music Player

A modern Android music player application built using Kotlin + Jetpack Compose, focused on clean UI, smooth playback, and robust state handling.

🚀 Features
Queue Management

Add songs to queue

Remove songs from queue

Reorder songs in queue (drag & drop)

Current queue persists locally

Media Playback

Play / Pause / Next / Previous

Background playback support

Media notification controls

Handles audio focus & interruptions

UI

Modern Material 3 design

Smooth scrolling lists

Responsive layout for different screen sizes

Light/Dark theme support

🧠 Architecture Overview

The project follows MVVM + Clean Architecture principles:

com.example.musicplayer
│
├── data/          → Repositories, data sources
├── di/            → Dependency Injection
├── presentation/ → Activities & Compose UI
├── viewmodel/     → State holders (ViewModels)

Layers
Layer	Responsibility
UI (Compose)	Display data & user interactions
ViewModel	Business logic & state
Data	Media handling, repositories

This ensures:

Separation of concerns

Testable components

Easy scalability

💾 Local Persistence

Queue state is stored locally using:

In-memory cache + saved state

Queue survives:

Screen rotations

Navigation between screens

⚙️ Setup Instructions
Prerequisites

Android Studio Flamingo or newer

Android SDK 31+

Kotlin 1.8+

Steps
git clone https://github.com/Sonakshi241004/Lokal_MusicPlayer.git
cd Lokal_MusicPlayer


Open in Android Studio → Sync → Run on emulator or device.

📦 APK

APK available in:

/app/release/app-release.apk


(Or generate via: Build → Generate Signed APK)

🎥 Demo Video

2–3 minute demo showing:

App launch

Playing songs

Queue operations

Background playback

(Attach Google Drive / YouTube link here)

⚠️ Assumptions & Trade-offs
Assumptions

User has audio files or streaming source available

Single active playback session

No user authentication

Trade-offs
Choice	Reason
No database	Simpler state handling
Local queue only	Avoids backend complexity
Media3	Modern, reliable playback
🧪 Error & Edge Case Handling

Handled:

No internet / no media

Empty queue

App backgrounded

Incoming calls / audio interruptions

📊 Evaluation Mapping
Criteria	How it’s addressed
Architecture	MVVM + Clean layers
Media reliability	Media3 + foreground service
UI accuracy	Material 3 + Compose
Performance	LazyColumn + state hoisting
State handling	ViewModels + SavedState
Error handling	Graceful fallbacks
Code quality	Modular & readable
👩‍💻 Author

Sonakshi
Computer Science & Engineering
GitHub: https://github.com/Sonakshi241004

📝 License

This project is for educational and demonstration purposes.

