\# Math App: Gamified Educational Ecosystem 🚀

<div align="center">
  <img src="https://sparrowsystemsug.com/img/logo.png" alt="Math App Logo" width="150">
  <p>
    <b>A unified educational platform bridging digital gaming and real-world math learning.</b>
  </p>
  <p>
    <a href="https://sparrowsystemsug.com/">View Website</a> •
    <a href="#-getting-started">Installation</a> •
    <a href="#-features">Features</a> •
    <a href="#-contributing">Contribute</a>
  </p>

  [![PHP Version](https://img.shields.io/badge/PHP-7.4%2B-777BB4?style=flat-square&logo=php)](https://www.php.net/)
  [![MySQL](https://img.shields.io/badge/Database-MySQL-4479A1?style=flat-square&logo=mysql&logoColor=white)](https://www.mysql.com/)
  [![Bootstrap](https://img.shields.io/badge/UI-Bootstrap%205-7952B3?style=flat-square&logo=bootstrap&logoColor=white)](https://getbootstrap.com/)
  [![OpenCV API](https://img.shields.io/badge/Vision-OpenCV%20API-5C3EE8?style=flat-square&logo=opencv&logoColor=white)](https://opencv.org/)
  [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
</div>

---

## 📖 Project Overview

The **Math App** is an innovative educational tool developed from extensive market research. It addresses the limitations of traditional learning by blending gamified progression with real-world productivity modules. 

The core of the app is a structured, multi-level system that mirrors school curricula—starting from Level 1 (counting/basic arithmetic) and advancing to complex topics like algebra and geometry. By integrating competition and AI-driven feedback, the app transforms math from a chore into an engaging challenge.

### 🌟 Key Features

*   **Gamified Curriculum:** Multi-level progression system (Level 1+) where advancement requires mastery of foundational topics.
*   **Competitive Drills:** "Speed Challenge" modules allowing students to compete in local and global leaderboards.
*   **Computer Vision (OpenCV Integration):**
    *   **Object Counter:** Use the camera to count real-world physical objects for tangible math practice.
    *   **Paper Grader:** Solve problems on paper and use the app to instantly verify results using AI vision.
*   **AI-Driven Tutor:** Real-time encouragement and lesson generation targeting a child's specific weak areas.
*   **Teacher/Parent Portal:** Built-in options to connect with professional tutors for tailored guidance.

---

## 🛠️ Tech Stack

This project is built using a reliable LAMP/WAMP-style architecture:

*   **Frontend:** HTML5, CSS3, JavaScript (ES6+), Bootstrap 5
*   **Backend:** PHP
*   **Database:** MySQL
*   **Vision Processing:** OpenCV (consumed via external API)
*   **Environment:** XAMPP, WAMP, or any Apache/PHP/MySQL stack.

---

## 🏁 Getting Started

This repository is intended for developers. Follow these steps to set up the local development environment.

### 1. Prerequisites
Ensure you have a local server installed:
*   [XAMPP](https://www.apachefriends.org/) (Windows/Linux/macOS)
*   [WAMP](https://www.wampserver.com/) (Windows)

### 2. Installation
1.  **Clone the repository:**
    ```bash
    git clone https://github.com/your-username/math-app.git
    ```
2.  **Move the project:**
    Copy the project folder into your local server's root directory:
    *   XAMPP: `C:/xampp/htdocs/math-app`
    *   WAMP: `C:/wamp64/www/math-app`

### 3. Database Setup
1.  Open **phpMyAdmin** (`http://localhost/phpmyadmin`).
2.  Create a new database named `math_app_db`.
3.  Import the `database.sql` file provided in the root folder of this repository.

### 4. Configuration
1.  Locate the `.env` and `config.php` files in the project root.
2.  Edit your database credentials:
    ```php
    define('DB_HOST', 'localhost');
    define('DB_USER', 'root');
    define('DB_PASS', 'your_password');
    define('DB_NAME', 'math_app_db');
    ```
3.  Set the `OPENCV_API_ENDPOINT` in your configuration to connect to the computer vision service.

### 5. Launch
Open your browser and navigate to:
```text
http://localhost/math-app/index.php
