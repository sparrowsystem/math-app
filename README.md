# Math App: A Unified Gamified Educational Ecosystem 🚀

<div align="center">
  <img src="https://sparrowsystemsug.com/img/logo.png" alt="Math App Logo" width="150">
  <p>
    <b>Transforming math drills into an immersive, multi-platform adventure.</b>
  </p>
  <p>
    <a href="https://sparrowsystemsug.com/">Official Website</a> •
    <a href="#-market-research-vision">The Vision</a> •
    <a href="#-core-features">Features</a> •
    <a href="#-getting-started">Installation</a>
  </p>

  <!-- Technology Badges -->
  [![Kotlin](https://img.shields.io/badge/Android-Kotlin-7F52FF?style=for-the-badge&logo=kotlin&logoColor=white)](https://kotlinlang.org/)
  [![Swift](https://img.shields.io/badge/iOS-Swift-F05138?style=for-the-badge&logo=swift&logoColor=white)](https://developer.apple.com/swift/)
  [![PHP](https://img.shields.io/badge/Backend-PHP-777BB4?style=for-the-badge&logo=php&logoColor=white)](https://www.php.net/)
  [![OpenCV](https://img.shields.io/badge/Vision-OpenCV%20API-5C3EE8?style=for-the-badge&logo=opencv&logoColor=white)](https://opencv.org/)
  [![MySQL](https://img.shields.io/badge/Database-MySQL-4479A1?style=for-the-badge&logo=mysql&logoColor=white)](https://www.mysql.com/)
</div>

---

## 📖 Market Research & Vision

Based on our **Market Research Report**, we identified that while exercise and productivity apps have limitations in isolation, their greatest potential lies in **Educational Gamification**. 

The **Math App** is a unified solution that bridges the gap between digital play and real-world learning. We have moved away from regional SAT/ACT drills to create a universal curriculum that helps parents and children master math through:
1.  **Gamified Progression:** Making study feel like a game.
2.  **Productivity Modules:** Utilizing Computer Vision for real-world interaction.
3.  **Competition:** Fostering community through speed challenges.

---

## 🌟 Core Features

### 🎮 Gamified Learning & Competition
*   **Structured Curriculum:** Multi-level system starting at **Level 1**, mirroring school progression from basic arithmetic to Fractions, Algebra, and Geometry.
*   **Speed Challenges:** Local and Global leaderboards inspired by exercise mechanics to drive international connectedness and local pride.
*   **Gameplay Obstacles:** Progress is unlocked by solving math problems; correct answers provide "boosters" while incorrect answers require reinforcement lessons.

### 🛠️ Productivity Modules (The Real-World Bridge)
*   **Object Counter:** A computer-vision tool allowing children to count physical objects using the camera, reinforcing tangible math concepts.
*   **Paper Grader:** Allows students to solve problems on paper and instantly verify their work via the app, bridging handwriting with digital feedback.

### 🤖 Support & Tutoring
*   **AI-Driven Support:** Real-time encouragement and personalized lessons generated specifically for a child's weak areas.
*   **Professional Access:** Integrated portal for parents to connect with human teachers for tailored academic guidance.

---

## 🛠️ Technical Stack

### **Client-Side (Mobile)**
*   **Android:** Kotlin (Native)
*   **iOS:** Swift (Native)
*   **Architecture:** MVVM for both platforms to ensure consistent logic.

### **Server-Side (Backend)**
*   **API:** PHP (Server-side logic and data orchestration)
*   **Database:** MySQL (User progress, levels, and global rankings)
*   **Vision:** OpenCV API (Powering the Object Counter and Paper Grader)

---

## 🏁 Getting Started

This repository contains the source code for the Android/iOS clients and the PHP backend.

### 1. Backend Setup (PHP/MySQL)
1.  Ensure you have **XAMPP** or **WAMP** running.
2.  Import `database.sql` into your MySQL server via phpMyAdmin.
3.  Configure your `.env` or `config.php` file with your local database credentials.
4.  Ensure the OpenCV API endpoint is accessible.

### 2. Android Setup (Kotlin)
1.  Open the `/android` folder in **Android Studio**.
2.  Update the `BASE_URL` in your network configuration to point to your machine's local IP (e.g., `http://192.168.x.x/api`).
3.  Build and run on an emulator or physical device.

### 3. iOS Setup (Swift)
1.  Open the `/ios` folder in **Xcode**.
2.  Run `pod install` (if using CocoaPods).
3.  Update the API endpoint in your Swift networking layer.
4.  Build and run on a Simulator or iPhone.

---

## 📂 Project Structure

```text
├── android/            # Kotlin source code (Android Studio Project)
├── ios/                # Swift source code (Xcode Project)
├── backend/            # PHP API logic and OpenCV integration
├── database/           # MySQL schema files
└── documentation/      # Market Research Reports and Storyboarding
