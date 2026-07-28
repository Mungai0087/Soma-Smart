# Soma Smart 🧠📚

**Soma Smart** is an AI-powered, offline-first mobile learning application tailored specifically for Kenya's Competency-Based Curriculum (CBC) transition for primary and junior secondary students. Built natively with modern Android technologies (Kotlin & Jetpack Compose), Soma Smart delivers localized curriculum content, AI-driven study assistance, offline practice quizzes, gamified progression, and printable PDF report card generation.

---

## ✨ Core Features

* **📚 CBC Curriculum Alignment:**
  * Comprehensive coverage for Grade 1 through Grade 9 subjects (Mathematics, English, Kiswahili, Science & Technology, Social Studies, Agriculture, and Creative Arts).
  * KICD-compliant lesson structures, topic summaries, and practice exercises.

* **🤖 AI-Powered Learning Assistant (Gemini API Integration):**
  * **Soma AI Smart Quiz Generator:** Automatically generates interactive quizzes tailored to specific subjects and difficulty levels.
  * **Interactive AI Study Tutor:** Real-time conversational tutor providing step-by-step explanations, Swahili/English bilingual support, and conceptual breakdowns.

* **📴 Offline-First Architecture:**
  * Powered by **Room Database** for complete offline lesson caching, quiz history, XP tracking, and streak counts.
  * **Offline JSON Backup & Restore:** Export and import full study progress locally without relying on continuous internet connectivity.

* **📄 Printable PDF Exam Sheets & Progress Reports:**
  * **Assessment Reports:** Export completed quiz attempts and detailed answer keys with explanations into standard, printable PDF documents directly from device memory.
  * **Academic Progress Report Cards:** Generate official CBC student performance reports complete with subject score breakdowns, study goal meters, and parent action plans.

* **🎮 Gamification & Engagement:**
  * XP point accumulation, streak counters, weekly study minute targets, and unlockable achievement badges.
  * Daily Quick Quiz Challenges and traditional Swahili proverbs (*Methali za Kiswahili*) for culturally resonant motivation.

* **💳 Premium Subscription & M-Pesa Integration:**
  * Direct **Lipa na M-Pesa STK Push** dialogs with Paybill support (Paybill 400200 / Co-operative Bank) and secure credit card checkout simulation.

---

## 🛠️ Tech Stack & Architecture

* **Language:** [Kotlin](https://kotlinlang.org/)
* **UI Framework:** [Jetpack Compose](https://developer.android.com/jetpack/compose) with Material Design 3 (M3)
* **Architecture:** MVVM (Model-View-ViewModel) + Clean Architecture principles
* **Local Persistence:** [Room Database](https://developer.android.com/training/data-storage/room) with KSP
* **Asynchronous Operations:** Kotlin Coroutines & `StateFlow` / `collectAsStateWithLifecycle`
* **AI Engine:** Google Gemini REST API / Server-Side Gemini API
* **Document Engine:** Android Native `PdfDocument` framework
* **Testing:** Robolectric & Roborazzi screenshot verification

---

## 🚀 Getting Started

### Prerequisites

* **Android Studio:** Ladybug (2024.2.1) or newer recommended
* **JDK:** Version 17 or higher
* **Android SDK:** Compile SDK 35, Min SDK 24
* **Gemini API Key:** Required for AI tutor and dynamic quiz generation features

### Installation & Setup

1. **Clone the Repository:**
   ```bash
   git clone https://github.com/your-username/soma-smart.git
   cd soma-smart
   ```

2. **Configure API Keys:**
   Create a `.env` file in the project root (or set the API key in your AI Studio Secrets panel):
   ```env
   GEMINI_API_KEY=your_actual_gemini_api_key_here
   ```

3. **Build the Project:**
   In Android Studio, select **Sync Project with Gradle Files**, then run the application on an emulator or physical Android device (API 24+).

4. **Run Unit & Robolectric Tests:**
   ```bash
   gradle :app:testDebugUnitTest
   ```

---

## 📱 Screenshots & Overview

| **Home Dashboard** | **AI Quiz Generator** | **PDF Export** |
| :---: | :---: | :---: |
| CBC Subject breakdown, streak counter, and weekly study goal progress | Dynamic question creation, real-time timer, and instant explanations | Native PDF generation for exam sheets and parent report cards |

---

## 📄 License

This project is licensed under the MIT License - see the `LICENSE` file for details.
