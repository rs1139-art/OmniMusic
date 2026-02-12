🎵 OmniMusic
OmniMusic is a modern Android music application inspired by Spotify that unifies music across multiple streaming platforms.

It connects to Spotify, Amazon Music, and YouTube Music using official APIs and enables users to securely import, merge, and manage their playlists in one centralized app.

Built using Kotlin, Jetpack Compose, Clean Architecture, MVVM, and modern Android development best practices, OmniMusic focuses on scalability, security, and cross-platform music unification.

🚀 Features
🔐 Secure Multi-Platform Authentication
Spotify OAuth (PKCE)

Google OAuth (YouTube Music)

Amazon Login (if API access available)

Encrypted token storage using Android Keystore

🎶 Unified Playlist Import
Import playlists from:

Spotify

YouTube Music

Amazon Music (if API available)

Intelligent duplicate detection

ISRC-based track matching

Fuzzy metadata matching (Title + Artist)

Cross-platform playlist merging

🔍 Cross-Platform Search
Search music metadata across connected services in one unified interface.

💾 Local Data Persistence
Room Database

Cached metadata

Playlist history

Secure storage of tokens

🎨 Modern UI
Jetpack Compose

Material 3

Dark Mode support

Responsive layout

⚙ Clean Architecture
MVVM pattern

Repository abstraction

Dependency Injection (Hilt)

Retrofit networking

Coroutines & Flow

🏗 Architecture Overview
OmniMusic follows Clean Architecture principles:

Presentation Layer (Compose UI + ViewModels)
        ↓
Domain Layer (Use Cases)
        ↓
Data Layer (Repositories)
        ↓
Network + Database
The app abstracts each streaming platform behind a unified MusicRepository, enabling future expansion.

🔒 Security & Compliance
No DRM bypassing

Uses only officially permitted APIs

Tokens stored securely

API keys not hardcoded

Environment-based configuration

OmniMusic respects rate limits and platform terms of service.

🛠 Tech Stack
Kotlin

Jetpack Compose

MVVM + Clean Architecture

Hilt (Dependency Injection)

Retrofit

Room Database

Coroutines & Flow

Gradle

Optional backend:

Node.js / Firebase (for secure token exchange)

📦 Build Instructions
Clone repository

Add your API keys in local.properties

Enable Spotify & Google Developer access

Sync Gradle

Build APK

./gradlew assembleRelease
🔑 API Requirements
You must register developer applications for:

Spotify Developer Dashboard

Google Cloud Console (YouTube Data API v3)

Amazon Developer Console (if access granted)

🎯 Project Goals
Provide a unified cross-platform music management experience

Eliminate playlist fragmentation

Maintain compliance with streaming service policies

Demonstrate production-grade Android architecture

📌 Roadmap
Smart recommendation engine

AI-powered playlist blending

Social sharing

Cloud sync

Web dashboard version

Analytics dashboard

⚠ Limitations
Full music playback may be restricted by API terms

Amazon Music API access may require approval

YouTube Music integration uses YouTube Data API where applicable

🤝 Contributing
Pull requests are welcome. Please follow clean architecture principles and ensure all code is production-ready.

📜 License
MIT License (or choose appropriate license)
