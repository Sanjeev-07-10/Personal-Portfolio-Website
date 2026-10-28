# Sanjeev Velan S — 3D Developer Portfolio

A high-performance, futuristic 3D developer portfolio website built for **Sanjeev Velan S**, Computer Science and Engineering student at **Easwari Engineering College**.

![Portfolio Overview](public/favicon.svg)

---

## 🌟 Features & Highlights

- **Interactive 3D WebGL Hero Canvas**: Custom Three.js cybernetic icosahedron core with orbiting electron rings, glowing holographic core, and mouse parallax damping.
- **Ambient 3D Particle Constellation**: Deep space particles floating subtly in the background across sections.
- **Glassmorphism Design System**: Tailored dark theme (`#060812`) with neon cyan (`#38bdf8`) and purple (`#a855f7`) accents, glowing borders, and smooth backdrop-filter blurs.
- **Verified Credentials**:
  - **Easwari Engineering College** (Computer Science & Engineering)
  - **CGPA 8.4 / 10.0**
  - **110 LeetCode Problems Solved** (with live animated counter)
  - **Python & Java** core competency
  - **DSA & Web Development**
- **Centralized Configuration**: All personal details, social profile links, project entries, and achievements are centralized in `src/config/portfolio.ts` for instant customization.
- **Accessible & Responsive**: Fully responsive layout from 375px mobile screens to wide monitors with `prefers-reduced-motion` compliance.
- **Client-Side Form Validation**: Contact form with mailto fallback and confetti celebration upon valid submission.

---

## 🚀 Quick Start

### 1. Prerequisites
- **Node.js** v18+ (tested on Node v24)
- **npm** v9+

### 2. Run Locally in Development
```powershell
npm run dev
```
Open [http://localhost:5173](http://localhost:5173) in your browser.

### 3. Production Build
```powershell
npm run build
```
Generates optimized static output inside the `dist/` directory ready for deployment on Vercel, Netlify, or GitHub Pages.

---

## ⚙️ How to Customize Personal Details

All configuration is located in a single file:  
👉 **[`src/config/portfolio.ts`](src/config/portfolio.ts)**

### Update Links & Profiles:
1. **GitHub Profile**:
   ```ts
   socials: {
     github: {
       name: "GitHub",
       url: "https://github.com/your-username",
       isConfigured: true,
     }
   }
   ```
2. **LinkedIn Profile**:
   ```ts
   linkedin: {
     name: "LinkedIn",
     url: "https://linkedin.com/in/your-profile",
     isConfigured: true,
   }
   ```
3. **LeetCode Profile**:
   ```ts
   leetcode: {
     url: "https://leetcode.com/u/your-username",
     isConfigured: true,
   }
   ```
4. **Email Address**:
   Set `email: "your-email@domain.com"` and `isEmailConfigured: true` in `personal`.

5. **Adding Real Projects**:
   Replace placeholder projects in `projects` array with your actual project titles, descriptions, live demo URLs, and GitHub repos.

---

## 📁 Project Architecture

```
portfolio/
├── public/
│   └── favicon.svg                  # Modern SV monogram favicon
├── src/
│   ├── components/
│   │   ├── Navbar.tsx               # Sticky navbar with active section observer
│   │   ├── Hero.tsx                 # Striking hero screen with badges & 3D canvas
│   │   ├── ThreeHeroCanvas.tsx      # Three.js 3D WebGL holographic core
│   │   ├── ThreeBackgroundParticles.tsx # Ambient 3D particle constellation
│   │   ├── SectionHeading.tsx       # Reusable section title with badges
│   │   ├── About.tsx                # Verified education & background cards
│   │   ├── Skills.tsx               # Categorized tech stack (Python, Java, DSA, Web)
│   │   ├── Projects.tsx             # Project showcase with architecture blueprints
│   │   ├── ProjectCard.tsx          # Reusable glassmorphism project card
│   │   ├── LeetCode.tsx             # 110 LeetCode counter & topic breakdown
│   │   ├── Education.tsx            # Easwari Engineering College timeline & CGPA
│   │   ├── Achievements.tsx         # Verified highlights & configurable slots
│   │   ├── Contact.tsx              # Validated contact form + mailto fallback
│   │   ├── Footer.tsx               # Dynamic year, navigation, and brand
│   │   └── BrandIcons.tsx           # Crisp SVG GitHub and LinkedIn icons
│   ├── config/
│   │   └── portfolio.ts             # Central configuration file for all data
│   ├── index.css                    # Design tokens, glassmorphism, animations
│   ├── App.tsx                      # Root component assembling all sections
│   └── main.tsx                     # React entrypoint
├── index.html                       # SEO meta tags, Google Fonts, Open Graph
├── package.json
└── vite.config.ts
```

---

## 🛠️ Built With
- **React 19**
- **TypeScript**
- **Vite**
- **Three.js** (WebGL 3D graphics)
- **Lucide React** (icons)
- **Canvas Confetti** (interactive animations)
