# 🎵 Lokal Music Player

A modern Android music player application built using **Kotlin + Jetpack Compose**, focused on clean UI, smooth playback, and robust state handling.

---

## 🚀 Features

### Queue Management
- Add songs to queue  
- Remove songs from queue  
- Reorder songs in queue (drag & drop)  
- Current queue persists locally  

### Media Playback
- Play / Pause / Next / Previous  
- Background playback support  
- Media notification controls  
- Handles audio focus & interruptions  

### UI
- Modern Material 3 design  
- Smooth scrolling lists  
- Responsive layout for different screen sizes  
- Light/Dark theme support  

---


### Layers

| Layer | Responsibility |
|------|----------------|
| UI (Compose) | Display data & user interactions |
| ViewModel | Business logic & state |
| Data | Media handling, repositories |

This ensures:
- Separation of concerns  
- Testable components  
- Easy scalability  

---

## 💾 Local Persistence

Queue state is stored locally using:
- In-memory cache + saved state  

Queue survives:
- Screen rotations  
- Navigation between screens  

---

## ⚙️ Setup Instructions

### Prerequisites
- Android Studio Flamingo or newer  
- Android SDK 31+  
- Kotlin 1.8+  

### Steps
```bash
git clone https://github.com/Sonakshi241004/Lokal_MusicPlayer.git
cd Lokal_MusicPlayer



