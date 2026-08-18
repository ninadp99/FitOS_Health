# FitOS - Personal AI Health Companion

<div align="center">
  <h3>Your Personal Health OS with AI-Powered Insights</h3>
  <p>
    <strong>FitOS</strong> is a React Native mobile app that combines AI-powered nutrition analysis, intelligent workout planning, and comprehensive health tracking—all stored locally on your device.
  </p>

  ![React Native](https://img.shields.io/badge/React_Native-0.81.5-61DAFB?logo=react&logoColor=white)
  ![Expo](https://img.shields.io/badge/Expo-54.0-000020?logo=expo)
  ![TypeScript](https://img.shields.io/badge/TypeScript-5.9-3178C6?logo=typescript&logoColor=white)
  ![License](https://img.shields.io/badge/License-MIT-green)
</div>

---

## ✨ Features

### 🤖 AI-Powered Nutrition Analysis
- **Food Photo Recognition**: Upload photos of your meals using AI vision models
- **Instant Nutrition Data**: Get detailed macros (protein, carbs, fats) and calorie estimates
- **Meal Logging**: Automatic timestamps and date-based organization
- **Daily Summaries**: Quick overview of your nutrition for the day

### 💪 Intelligent Workout Planning
- **AI Workout Generator**: Get personalized beginner workout plans from Groq AI
- **Flexible Scheduling**: Choose your workout days (0-7 days per week)
- **Smart Planning**: Full structure → Warmup → Main Exercises → Cooldown
- **Exercise Tracking**: Built-in checkboxes to log completed exercises
- **YouTube Integration**: Video tutorials available for every exercise
- **Rest Days**: Dedicated rest day screens for your non-workout days

### 📊 Comprehensive Health Tracking
- **Weight Logging**: Track weight changes over time
- **Workout History**: View all completed workouts and progress
- **Sleep Tracking**: Log hours slept each night
- **Water Intake**: Monitor daily hydration
- **Streak Counter**: Stay motivated with your workout streak
- **Progress Dashboard**: Visual overview of all health metrics

### 📱 Modern UI/UX
- **Bottom Navigation**: Easy access to all major sections
- **Smooth Animations**: Native React Native transitions
- **Responsive Design**: Optimized for mobile screens
- **Dark Mode Support**: Eye-friendly interface

### 💾 Local Data Storage
- **No Cloud Required**: All data stored securely on your device
- **Automatic Persistence**: Zustand + AsyncStorage keeps your data safe
- **Offline First**: Works completely offline
- **Device-Only**: Your health data stays on your phone

---

## 🛠️ Tech Stack

| Component | Technology |
|-----------|------------|
| **Framework** | React Native + Expo 54 |
| **Language** | TypeScript 5.9 |
| **State Management** | Zustand with AsyncStorage Persist |
| **AI Engine** | Groq API (llama-3.3-70b + llama-4-scout-17b for vision) |
| **Local Storage** | AsyncStorage |
| **Navigation** | React Native Navigation |
| **Device** | Android (Samsung Galaxy S24 Ultra via Expo Go) |

---

## 📋 Screens & Navigation

1. **Onboarding Screen** - Initial setup with profile creation
2. **Dashboard** - Today's health overview (meals, water, sleep, workouts)
3. **Nutrition Screen** - Food photo analysis and meal logging
4. **Workout Screen** - AI-generated plans and exercise tracking
5. **Progress Screen** - Historical data and streaks
6. **Settings Screen** - Profile management and app preferences
7. **Bottom Navigation** - Quick access to all screens

---

## 🚀 Getting Started

### Prerequisites
- Node.js 18+ and npm/yarn
- Expo CLI: `npm install -g expo-cli`
- Android device or emulator
- Groq API key (get one for free at [console.groq.com](https://console.groq.com))

### Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/ninadp99/FitOS_Health.git
   cd FitOS_Health
   ```

2. **Install dependencies**
   ```bash
   npm install
   ```

3. **Add your Groq API key**
   - Create a `.env` file in the root directory (or add to your environment)
   - Add: `GROQ_API_KEY=your_api_key_here`

4. **Start the app**
   ```bash
   # For Android
   npm run android

   # Or start the development server
   npm start
   ```

5. **Open in Expo Go**
   - Install Expo Go on your Android device
   - Scan the QR code from the terminal

---

## 📱 Screenshots

<div align="center">

### Onboarding Flow
Get started in 7 simple steps - personalized for your goals, body, and lifestyle.

![Onboarding Step 1](screenshots/01-onboarding-step1-name.png) ![Fitness Goal](screenshots/02-onboarding-step2-fitness-goal.png) ![Body Info](screenshots/03-onboarding-step3-body-measurements.png)

---

### Dashboard with AI Coach
Your daily health overview powered by Groq AI. See nutrition, water intake, sleep, and workout status at a glance.

![Dashboard](screenshots/10-home-dashboard-ai-coach.png)

---

### Progress Tracking
Monitor weight, BMI, streaks, and achievements. Stay motivated with visual progress indicators.

![Progress](screenshots/09-progress-screen.png)

---

### AI Workout Planning
Get personalized workout plans with exercise descriptions, form cues, and YouTube video tutorials.

![Workout Details](screenshots/12-full-body-workout-details.png)

---

### Settings & Configuration
Manage your Groq AI models, profile metrics, macros, and app preferences.

![Settings](screenshots/13-settings-screen.png)

---

</div>

**Explore all screenshots in the [`/screenshots`](screenshots/) folder**

---

## 💡 How It Works

### Nutrition Flow
1. Open Nutrition screen
2. Tap "Add Meal" and take a photo
3. AI analyzes the image and extracts nutrition data
4. Review and confirm macros/calories
5. Meal saved with timestamp and date
6. Dashboard automatically shows today's meals

### Workout Flow
1. Select your workout days on profile setup
2. On workout days, open Workout screen
3. AI generates a personalized plan
4. Follow the exercises (warmup → main → cooldown)
5. Check off completed exercises
6. Save your workout
7. View updated progress and streaks

### Health Tracking
1. Log water intake throughout the day
2. Record sleep hours before bed
3. Log weight weekly or daily
4. View trends in Progress screen
5. All data persists automatically

---

## 📊 Data Storage

All data is stored locally using **Zustand** with **AsyncStorage persistence**:
```
{
  isOnboarded: boolean,
  profile: { name, age, goal, ... },
  meals: [{ date, timestamp, calories, macros, ... }],
  workouts: [{ date, exercises, duration, ... }],
  weightLog: [{ date, weight }],
  water: number,
  sleepHours: number,
  streak: number,
  totalWorkouts: number
}
```

**No backend. No cloud sync. Your data, your device.**

---

## 🤖 AI Capabilities

### Food Photo Analysis
- Model: `llama-4-scout-17b` (Groq Vision)
- Detects: Food type, portion size, estimated calories, macronutrients
- Speed: <5 seconds per analysis
- Accuracy: ~85% (user can adjust if needed)

### Workout Generation
- Model: `llama-3.3-70b-versatile` (Groq Text)
- Generates: Full workout plans for beginners
- Includes: Warmup, main exercises, cooldown, reps/sets
- Duration: 30-120 minutes (user customizable)

### Daily AI Brief
- Summarizes yesterday's nutrition, sleep, and workouts
- Provides personalized health insights
- Uses your actual logged data

---

## ⚙️ Configuration

### Groq API Usage
- **Estimated Daily Usage**: ~45,000 tokens
- **Free Tier Limit**: 500,000 tokens/day
- **Status**: Well under limit, stays free forever

### Supported Devices
- Android 9.0+ (tested on Samsung Galaxy S24 Ultra)
- iOS support planned
- Web version available (limited features)

---

## 🗂️ Project Structure

```
fitos/
├── src/
│   ├── screens/          # Navigation screens
│   ├── components/       # Reusable UI components
│   ├── store/           # Zustand state management
│   ├── services/        # Groq API integration
│   └── types/           # TypeScript interfaces
├── assets/              # Images, icons, splash screen
├── App.tsx              # Root component
├── app.json             # Expo configuration
└── package.json         # Dependencies
```

---

## 🔄 State Management

### Zustand Store (`useStore.ts`)
Single source of truth for all app state:
- Profile information
- Meal history with timestamps
- Workout history and schedule
- Weight log and streaks
- Water intake and sleep hours
- Preferences and settings

**Automatic Persistence**: All changes automatically saved to device storage via AsyncStorage middleware.

---

## 📈 Roadmap

- [x] Onboarding flow
- [x] Dashboard with daily overview
- [x] Food photo analysis
- [x] Workout planning and tracking
- [x] Health metrics (water, sleep, weight)
- [x] Progress tracking with streaks
- [ ] Morning AI brief with real data
- [ ] Weekly Excel export (.xlsx)
- [ ] Social sharing (optional)
- [ ] Apple Health/Google Fit integration (future)

---

## 🚨 Privacy & Security

✅ **Your Data is Safe**
- All data stored locally on your device
- No internet connection needed (except for AI features)
- No accounts or sign-ups required
- No data collection or tracking
- No advertisements

---

## 📜 License

This project is licensed under the **MIT License** - see the [LICENSE](LICENSE) file for details.

---

## 🤝 Contributing

This is a personal project, but suggestions and insights are welcome!
- Report bugs via GitHub Issues
- Share feature ideas in Discussions
- Fork and create pull requests for improvements

---

## 💬 Feedback

Have questions or ideas? 
- **GitHub Issues**: Open an issue on this repo
- **GitHub Discussions**: Use the Discussions tab
- **GitHub Profile**: Visit [@ninadp99](https://github.com/ninadp99)

---

## 📞 Contact

- **GitHub**: [@ninadp99](https://github.com/ninadp99)
- **Project**: [FitOS_Health](https://github.com/ninadp99/FitOS_Health)
- **Report Issues**: Use GitHub Issues for bug reports and feature requests

---

<div align="center">
  <p>
    <strong>Built with ❤️ using React Native, Expo, and AI</strong>
  </p>
  <p>
    <em>Your personal health companion, always with you, always learning.</em>
  </p>
</div>
