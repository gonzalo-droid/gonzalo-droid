# README Redesign — gonzalo-droid

## Overview

Redesign of the GitHub profile README for `gonzalo-droid`. The goal is a professional, English-language profile that presents Gonzalo as a Mobile Developer (Android & iOS), showcases his apps with screenshots, organizes his tech stack by platform, and includes GitHub analytics.

---

## Layout: CV Structure (Structure B)

Sections stacked vertically, each with a clear uppercase label. No horizontal split between content and sidebar.

---

## Sections

### 1. Header (centered)
- Greeting: `Hi 👋, I'm Gonzalo`
- Subtitle: `Mobile Developer · Android & iOS · Passionate about AI in mobile solutions`
- Social links as icon+text badges (pill style):
  - 📺 YouTube → `https://youtube.com/GonzaloDroid2050?sub_confirmation=1`
  - 📸 Instagram → `https://www.instagram.com/gonzalo.lozg/`
  - 🎵 TikTok → `https://www.tiktok.com/@gonzalodroid`
  - 🌐 Portfolio → `https://gonzalo-lozg.me/`
- Shields.io badges:
  - GitHub followers: `https://img.shields.io/github/followers/gonzalo-droid?style=social`
  - YouTube subscribers: `https://img.shields.io/youtube/channel/subscribers/UCPjql8JlN5kw6hU2U_tngaw?style=social`

### 2. About Me
Bullet list in English:
- 📲 Android & iOS developer with Kotlin and Swift
- 🌱 Passionate about sharing my journey with the community, constantly learning
- ☁️ AI is transforming the world — I love exploring its potential in mobile solutions
- 🚀 Continuous learner, always exploring new tech applications
- 🎥 I build apps and face challenges, sharing everything with the community
- Adding portfolio link: `gonzalo-lozg.me`

### 3. Tech Stack
Grouped by platform using HTML `<table>` or `<div>` grid. Four categories:

| Category | Technologies |
|---|---|
| 📱 Android | Kotlin, Jetpack Compose, Hilt, Room, Retrofit |
| 🍎 iOS | Swift, SwiftUI |
| 🌐 Multiplatform | KMP, Flutter |
| 🔧 Tools & Services | Firebase, Slack, Notion |

Each category rendered as a card with colored label and chip-style badges using `shields.io` logo badges or plain text chips via HTML.

### 4. My Apps
Two app cards, each with **vertical layout**: info on top, full-width screenshot image below.

**Card structure:**
```
[App Name]
[Short description — 1-2 lines]
[Tech stack chips]
[Store / Web links as badges]
────────────────────────────
[Screenshot image — full width]
```

#### App 1: Quote Anime | Frases Anime
- **Description:** Discover and share inspiring quotes from your favorite anime. Browse by category, save your favorites, and receive daily quotes via notifications or your home screen widget.
- **Stack:** Kotlin, Jetpack Compose, Hilt, Room, Glance API, SwiftUI, SwiftData, WidgetKit, Firebase, AdMob, MVVM + Clean Architecture
- **Links:**
  - Play Store: `https://play.google.com/store/apps/details?id=com.gondroid.quoteanime`
  - App Store: `https://apps.apple.com/pe/app/quoteanime-frases-de-anime/id6762100338?l=en-GB`
  - Web: `https://quote-anime-web.vercel.app/`
- **Image:** `assets/app_quote_anime.png`

#### App 2: AutoTest Licencia
- **Description:** Practice for your driving license exam. Review an updated and categorized question bank, take simulation tests, and track your results.
- **Stack:** Kotlin, Jetpack Compose, Hilt, Firebase, MVVM
- **Links:**
  - Play Store: `https://play.google.com/store/apps/details?id=com.gondroid.mtcquiz`
- **Image:** `assets/app_autotest.jpg`

### 5. GitHub Analytics
Three stat cards centered, using existing Vercel-hosted stats service + streak:

```
[GitHub Stats]  [Top Languages]  [GitHub Streak]
```

- Stats: `https://github-readme-stats-eight-theta.vercel.app/api?username=gonzalo-droid&show_icons=true&theme=algolia&include_all_commits=true&count_private=true`
- Top Languages: `https://github-readme-stats-eight-theta.vercel.app/api/top-langs/?username=gonzalo-droid&layout=compact&langs_count=8&theme=algolia`
- Streak: `https://github-readme-streak-stats.herokuapp.com/?user=gonzalo-droid&theme=algolia`

All three wrapped in `<p align="center">` with `height="180em"`.

---

## Implementation Notes

- All content in **English**
- Use `<div align="center">` for centered sections
- App cards use HTML `<table>` for layout compatibility across GitHub's markdown renderer (no CSS grid/flexbox support)
- Images referenced as relative paths: `assets/app_quote_anime.png`, `assets/app_autotest.jpg`
- Tech stack badges: use `shields.io` with `style=flat-square` and appropriate logo colors, OR plain HTML chips — keep consistent
- `.superpowers/` should be added to `.gitignore`
