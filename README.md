# Nutriz 🥗

> AI-powered fitness and nutrition app built for the Chilean market.

Nutriz helps Chilean gym-goers and fitness enthusiasts track their nutrition, get personalized meal and exercise recommendations, and use AI body analysis to understand their progress — all in Spanish and tailored to Chilean food culture.

---

## The problem

Most nutrition and fitness apps are built for the US or European market. Food databases don't include Chilean staples, calorie targets don't reflect local eating habits, and the UX is in English. Nutriz is built from the ground up for Chile.

---

## Key features

### AI body analysis
Take a photo and get personalized food and exercise recommendations based on your current body composition. Powered by vision AI — no wearables, no manual measurements.

### Nutrition tracking
- Chilean food database including local staples and supermarket products
- Macro and calorie tracking with daily and weekly views
- Meal logging with photo recognition

### Personalized plans
- Custom workout routines based on your goal (muscle gain, weight loss, maintenance)
- Weekly meal plans adapted to Chilean cuisine
- Progress tracking with AI-generated insights

### Built for Chile
- 100% in Spanish
- Chilean food culture and portion sizes
- Local supermarket product integration (planned)

---

## Tech stack

| Layer | Technology |
|---|---|
| Mobile app | Flutter (iOS & Android) |
| Backend API | FastAPI (Python) |
| Database & auth | Supabase (PostgreSQL) |
| File storage | Cloudflare R2 |
| AI features | Vision AI for body analysis · LLM for recommendations |
| Deployment | Railway |

---

## Architecture

```
Flutter App
     ↓
FastAPI Backend (Railway)
     ↓              ↓
Supabase        Cloudflare R2
(DB + Auth)     (Photo storage)
     ↓
Vision AI ← body photos
     ↓
Personalized recommendations
```

---

## Planned features

- [ ] AI body composition analysis from photo
- [ ] Personalized meal recommendations based on body analysis
- [ ] Exercise plan generator
- [ ] Chilean food database
- [ ] Macro & calorie tracker
- [ ] Progress photo timeline
- [ ] Weekly AI-generated insights report
- [ ] Barcode scanner for Chilean supermarket products
- [ ] Community challenges and streaks

---

## Getting started

> 🚧 Nutriz is currently in early development. Star the repo to follow progress.

### Backend

```bash
git clone https://github.com/james-own/nutriz
cd nutriz/backend
poetry install
poetry run uvicorn main:app --reload
```

### Mobile app

```bash
cd nutriz/mobile
flutter pub get
flutter run
```

---

## Environment variables

```env
SUPABASE_URL=your_supabase_url
SUPABASE_KEY=your_supabase_anon_key
CLOUDFLARE_R2_BUCKET=your_bucket
CLOUDFLARE_R2_ACCESS_KEY=your_key
CLOUDFLARE_R2_SECRET_KEY=your_secret
```

---

## Author

**Jameson Michel** — Senior Java Engineer · Flutter Developer  
[GitHub](https://github.com/james-own) · [LinkedIn](https://www.linkedin.com/in/jamesonm/)

---

> Built in Santiago, Chile 🇨🇱
