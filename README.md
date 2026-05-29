# 🩺 Diabetes Risk Analyzer

> A smart Android application that estimates diabetes risk instantly using a **Fuzzy Logic Inspired Algorithm** — empowering users with health awareness through clinical data analysis and symptom assessment.

---

## 📖 About the App

**Diabetes Risk Analyzer** is an Android mobile application developed to help individuals assess their potential risk of diabetes based on clinical health indicators and common symptoms. The app uses a **Fuzzy Logic Inspired Algorithm** to analyze user-provided data including fasting glucose level, BMI, age, and five key diabetes-related symptoms. Based on the analysis, the app classifies the user's risk as **Low**, **Medium**, or **High** and provides personalized health recommendations.

This app is designed for general users who want to monitor their health, students studying medical informatics, and anyone seeking early awareness about diabetes risk factors. It solves the problem of lack of awareness by providing an instant, easy-to-understand risk estimation without needing a hospital visit. The app features a complete result history, visual charts, push notifications, and a clean dark-themed user interface — making it both functional and professional.

> ⚠️ **Disclaimer:** This application is for educational and awareness purposes only. It does NOT provide medical diagnosis. Always consult a qualified healthcare professional.

---

## 📸 App Screenshots

| Splash Screen | Input Form | Input Form (Symptoms) |
|:---:|:---:|:---:|
| ![Splash](screenshots/splash_screen.png) | ![Input](screenshots/input_screen.png) | ![Symptoms](screenshots/symptoms_screen.png) |

| Result - Summary | Result - Charts | History |
|:---:|:---:|:---:|
| ![Summary](screenshots/result_summary.png) | ![Charts](screenshots/result_charts.png) | ![History](screenshots/history_screen.png) |

---

## ✨ Features

- 🔍 **Fuzzy Logic Risk Analysis** — Calculates risk based on 5 symptoms + clinical inputs
- 🩸 **Clinical Input Support** — Accepts Age, Fasting Glucose Level, and BMI
- 📋 **5-Symptom Questionnaire** — Water intake, urination, weight loss, wound healing, hunger
- 📊 **Visual Charts** — Animated Bar Chart and Radar Chart showing score breakdown
- 🟢🟡🔴 **Three Risk Levels** — Low / Medium / High with personalized messages
- 🔔 **Push Notifications** — Instant risk alert after every analysis
- 📂 **Result History** — All past results saved with Room Database
- ✅ **Input Validation** — All fields validated with proper error messages
- 📤 **Share Results** — Share your result via any app
- 🎨 **Dark Theme UI** — Modern Material Design 3 interface
- 🔄 **Smooth Animations** — Slide and fade transitions between screens

---

## 🖥️ Technologies Used

| Technology | Purpose |
|-----------|---------|
| **Java** | Primary programming language |
| **Android Studio** | Development IDE |
| **XML** | UI layout design |
| **Material Design 3** | UI components and styling |
| **Room Database** | Local storage for result history |
| **MPAndroidChart v3.1.0** | Bar chart and Radar chart visualization |
| **Fragments** | Tabbed result screen (Summary + Chart) |
| **NotificationCompat** | Push notifications |
| **Gradle 8.9** | Build system |
| **Android SDK 34** | Target platform (Android 14) |

---

## 🧠 Algorithm — How It Works

The app uses a **Fuzzy Logic Inspired Scoring Algorithm**:

### Step 1 — Symptom Scoring
Each of the 5 questions is scored from **1 to 4**:

| Score | Meaning |
|-------|---------|
| 1 | Normal |
| 2 | Slightly Abnormal |
| 3 | Abnormal |
| 4 | Highly Abnormal |

### Step 2 — Clinical Bonus Scoring

| Condition | Bonus Points |
|-----------|-------------|
| Age 45–59 | +1 |
| Age 60+ | +2 |
| Glucose 100–125 mg/dL | +1 |
| Glucose 126–199 mg/dL | +2 |
| Glucose 200+ mg/dL | +3 |
| BMI 25–29.9 | +1 |
| BMI 30+ | +2 |

### Step 3 — Risk Determination

| Total Score | Risk Level | Action |
|------------|-----------|--------|
| ≤ 7 | 🟢 **LOW** | Maintain healthy lifestyle |
| 8 – 14 | 🟡 **MEDIUM** | Improve diet, monitor health |
| ≥ 15 | 🔴 **HIGH** | Consult a doctor immediately |

---

## 📱 Android Concepts Implemented

- ✅ **Activities** — Splash, Main (Input), Result, History
- ✅ **Fragments** — Result Summary Fragment, Result Chart Fragment
- ✅ **Action Bar / Toolbar** — With custom menus on all screens
- ✅ **Intents** — For navigation and passing data between screens
- ✅ **Push Notifications** — NotificationChannel + NotificationCompat
- ✅ **RecyclerView** — Custom adapter for history list
- ✅ **Room Database** — Entity, DAO, Database for persistent storage
- ✅ **Input Validation** — TextInputLayout with error messages
- ✅ **Animations** — Slide-in, slide-out, fade transitions
- ✅ **Vector Drawables** — Custom icons and backgrounds

---

## 📥 APK Download

Download and install the app directly on your Android phone:

**[⬇️ Download DiabetesRiskAnalyzer.apk](apk/DiabetesRiskAnalyzer.apk)**

> File size: ~6 MB | Minimum Android version: 7.0 (Nougat)

---

## 📲 How to Install the APK

1. Click the APK download link above
2. Open the downloaded file on your Android phone
3. If prompted, go to **Settings → Security → Enable "Install from Unknown Sources"**
4. Tap **Install**
5. Open **Diabetes Risk Analyzer** and start your health assessment

---

## 💻 How to Run the Project in Android Studio

1. **Clone or download** this repository:
```bash
git clone https://github.com/mahr168/Android_project.git
```
2. Open **Android Studio**
3. Click **File → Open** and select the `app/` folder
4. Wait for **Gradle sync** to complete
5. Set your SDK path in `local.properties`:
```
sdk.dir=C:\Users\YOUR_NAME\AppData\Local\Android\Sdk
```
6. Connect an Android device or start an **emulator** (API 24+)
7. Click **▶ Run**

### Requirements
- Android Studio Hedgehog (2023.1.1) or newer
- JDK 17+
- Android SDK API 24 – 34
- Internet connection for Gradle dependency download

---

## 🎥 Demo Video

[▶️ Watch Demo Video](https://github.com/mahr168/Android_project)

*(Demo video coming soon)*

---

## 🔒 Privacy Policy

This app collects no personal data and does not transmit any information to external servers. All data entered by the user (name, age, glucose level, symptoms) is stored **locally on the device only** using Room Database and is never shared with any third party.

[📄 View Full Privacy Policy](docs/privacy_policy.pdf)

---

## 📚 User Manual

A complete user guide explaining how to use the app step by step is available here:

[📖 View User Manual](docs/user_manual.pdf)

---

## 🚀 Future Enhancements

- 🔥 Firebase integration for cloud-based result sync
- 👨‍⚕️ Nearby doctor/clinic locator feature
- 📊 Weekly and monthly health trend graphs
- 🌙 Light / Dark theme toggle
- 🌍 Multi-language support (Urdu, Arabic, etc.)
- 📧 Email result report to doctor
- 🤖 AI-based improved prediction model
- 👤 User account and profile management

---

## 📁 Project Structure

```
Android_project/
│
├── app/                          ← Complete Android source code
│   └── src/main/
│       ├── java/com/health/diabetesrisk/
│       │   ├── activities/       ← SplashActivity, MainActivity, ResultActivity, HistoryActivity
│       │   ├── fragments/        ← ResultSummaryFragment, ResultChartFragment
│       │   ├── models/           ← RiskResult.java
│       │   ├── adapters/         ← HistoryAdapter.java
│       │   └── utils/            ← DiabetesAlgorithm, AppDatabase, NotificationHelper
│       └── res/
│           ├── layout/           ← All XML screen layouts
│           ├── values/           ← Colors, strings, themes
│           ├── drawable/         ← Icons and backgrounds
│           └── menu/             ← Action bar menus
│
├── screenshots/                  ← App screen screenshots
├── apk/                          ← Installable APK file
├── docs/                         ← Privacy policy and user manual
├── README.md                     ← This file
├── LICENSE                       ← MIT License
├── .gitignore                    ← Git ignore rules
├── build.gradle                  ← Root build config
└── settings.gradle               ← Project settings
```

---

## 👩‍💻 Developed By

| | |
|--|--|
| **Student Name** | Ishfa |
| **Project** | Final Project — Mobile Application Development |
| **Department** | Computer Science / Information Technology |
| **GitHub** | [github.com/mahr168](https://github.com/mahr168) |

---

## 📄 License

This project is licensed under the **MIT License** — see the [LICENSE](LICENSE) file for details.

---

<p align="center">
  Made with ❤️ for educational purposes | Not a medical diagnosis tool
</p>
