# Math App: Gamified Educational Mobile Ecosystem 🚀

<div align="center">
  <img src="https://sparrowsystemsug.com/img/logo.png" alt="Math App Logo" width="150">
  <p>
    <b>A native Android educational platform bridging digital gaming and real-world math learning.</b>
  </p>
  <p>
    <a href="https://sparrowsystemsug.com/">View Website</a> •
    <a href="#-getting-started">Setup Guide</a> •
    <a href="#-features">Features</a> •
    <a href="#-contributing">Contribute</a>
  </p>

  [![Kotlin](https://img.shields.io/badge/Language-Kotlin-7F52FF?style=flat-square&logo=kotlin&logoColor=white)](https://kotlinlang.org/)
  [![Android](https://img.shields.io/badge/Platform-Android-3DDC84?style=flat-square&logo=android&logoColor=white)](https://developer.android.com/)
  [![OpenCV](https://img.shields.io/badge/Vision-OpenCV%20SDK-5C3EE8?style=flat-square&logo=opencv&logoColor=white)](https://opencv.org/)
  [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
</div>

---

## 📖 Project Overview

The **Math App** is a native Android application built in **Kotlin**. Developed from extensive market research, it transforms traditional math education into an immersive mobile gaming experience. 

The app features a structured, multi-level progression system (starting at Level 1) that mirrors school curricula. By leveraging mobile hardware, it integrates **Computer Vision** to bridge the gap between digital drills and physical classroom work (handwritten paper and physical objects).

### 🌟 Key Features

*   **Gamified Learning Path:** Multi-level progression (Level 1+) where users "level up" by mastering arithmetic, algebra, and geometry.
*   **Mobile Speed Challenges:** Competitive local and global leaderboards to foster community and drive engagement.
*   **On-Device Computer Vision (OpenCV):**
    *   **Object Counter:** Uses the smartphone camera to detect and count physical objects for interactive learning.
    *   **Paper Grader:** Scan handwritten math problems to receive instant AI-driven verification.
*   **AI Tutor:** Provides real-time feedback and dynamically generates lessons based on the user's performance.
*   **Parent/Teacher Portal:** Secure module to track progress and connect with professional tutoring services.

---

## 🛠️ Tech Stack

*   **Language:** Kotlin
*   **Platform:** Android (Min SDK 24+)
*   **Architecture:** MVVM (Model-View-ViewModel)
*   **UI Framework:** Jetpack Compose (or XML Layouts)
*   **Networking:** Retrofit / OkHttp (to consume the PHP/MySQL API)
*   **Computer Vision:** OpenCV Android SDK
*   **Local Database:** Room Persistence Library

---

## 🏁 Getting Started

Follow these steps to set up the development environment on your machine.

### 1. Prerequisites
*   **Android Studio** (Latest version recommended: Jellyfish or newer)
*   **JDK 17** or higher
*   **Android SDK** (API Level 34 target)
*   **PHP/MySQL Backend:** Ensure your backend API is running (via XAMPP/WAMP) so the mobile app can sync data.

### 2. Installation
1.  **Clone the repository:**
    ```bash
    git clone https://github.com/your-username/math-app-kotlin.git
    ```
2.  **Open in Android Studio:**
    - File > Open > Select the cloned folder.
3.  **Sync Project:**
    - Wait for Gradle to finish syncing and downloading dependencies.

### 3. Configuration
1.  Locate the `Constants.kt` or `network_config.xml` file.
2.  Update the `BASE_URL` to point to your local PHP server IP:
    ```kotlin
    val BASE_URL = "http://192.168.x.x/math-app-api/" 
    ```
    *(Note: Do not use 'localhost' inside an Android emulator; use your machine's local IP address).*

### 4. Running the App
1.  Connect a physical Android device or launch the **Android Emulator**.
2.  Press the **Run** button in Android Studio.

---

## 📂 Project Structure

```text
├── app/
│   ├── src/main/java/com/mathapp/
│   │   ├── ui/             # Jetpack Compose Screens/Fragments
│   │   ├── viewmodel/      # Business logic and state management
│   │   ├── data/           # Repositories and Room Database
│   │   └── vision/         # OpenCV implementations (Object Counter)
│   ├── src/main/res/       # Layouts, Drawables, and Strings
│   └── build.gradle.kts    # Project dependencies
└── README.md
