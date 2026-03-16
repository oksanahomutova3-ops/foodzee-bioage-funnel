# FoodZee Bio Age Quiz Funnel

Bio Age quiz funnel — 13 onboarding screens with localization (9 languages).

## How to use

1. Download `foodzee-bioage-final (1).zip`
2. Unzip it
3. Copy `src/AIPAGES/` folder into your project's `src/AIPAGES/`
4. Copy `src/locales/` JSON files into your project's `src/locales/` folders
5. Open `preview.html` in browser to see the visual preview

## Screens flow (13 screens)

| # | Screen | Type | Component |
|---|--------|------|-----------|
| 0 | Welcome | Landing (green bg, hero image) | BioWelcome |
| 1 | How old are you? | Scroll picker (18-80, default 30) | BioAge |
| 2 | Sleep hours | Single choice (4 options) | BioSleep |
| 3 | Activity level | Single choice (4 options) | BioActivity |
| 4 | Stress level | Single choice (3 options) | BioStress |
| 5 | Diet quality | Single choice (3 options) | BioDiet |
| 6 | Water intake | Single choice (3 options) | BioWater |
| 7 | Energy by evening | Single choice (3 options) | BioEnergy |
| 8 | Resting heart rate | Scroll picker (40-120 bpm) | BioHeartRate |
| 9 | Daily steps | Single choice (5 options) | BioDailySteps |
| 10 | Small Changes, Big Impact | Transition (green bg, image) | BioTransition |
| 11 | Analyzing | Auto-advance animation (4.2s) | BioAnalyzing |
| 12 | Paywall | Dashboard + comparison + features + reviews + plans | BioPaywall |

## File structure
## Developer notes

- All components follow the project convention: `/* eslint-disable */`, `function Page()`, `export default Page`
- All text via `t('namespace.key')` — no hardcoded strings
- Analytics: `Analytics.trackEvent()` on every user action
- Styles: SCSS modules only, no inline styles
- Back button: shown only when `currentIndex !== 0`
- Images: placeholders marked with CSS comments `/* Developer: set background-image */`
- Locales: EN, DE, ES, FR translated; CS, ID, IT, PT, TR contain EN text (need translation)
- Preview: open `preview.html` in any browser to see the full funnel
