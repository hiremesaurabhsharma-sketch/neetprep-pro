# NEETPrep Pro - Premium Medical Entrance MCQ Simulator & Test Series

A highly polished, responsive Single Page Application (SPA) designed to simulate the **National Testing Agency (NTA) NEET UG computer-based exam environment**. Mapped directly to the latest NCERT syllabus for **Class 11th & 12th**, it empowers medical aspirants with topic-targeted testing, custom combination mocks, and rich performance analytics.

---

## 🌟 Core Features

- **Class Selection Hub**: Dynamic dashboard to select standard Class 11th or Class 12th NCERT modules.
- **Unified Domain Selector**: Separate testing streams for:
  - **Physics** (Bright Cyan theme - focused on concepts and formulas)
  - **Chemistry** (Vibrant Amber theme - physical, organic reaction mechanisms)
  - **Botany** (Lush Emerald Green theme - plant structure, physiological systems)
  - **Zoology** (Majestic Amethyst theme - human systems, genetics, evolution)
  - **Full-Syllabus Mixed Mock Test**: Triggers a balanced mixed paper representing all domains proportionally.
- **Custom Syllabus Configurator**:
  - Interactive multi-select checklists of actual NEET chapters.
  - Weights displayed per chapter (High, Medium, Low yield).
  - Search filter to query chapters in real-time.
  - Select All / Clear toggles.
- **Flexible Test Parameters**:
  - **Question Density**: Launch tests with 10, 20, 30, 45, 90, or 180 questions (standard full-length).
  - **Timer Settings**: Choose Auto (standard NTA: 1 minute per question), Custom slider, or No Time Limit.
- **NTA Examination Simulator Portal**:
  - Live ticking timer with amber and red alert states.
  - Left presentation panel with highly legible, clear scientific typography.
  - Interactive A, B, C, D radio options matching the subject color accents.
  - Color-coded **NTA Question Navigator Palette** showing the state of every question (Unvisited, Visited, Answered, Marked for Review, Answered & Marked for Review).
  - Quick-navigation by directly clicking palette numbers.
- **Detailed Visual Analytics Dashboard**:
  - Overall scorecard with Marks Obtained, Percentage, and Accuracy Rate.
  - NEET Standard Scoring Model: **+4 for Correct, -1 for Incorrect, 0 for Unattempted**.
  - Dynamic **SVG Radial Progress Gauge** rendering the success ratio.
  - **Chapter-wise Diagnostics Insights**: Automatically groups and lists chapters into **Mastered (≥80%)**, **Needs Practice (50-80%)**, or **Critical Attention (<50%)** based on results.
  - **Question-by-Question Solution Keys**: Review correct vs chosen options and detailed, conceptual explanations for every question.
  - Filter solutions by state: All, Correct, Incorrect, Unattempted.

---

## 🛠️ Architecture & Tech Stack

- **Structure (Semantic HTML5)**: Native layout with smooth transition states inside a single base `index.html` structure.
- **Styling (CSS3 Custom Design System)**:
  - Responsive flexbox/grid layout optimized for both desktop simulator screens and mobile viewing.
  - Glassmorphic card styling (`backdrop-filter`) with custom glows and shadows.
  - Variable-driven CSS structure supporting clean HSL color systems.
- **Logic (Vanilla JS - ES6)**:
  - State machine storing candidate options, test progress, and analytics.
  - **Procedural Conceptual Question Generator**: An advanced generator that dynamically creates standard-compliant, high-yield NEET conceptual questions to support unlimited mock lengths (up to 180 questions on any customized chapter subset!).
- **Icons**: Lucide vector icons imported via CDN.
- **Fonts**: Outfit (headings) & Plus Jakarta Sans (body) via Google Fonts.

---

## 🚀 How to Run the Website

Since the project is structured as a pure client-side SPA with zero heavy third-party bundle dependencies, you can run it instantly using any simple web server.

### Method 1: Using npx (Recommended for developers)
Open your terminal in the workspace directory and execute:
```bash
npx http-server ./
```
Then, navigate to the local address displayed in your console (usually `http://localhost:8080`).

### Method 2: Python simple HTTP server
If you have Python installed, run:
```bash
python -m http.server 8000
```
Then visit `http://localhost:8000` in your browser.

---

## 📝 NEET UG Marking Scheme Reference
The application integrates the official National Testing Agency guidelines:
- **Correct Answer**: $+4$
- **Incorrect Answer**: $-1$
- **Unattempted**: $0$
- **Total Possible Score (180 questions)**: $720$ Marks
