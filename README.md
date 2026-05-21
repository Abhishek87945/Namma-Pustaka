# Abhishek Library Management System (Namma Pustaka)

Welcome to the **Abhishek Library Management System** (formerly known as *Namma Pustaka*), a robust, state-of-the-art Android application designed to streamline library book tracking, barcode scanning, and student activity logs. Built with modern Android development paradigms, this project is fully configured, clean, and ready to be pushed directly to **GitHub** and opened in **Android Studio**.

---

## 🌟 Key Features

The app is packed with premium features aimed at making library management smooth and interactive:

- **📚 Comprehensive Cataloging (Books Screen)**: Search, view, and navigate through a vast collection of cataloged books. Modern and responsive Jetpack Compose card views display cover art and status.
- **📷 Barcode Scanning (Scan Screen)**: Integrated with **Google ML Kit Barcode Scanning** and **Android CameraX** to quickly scan barcodes for issuing or returning books.
- **📊 Real-time Analytics & Transaction Log (History Screen)**: A beautiful timeline showing chronologically sorted book transactions (check-ins and check-outs) with exact timestamps.
- **👥 Student Management (Students Screen)**: Manage student names, IDs, departments, and active check-out counts in a cleanly organized list.
- **🏆 Gamified Engagement (Ranking / Leaderboard Screen)**: A dedicated leaderboard ranking students based on the number of books read, fostering a healthy culture of reading!
- **➕ Dynamic Book Addition (Add Book Screen)**: A user-friendly form to add new books to the repository with customized metadata fields (title, author, ISBN, copies, cover image URL, etc.).
- **⚙️ Deep Room Integration**: All entities (Books, Students, Transactions) are fully backed by an offline-first **Room Database** utilizing asynchronous Kotlin Coroutines for seamless performance.

---

## 🛠️ Technology Stack

- **UI Framework**: [Jetpack Compose](https://developer.android.com/compose) (declarative modern UI development)
- **Programming Language**: [Kotlin](https://kotlinlang.org/)
- **Local Persistence**: [Room SQLite Database](https://developer.android.com/training/data-storage/room)
- **Scanning Technology**: [Google ML Kit Barcode Detection](https://developers.google.com/ml-kit/vision/barcode-scanning) & [CameraX API](https://developer.android.com/training/camerax)
- **Dependency Management**: [Gradle Version Catalogs](https://developer.android.com/build/migrate-to-catalogs) (Kotlin DSL)
- **Networking/Image Loading**: [Coil Compose](https://coil-kt.github.io/coil/) (modern image loading for Jetpack Compose)
- **Architecture Pattern**: MVVM (Model-View-ViewModel) with structured package segregation.

---

## 🚀 Setup & Android Studio Instructions

This project is configured to run flawlessly on the latest version of **Android Studio (Ladybug / Koala or newer)**.

### Prerequisites

1. **Android Studio**: Ensure you have Android Studio installed.
2. **JDK**: JDK 17 or newer (configured automatically within Android Studio).
3. **Android SDK**: Compile SDK is set to version **34**, and the minimum supported Android SDK is **26** (Android 8.0 Oreo).

### Opening in Android Studio

1. Launch **Android Studio**.
2. Select **Open** (or **File > Open**).
3. Navigate to the directory containing this project (`abhishek`) and click **OK**.
4. Allow Gradle to sync dependencies and index the project (this may take 1-2 minutes).
5. Build the project using **Build > Make Project** or click the **Run** button (green play icon) to deploy the app to your Emulator or physical device.

---

## 📁 Repository Directory Structure

```
abhishek/
├── app/
│   ├── src/
│   │   ├── main/
│   │   │   ├── java/com/example/abhishek/      # Refactored Source Package
│   │   │   │   ├── MainActivity.kt             # Main entry point with Compose NavHost
│   │   │   │   ├── data/                       # Room Entities, DAOs, Database definitions
│   │   │   │   ├── ui/                         # Jetpack Compose Screens and UI Theme
│   │   │   │   └── viewmodel/                  # MVVM ViewModels
│   │   │   └── AndroidManifest.xml             # Permissions & App metadata
│   │   └── test/ & androidTest/                # Local and Instrumented unit tests
│   └── build.gradle.kts                        # App module configurations
├── gradle/
│   └── libs.versions.toml                      # Version catalogs (libs declaration)
├── settings.gradle.kts                         # Root Gradle settings (Project renamed)
└── README.md                                   # Documentation (this file!)
```

---

## 📦 Publishing to GitHub

To put this project on your personal GitHub, open your terminal inside the project root folder and execute the following commands:

```bash
# 1. Initialize local Git repository (Already initialized for you)
git init

# 2. Stage all files (Build/temporary files are ignored automatically by .gitignore)
git add .

# 3. Create your first commit
git commit -m "Initial commit: Rename project and packages to abhishek, ready for production"

# 4. Link your local repository to your remote GitHub repository
git remote add origin https://github.com/YOUR_GITHUB_USERNAME/YOUR_REPOSITORY_NAME.git

# 5. Rename primary branch to main (Standard convention)
git branch -M main

# 6. Push code to GitHub
git push -u origin main
```

---

*Made with ❤️ by Abhishek. Happy Coding!*
