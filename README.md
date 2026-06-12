# MatchAI 🚀

[![Live Demo](https://img.shields.io/badge/Live%20Demo-Vercel-blueviolet?style=for-the-badge&logo=vercel)](https://match-ai-frontend.vercel.app/)

MatchAI is a premium, high-performance automated job application client. Designed with modern aesthetics, smooth parallax interactions, and responsive layouts, MatchAI guides job seekers through a seamless flow—from resume parsing and profile verification to strategy generation and one-click automated job applications.

---

## ✨ Features

### 1. 🌌 Immersive Landing Experience
- **Premium Particle Backdrop:** Powered by `tsparticles` for a dynamic and interactive background.
- **Glassmorphic Hero Section:** Captivating visual callouts with smooth hover transitions.
- **Bento Grid Feature Showcase:** A modern grid highlighting key features like Semantic Matching, Automated Applications, and Privacy Control.
- **Scroll-Triggered Feature Walkthrough:** Smooth parallax scroll effects driven by `lenis` and `framer-motion`.
- **Integrated Auth Modals:** Beautiful, smooth modal transitions for User Registration and Login.

### 2. 📋 Interactive Onboarding Pipeline
- **Resume Dropzone:** An elegant drag-and-drop interface (`react-dropzone`) that initiates the resume ingestion process.
- **Profile Verification Form:** A comprehensive form validated via `react-hook-form` and `zod` to verify extracted contact details, current role, core skills, and work history.
- **Preference Ranker:** A custom card deck allowing candidates to specify target roles and rank work preferences (e.g., Remote vs. Hybrid vs. Onsite).
- **Strategy Engine Transition:** A retro terminal-style overlay displaying step-by-step algorithms configuring rules and searching the web.

### 3. 💼 Recommended Matches & Auto-Apply
- **Target Match Dashboard:** Displays highly compatible roles categorized by companies, direct links to application platforms (Lever, Greenhouse, etc.), and custom match percentage indicators.
- **Bulk Application Selection:** Option to filter, select, and queue multiple roles at once.
- **Smart Apply Modal:** Simulates missing application requirements, displays executing automation logs, and celebrates successful portal submissions.

---

## 🛠️ Tech Stack

- **Frontend Core:** [React](https://react.dev/) + [TypeScript](https://www.typescriptlang.org/) + [Vite](https://vitejs.dev/)
- **Styling:** [TailwindCSS](https://tailwindcss.com/) (Version 3)
- **Animations:** [Framer Motion](https://www.framer.com/motion/)
- **Smooth Scrolling:** [Lenis](https://lenis.darkroom.engineering/)
- **Forms & Validation:** [React Hook Form](https://react-hook-form.com/) + [Zod](https://zod.dev/)
- **Icons & Particles:** [Lucide React](https://lucide.dev/) + [@tsparticles/react](https://particles.js.org/)

---

## 📁 Project Structure

```bash
src/
├── App.tsx                    # Main App Shell & State Router (Landing <-> Onboarding)
├── main.tsx                   # App Entrypoint
├── index.css                  # Tailwind imports, custom scrollbar & dark/light theme configs
└── components/
    ├── dashboard/             # Post-onboarding panels
    │   ├── JobDashboard.tsx   # Recommended jobs feed & selection
    │   └── SmartApplyModal.tsx# Executing console simulation
    ├── landing/               # Brand marketing & introduction components
    │   ├── AnimatedBackground.tsx
    │   ├── AuthModal.tsx
    │   ├── BentoGridFeatures.tsx
    │   ├── HeroSection.tsx
    │   ├── LandingPage.tsx
    │   ├── ParallaxCTA.tsx
    │   ├── ScrollFeatureShowcase.tsx
    │   └── SmoothScrollProvider.tsx
    └── onboarding/            # Form wizards & pipeline transitions
        ├── OnboardingPage.tsx
        ├── PreferenceRanking.tsx
        ├── ProfileVerificationForm.tsx
        ├── ResumeDropzone.tsx
        └── StrategyEngineTransition.tsx
```

---

## 🚀 Getting Started

### Prerequisites
- [Node.js](https://nodejs.org/) (v18+ recommended)
- [npm](https://www.npmjs.com/)

### Installation & Run

1. **Install Dependencies & Start dev server:**
   You can run the pre-configured `start.bat` script on Windows:
   ```bash
   .\start.bat
   ```
   *Or manually install and run:*
   ```bash
   npm install
   npm run dev
   ```

2. **Accessing the App:**
   Open [http://localhost:5173](http://localhost:5173) in your browser.

---

## ⚙️ Available Scripts

In the project directory, you can run:

- **`npm run dev`**: Runs the app in the development mode.
- **`npm run build`**: Builds the production bundle (build output target is configured in Vite).
- **`npm run preview`**: Locally previews the production build.
