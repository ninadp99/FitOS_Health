# FitOS UI Screens

## 📱 App Navigation Overview

```
┌─────────────────────────────────────┐
│         FitOS App Flow              │
├─────────────────────────────────────┤
│  1. Onboarding  →  Profile Setup    │
│                 ↓                   │
│  2. Dashboard   →  Daily Overview   │
│  3. Nutrition   →  Food Logging     │
│  4. Workout     →  Exercise Plans   │
│  5. Progress    →  Streaks & Stats  │
│  6. Settings    →  Profile Edit     │
└─────────────────────────────────────┘
```

---

## 🎨 Screen Layouts

### 1. Onboarding Screen
```
┌────────────────────────────┐
│    Welcome to FitOS! 👋    │
├────────────────────────────┤
│                            │
│   [Logo & Intro Text]      │
│                            │
│                            │
│   ┌──────────────────────┐ │
│   │ Get Started          │ │
│   └──────────────────────┘ │
│                            │
└────────────────────────────┘
```

**Collects:**
- Name
- Age / Date of Birth
- Fitness Goal (Weight Loss / Gain / Maintenance / Build Strength)
- Current Weight
- Workout Preferences

---

### 2. Dashboard Screen
```
┌────────────────────────────┐
│   Dashboard          ☀️    │
├────────────────────────────┤
│                            │
│  📅 Today, August 18       │
│                            │
│  ┌──────────────────────┐  │
│  │ 💧 Water Intake      │  │
│  │   6/8 cups           │  │
│  └──────────────────────┘  │
│                            │
│  ┌──────────────────────┐  │
│  │ 🍽️  Today's Meals    │  │
│  │ • Breakfast: 450 cal │  │
│  │ • Lunch: 680 cal     │  │
│  │ • Snack: 120 cal     │  │
│  │ Total: 1,250 cal     │  │
│  └──────────────────────┘  │
│                            │
│  ┌──────────────────────┐  │
│  │ 😴 Sleep            │  │
│  │   7.5 hours          │  │
│  └──────────────────────┘  │
│                            │
│  ┌──────────────────────┐  │
│  │ 💪 Today's Workout  │  │
│  │   None logged yet    │  │
│  └──────────────────────┘  │
│                            │
└────────────────────────────┘

Bottom Navigation:
[Dashboard] [Nutrition] [Workout] [Progress] [Settings]
```

**Features:**
- Real-time daily overview
- Quick access to all health metrics
- Add meal, water, sleep buttons
- Workout status indicator

---

### 3. Nutrition Screen
```
┌────────────────────────────┐
│   Nutrition          🍽️    │
├────────────────────────────┤
│                            │
│  ┌──────────────────────┐  │
│  │   📷 Add Meal        │  │
│  │   Take Photo         │  │
│  └──────────────────────┘  │
│                            │
│  Today's Meals (8/18):     │
│  ┌──────────────────────┐  │
│  │ Breakfast   450 cal  │  │
│  │ 7:30 AM     🖼️       │  │
│  │                      │  │
│  │ Protein: 20g         │  │
│  │ Carbs: 60g           │  │
│  │ Fat: 15g             │  │
│  └──────────────────────┘  │
│                            │
│  ┌──────────────────────┐  │
│  │ Lunch       680 cal  │  │
│  │ 12:45 PM    🖼️       │  │
│  │                      │  │
│  │ Protein: 35g         │  │
│  │ Carbs: 85g           │  │
│  │ Fat: 25g             │  │
│  └──────────────────────┘  │
│                            │
│  Daily Total:              │
│  💪 Protein: 55g / 120g    │
│  🌾 Carbs: 145g / 250g     │
│  🥑 Fat: 40g / 80g         │
│                            │
└────────────────────────────┘
```

**Features:**
- Photo-based meal logging
- AI nutritional analysis
- Macro tracking
- Daily summaries
- Historical meal view

---

### 4. Workout Screen
```
┌────────────────────────────┐
│   Workout            💪    │
├────────────────────────────┤
│                            │
│  📅 Set Workout Days       │
│  ┌──────────────────────┐  │
│  │ ☑️ Monday            │  │
│  │ ☑️ Tuesday           │  │
│  │ ☐ Wednesday          │  │
│  │ ☑️ Thursday          │  │
│  │ ☑️ Friday            │  │
│  │ ☐ Saturday           │  │
│  │ ☐ Sunday             │  │
│  └──────────────────────┘  │
│                            │
│  📋 Today's Workout        │
│  ┌──────────────────────┐  │
│  │ 60 min Full Body     │  │
│  │ Beginner Level       │  │
│  └──────────────────────┘  │
│                            │
│  🔥 Warmup (5 min)         │
│  ☐ Arm Circles   [Video]   │
│  ☑️ Jumping Jacks [Video]  │
│  ☐ Leg Swings    [Video]   │
│                            │
│  💪 Main Workout (45 min)  │
│  ☑️ Push-ups      [Video]  │
│  ☑️ Squats        [Video]  │
│  ☐ Lunges        [Video]   │
│  ☐ Planks        [Video]   │
│  ☑️ Burpees      [Video]   │
│                            │
│  😌 Cool Down (10 min)     │
│  ☐ Stretching    [Video]   │
│  ☐ Deep Breathing [Video]  │
│                            │
│  ┌──────────────────────┐  │
│  │  ✅ Save Workout    │  │
│  └──────────────────────┘  │
│                            │
└────────────────────────────┘
```

**Features:**
- AI-generated personalized plans
- Warmup → Main → Cooldown structure
- Exercise checkboxes
- YouTube video links
- Automatic logging
- Rest day screens

---

### 5. Progress Screen
```
┌────────────────────────────┐
│   Progress           📈    │
├────────────────────────────┤
│                            │
│  🔥 Workout Streak         │
│  ┌──────────────────────┐  │
│  │        🔥 12 Days    │  │
│  │                      │  │
│  │    Keep it going!    │  │
│  └──────────────────────┘  │
│                            │
│  📊 Total Workouts: 47     │
│                            │
│  ⚖️  Weight Trend           │
│  ┌──────────────────────┐  │
│  │  85 ────────┐        │  │
│  │  83 ────┐   │        │  │
│  │  81 ┐   │   │        │  │
│  │  79 │   │   │        │  │
│  │     Aug Sep Oct       │  │
│  └──────────────────────┘  │
│                            │
│  📈 Recent Workouts        │
│  • Aug 18: 60 min          │
│  • Aug 16: 45 min          │
│  • Aug 15: 60 min          │
│  • Aug 13: 90 min          │
│  • Aug 12: 60 min          │
│                            │
│  💪 Best Performance       │
│  • Longest: 120 min        │
│  • Most Frequent: Aug      │
│                            │
└────────────────────────────┘
```

**Features:**
- Workout streaks
- Weight trends
- Historical data
- Performance stats
- Visual graphs

---

### 6. Settings Screen
```
┌────────────────────────────┐
│   Settings           ⚙️    │
├────────────────────────────┤
│                            │
│  👤 Profile                │
│  ┌──────────────────────┐  │
│  │ Name: Nina           │  │
│  │ Age: 28              │  │
│  │ Goal: Build Strength │  │
│  │ Weight: 68 kg        │  │
│  │                      │  │
│  │ [Edit Profile]       │  │
│  └──────────────────────┘  │
│                            │
│  🤖 AI Settings            │
│  ┌──────────────────────┐  │
│  │ AI Model:            │  │
│  │ • Nutrition: Vision  │  │
│  │ • Workout: Text Gen  │  │
│  │                      │  │
│  │ [Update Preferences] │  │
│  └──────────────────────┘  │
│                            │
│  📱 App Settings           │
│  ┌──────────────────────┐  │
│  │ Theme: Light/Dark    │  │
│  │ Notifications: On    │  │
│  │ Daily Brief: 7 AM    │  │
│  │                      │  │
│  │ [Preferences]        │  │
│  └──────────────────────┘  │
│                            │
│  ℹ️  About                  │
│  • Version: 1.0.0          │
│  • Privacy Policy          │
│  • About FitOS             │
│                            │
│  ┌──────────────────────┐  │
│  │ [Reset All Data]     │  │
│  └──────────────────────┘  │
│                            │
└────────────────────────────┘
```

**Features:**
- Profile editing
- AI preferences
- App settings
- About & help
- Data management

---

## 🎯 User Journey

```
START → Onboarding → Dashboard → Choose Activity
                          ↓
                    ┌─────┼─────┐
                    ↓     ↓     ↓
                 Nutrition Workout Progress
                    ↓     ↓     ↓
                  AI Analysis / Logging
                    ↓     ↓     ↓
                 Update Store → Refresh Dashboard
```

---

## 🌈 Color Scheme

| Element | Color | Usage |
|---------|-------|-------|
| Primary | `#007AFF` | Buttons, highlights |
| Success | `#34C759` | Complete, streaks |
| Warning | `#FF9500` | Warnings, inactive |
| Error | `#FF3B30` | Errors, critical |
| Background | Light/Dark | Theme-based |
| Text | Primary/Secondary | Content |

---

## 📐 Design Principles

✅ **Minimalist & Clean** - Focus on essentials
✅ **Accessible** - Large touch targets, readable text
✅ **Fast & Responsive** - Instant feedback
✅ **Offline-First** - Works without internet
✅ **Mobile-Optimized** - Built for thumbs
✅ **Dark Mode Support** - Eye-friendly

---

## 🔄 Data Flow

```
User Input (Photo/Manual) 
        ↓
    AI Analysis (Groq)
        ↓
    Validate & Format
        ↓
    Zustand Store
        ↓
    AsyncStorage (Persist)
        ↓
    UI Update (Instant)
```

---

## 📲 Responsive Breakpoints

- **Mobile**: 375px - 768px (Primary)
- **Tablet**: 768px - 1024px (Secondary)
- **Web**: 1024px+ (Limited support)

---

## ✨ Interactive Elements

- **Buttons**: Tap feedback with ripple effect
- **Toggle Switches**: Smooth animations
- **Progress Bars**: Real-time updates
- **Charts**: Interactive graphs
- **Modals**: Slide-up actions
- **Bottom Sheet**: Additional options

---

## 🎬 Animations

- **Screen Transitions**: Slide left/right
- **Modal Pop**: Scale + fade
- **Button Press**: Scale down + ripple
- **Loading**: Spinner animation
- **Success**: Checkmark animation
- **Streak Update**: Confetti effect

---

## 📊 Key Metrics Displayed

### Dashboard
- Water intake (cups/day)
- Calories (total + meals)
- Sleep hours
- Workout status

### Nutrition
- Protein, Carbs, Fat (grams + %)
- Calories (current/goal)
- Meal count
- Macro ratios

### Workout
- Duration (minutes)
- Exercise count
- Completion %
- Calories burned (estimated)

### Progress
- Streak count (days)
- Total workouts
- Weight trend
- Goal progress

---

## 🚀 Performance Targets

- **Load Time**: < 2 seconds
- **AI Response**: < 5 seconds
- **UI Responsiveness**: 60 FPS
- **Storage**: < 50 MB

---

## 📝 Form Validation

✅ Non-empty fields required
✅ Valid date/time formats
✅ Weight range: 30-200 kg
✅ Age range: 13-120 years
✅ Realistic calorie estimates

---

## 🎨 Component Library

- Custom TextInput with validation
- Reusable Card components
- Theme-aware buttons
- Responsive layouts
- Loading indicators
- Toast notifications

---
