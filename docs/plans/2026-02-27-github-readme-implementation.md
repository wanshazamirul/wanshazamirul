# GitHub Profile README Implementation Plan

> **For Claude:** REQUIRED SUB-SKILL: Use superpowers:executing-plans to implement this plan task-by-task.

**Goal:** Redesign GitHub profile README with deployed project links, file trees, and balanced layout

**Architecture:** Single markdown file (README.md) with embedded HTML for badges, collapsible sections for file trees, and table-based quick links

**Tech Stack:** Markdown, HTML, shields.io badges

---

## Prerequisites

**Required Information from User:**

Before starting, collect these deployed URLs:

| Project | Repo | Deployed URL (Needed) |
|---------|------|----------------------|
| dooitnow | https://github.com/wanshazamirul/dooitnow | `___________` |
| Dapoqec | https://github.com/wanshazamirul/dapoqec | `___________` |
| Waktu Solat | https://github.com/wanshazamirul/waktu-solat-dashboard | `___________` |
| arwah | https://github.com/wanshazamirul/arwah | `___________` |
| BangShamPayung | https://github.com/wanshazamirul/bangshampayung | `___________` |

**Action:** Ask user for deployed URLs before proceeding with Task 1.

---

### Task 1: Read Current README

**Files:**
- Read: `C:\Users\Shazwan\Desktop\PROJECTS\DEVELOPMENT\wanshazamirul\README.md`

**Step 1: Read existing README**

```bash
cat "C:\Users\Shazwan\Desktop\PROJECTS\DEVELOPMENT\wanshazamirul\README.md"
```

**Purpose:** Understand current structure before replacing

**Step 2: Backup current README**

```bash
cp "C:\Users\Shazwan\Desktop\PROJECTS\DEVELOPMENT\wanshazamirul\README.md" "C:\Users\Shazwan\Desktop\PROJECTS\DEVELOPMENT\wanshazamirul\README.backup.md"
```

**Purpose:** Keep backup in case we need to reference original

---

### Task 2: Generate File Trees for Projects

**Files:**
- Reference: `C:\Users\Shazwan\Desktop\PROJECTS\DEVELOPMENT\dooitnow\`
- Reference: `C:\Users\Shazwan\Desktop\PROJECTS\DEVELOPMENT\dapoqec\`
- Reference: `C:\Users\Shazwan\Desktop\PROJECTS\DEVELOPMENT\waktu-solat-dashboard\`
- Reference: `C:\Users\Shazwan\Desktop\PROJECTS\DEVELOPMENT\arwah\`
- Reference: `C:\Users\Shazwan\Desktop\PROJECTS\DEVELOPMENT\archive\bangshampayung\`

**Step 1: Generate dooitnow file tree**

```bash
cd "C:\Users\Shazwan\Desktop\PROJECTS\DEVELOPMENT\dooitnow" && tree -L 2 -I "node_modules|.next|.git" --charset ascii
```

**Expected Output:** Structure showing src/, public/, key directories

**Step 2: Generate Dapoqec file tree**

```bash
cd "C:\Users\Shazwan\Desktop\PROJECTS\DEVELOPMENT\dapoqec" && tree -L 2 -I "node_modules|.next|.git" --charset ascii
```

**Step 3: Generate Waktu Solat file tree**

```bash
cd "C:\Users\Shazwan\Desktop\PROJECTS\DEVELOPMENT\waktu-solat-dashboard" && tree -L 2 -I "node_modules|.next|.git" --charset ascii
```

**Step 4: Generate arwah file tree**

```bash
cd "C:\Users\Shazwan\Desktop\PROJECTS\DEVELOPMENT\arwah" && tree -L 2 -I "node_modules|.next|.git" --charset ascii
```

**Step 5: Generate BangShamPayung file tree**

```bash
cd "C:\Users\Shazwan\Desktop\PROJECTS\DEVELOPMENT\archive\bangshampayung" && tree -L 2 -I "node_modules|.next|.git" --charset ascii
```

**Note:** If `tree` command not available, use manual listing or alternative method.

---

### Task 3: Write New README.md

**Files:**
- Modify: `C:\Users\Shazwan\Desktop\PROJECTS\DEVELOPMENT\wanshazamirul\README.md`

**Step 1: Write complete README content**

Create new `README.md` with the following content:

```markdown
<p align="center">
  <span>👋</span>
</p>

<h1 align="center">Shazwan Amirul</h1>
<p align="center">
  <em>I make things I like, mostly for Malaysia 🇲🇾</em>
</p>

<p align="center">
  <a href="https://github.com/wanshazamirul" target="_blank">
    <img src="https://img.shields.io/badge/GitHub-333333?style=for-the-badge&logo=github" alt="GitHub" />
  </a>
</p>

---

## 🚀 Featured Projects

### ⭐ Main Projects

---

<a href="https://dooitnow-demo.vercel.app">
  <picture>
    <img src="https://img.shields.io/badge/🔗_Live_Demo-blue?style=for-the-badge" alt="Live Demo">
  </picture>
</a>

## 💰 dooitnow
*Your Personal Finance Companion - Track, Budget, Grow*

**Features:**
- 🇲🇾 Malaysian NLP input (400+ keywords: mamak, Grab, Touch n Go)
- 🤖 AI-powered budget insights & spending forecasts
- 🕌 EPF/KWSP tracker, Zakat calculator, LHDN tax categories
- 💾 100% local storage (privacy-first)
- 📱 PWA-ready with glass morphism UI

<details>
<summary>📁 Project Structure</summary>

```
dooitnow/
├── src/
│   ├── app/
│   │   ├── (app)/
│   │   │   ├── dashboard/      # Overview & insights
│   │   │   ├── transactions/   # Full CRUD with NLP
│   │   │   ├── analytics/      # Visual charts
│   │   │   ├── budgets/        # AI budget tracking
│   │   │   ├── tax/            # LHDN tracker
│   │   │   └── settings/
│   ├── components/
│   │   ├── glass/              # Glass morphism UI
│   │   ├── layout/             # FAB, bottom-nav
│   │   └── ui/                 # Reusable components
│   └── lib/
│       ├── malaysian-nlp.ts    # 400+ keywords
│       ├── budget-intelligence.ts
│       └── tax-tracker.ts
├── public/
└── README.md
```
</details>

**Tech:** [![Next.js](https://img.shields.io/badge/Next.js-16-black?style=flat-square&logo=next.js)](https://nextjs.org) [![TypeScript](https://img.shields.io/badge-TS-5.7-blue?style=flat-square&logo=typescript)](https://www.typescriptlang.org) [![Framer Motion](https://img.shields.io/badge/Framer-12-ff0066?style=flat-square)](https://www.framer.com) [![Tailwind](https://img.shields.io/badge/Tailwind-v4-06B6D4?style=flat-square&logo=tailwind-css)](https://tailwindcss.com)

[![View Code](https://img.shields.io/badge/GitHub-Repo-333333?style=for-the-badge&logo=github)](https://github.com/wanshazamirul/dooitnow)

---

<a href="https://dapoqec-demo.vercel.app">
  <picture>
    <img src="https://img.shields.io/badge/🔗_Order_Now-green?style=for-the-badge" alt="Order Now">
  </picture>
</a>

## 🍜 Dapoqec
*Malaysian Food Ordering with Infaq Charity*

**Features:**
- 🛒 Food ordering with cart management
- 🤲 Infaq charity integration (Ramadhan feature)
- 📊 MOQ (Minimum Order Quantity) system
- 💳 Weekly sales tracking
- 🎨 Glass morphism UI

<details>
<summary>📁 Project Structure</summary>

```
dapoqec/
├── src/
│   ├── app/
│   │   ├── (app)/
│   │   │   ├── menu/           # Food menu
│   │   │   ├── cart/           # Shopping cart
│   │   │   ├── infaq/          # Charity feature
│   │   │   └── admin/          # Sales dashboard
│   ├── components/
│   │   ├── glass/              # Glass morphism
│   │   └── ui/
│   └── lib/
│       └── supabase.ts         # Database client
├── public/
└── README.md
```
</details>

**Tech:** [![Next.js](https://img.shields.io/badge/Next.js-16-black?style=flat-square&logo=next.js)](https://nextjs.org) [![Supabase](https://img.shields.io/badge/Supabase-3ECF8E?style=flat-square&logo=supabase)](https://supabase.com) [![TypeScript](https://img.shields.io/badge/TS-blue?style=flat-square&logo=typescript)](https://www.typescriptlang.org)

[![View Code](https://img.shields.io/badge/GitHub-Repo-333333?style=for-the-badge&logo=github)](https://github.com/wanshazamirul/dapoqec)

---

<a href="https://waktu-solat-demo.vercel.app">
  <picture>
    <img src="https://img.shields.io/badge/🔗_View_Times-purple?style=for-the-badge" alt="View Times">
  </picture>
</a>

## 🕌 Waktu Solat Dashboard
*Prayer Times for 24 Malaysian Zones*

**Features:**
- 🕐 Prayer times for 24 Malaysian zones
- 📖 Hadith of the Hour widget (24 hadiths, hourly rotation)
- 📅 Hijri Calendar widget with Malay day names
- 🌤️ Weather information (where available)
- ⏱️ Countdown timer to next prayer
- 🖥️ Fullscreen kiosk mode

<details>
<summary>📁 Project Structure</summary>

```
waktu-solat-dashboard/
├── src/
│   ├── app/
│   │   ├── page.tsx            # Main dashboard
│   │   ├── layout.tsx
│   │   └── globals.css
│   ├── components/
│   │   ├── PrayerTimes.tsx     # Main prayer card
│   │   ├── HadithWidget.tsx    # Rotating hadiths
│   │   ├── HijriCalendar.tsx   # Hijri calendar
│   │   └── WeatherWidget.tsx
│   └── lib/
│       ├── jakim-api.ts        # Prayer times API
│       └── hijri-calendar.ts   # Hijri calculations
├── public/
└── README.md
```
</details>

**Tech:** [![Next.js](https://img.shields.io/badge/Next.js-16-black?style=flat-square&logo=next.js)](https://nextjs.org) [![date-fns](https://img.shields.io/badge/date--fns-4.0-red?style=flat-square)](https://date-fns.org) [![Framer Motion](https://img.shields.io/badge/Framer-12-ff0066?style=flat-square)](https://www.framer.com)

[![View Code](https://img.shields.io/badge/GitHub-Repo-333333?style=for-the-badge&logo=github)](https://github.com/wanshazamirul/waktu-solat-dashboard)

---

### 🎮 Side Quests
<small>Fun experiments & side projects</small>

---

<a href="https://arwah-demo.vercel.app">
  <picture>
    <img src="https://img.shields.io/badge/🔗_Try_It-green?style=for-the-badge" alt="Try It">
  </picture>
</a>

## 🪦 arwah
*Tahlil Card Generator*

Auto-processes photos into memorial cards (grayscale, round crop, feather edges).

<details>
<summary>📁 Project Structure</summary>

```
arwah/
├── src/
│   ├── app/
│   │   ├── page.tsx            # Canvas processing
│   │   └── layout.tsx
│   └── lib/
│       └── image-processor.ts  # Grayscale, crop, feather
├── public/
│   ├── template.jpg            # Tahlil template
│   └── manifest.json
└── README.md
```
</details>

**Tech:** [![Next.js](https://img.shields.io/badge/Next.js-16-black?style=flat-square&logo=next.js)](https://nextjs.org) [![Canvas](https://img.shields.io/badge/Canvas-API-orange?style=flat-square)](https://developer.mozilla.org/en-US/docs/Web/API/Canvas_API)

[![View Code](https://img.shields.io/badge/GitHub-Repo-333333?style=for-the-badge&logo=github)](https://github.com/wanshazamirul/arwah)

---

<a href="https://bangshampayung-demo.vercel.app">
  <picture>
    <img src="https://img.shields.io/badge/🔗_RSVP_Now-green?style=for-the-badge" alt="RSVP">
  </picture>
</a>

## 🎉 BangShamPayung
*Iftar RSVP for Ramadhan*

Simple RSVP system for breaking fast together.

<details>
<summary>📁 Project Structure</summary>

```
bangshampayung/
├── src/
│   ├── app/
│   │   ├── page.tsx            # RSVP form
│   │   └── api/
│   │       └── rsvp/           # Supabase integration
│   └── components/
│       └── RSVPCard.tsx
├── public/
│   └── manifest.json
└── README.md
```
</details>

**Tech:** [![Next.js](https://img.shields.io/badge/Next.js-16-black?style=flat-square&logo=next.js)](https://nextjs.org) [![Supabase](https://img.shields.io/badge/Supabase-3ECF8E?style=flat-square&logo=supabase)](https://supabase.com)

[![View Code](https://img.shields.io/badge/GitHub-Repo-333333?style=for-the-badge&logo=github)](https://github.com/wanshazamirul/bangshampayung)

---

## 🛠️ Stack

```
Frontend    ⚛️ Next.js 16 • React • TypeScript
Styling     🎨 Tailwind CSS v4 • Framer Motion
UI          🧩 shadcn/ui • Lucide Icons
Backend     🔧 Node.js • Supabase
Tools       📦 Git • npm • Vercel
```

---

## 🔗 Quick Links

| Project | Live Demo | GitHub Repo |
|---------|-----------|-------------|
| 💰 dooitnow | [Demo →](https://dooitnow-demo.vercel.app) | [Repo →](https://github.com/wanshazamirul/dooitnow) |
| 🍜 Dapoqec | [Demo →](https://dapoqec-demo.vercel.app) | [Repo →](https://github.com/wanshazamirul/dapoqec) |
| 🕌 Waktu Solat | [Demo →](https://waktu-solat-demo.vercel.app) | [Repo →](https://github.com/wanshazamirul/waktu-solat-dashboard) |
| 🪦 arwah | [Try →](https://arwah-demo.vercel.app) | [Repo →](https://github.com/wanshazamirul/arwah) |
| 🎉 BangShamPayung | [RSVP →](https://bangshampayung-demo.vercel.app) | [Repo →](https://github.com/wanshazamirul/bangshampayung) |

---

<p align="center">
  <small>
    <em>Made in Malaysia 🇲🇾</em>
  </small>
</p>

<p align="center">
  <img src="https://media.giphy.com/media/v1.Y2lkPTc5MGI3NjExM3AybnB3eGZ3eGZ3eGZ3eGZ3eGZ3eGZ3eGZ3eGZ3eGZ3eGZ3/L8A2CLpJJW5d3NR5Tt/giphy.gif" width="80" />
</p>
```

**Step 2: Verify file was created**

```bash
cat "C:\Users\Shazwan\Desktop\PROJECTS\DEVELOPMENT\wanshazamirul\README.md" | head -20
```

**Expected Output:** Should show the header with 👋, "Shazwan Amirul", and tagline

---

### Task 4: Replace Placeholder URLs

**Files:**
- Modify: `C:\Users\Shazwan\Desktop\PROJECTS\DEVELOPMENT\wanshazamirul\README.md`

**Step 1: Replace all demo URLs with actual deployed URLs**

Search and replace the following placeholders:

| Placeholder | Replace With |
|-------------|--------------|
| `https://dooitnow-demo.vercel.app` | User's actual dooitnow URL |
| `https://dapoqec-demo.vercel.app` | User's actual Dapoqec URL |
| `https://waktu-solat-demo.vercel.app` | User's actual Waktu Solat URL |
| `https://arwah-demo.vercel.app` | User's actual arwah URL |
| `https://bangshampayung-demo.vercel.app` | User's actual BangShamPayung URL |

**Action:** Use user-provided URLs from Prerequisites section

**Step 2: Verify all links are correct**

```bash
grep -o "https://[^)]*" "C:\Users\Shazwan\Desktop\PROJECTS\DEVELOPMENT\wanshazamirul\README.md" | sort -u
```

**Expected:** Should list all unique URLs - verify they match user's actual deployed URLs

---

### Task 5: Verify Markdown Rendering

**Step 1: Check for markdown syntax errors**

```bash
cd "C:\Users\Shazwan\Desktop\PROJECTS\DEVELOPMENT\wanshazamirul"
```

Then manually review in VS Code or:

```bash
# No specific markdown linter, manual review recommended
# Check for: unclosed tags, malformed links, broken HTML
```

**Manual Checklist:**
- [ ] All `<details>` tags have closing `</details>`
- [ ] All `<a>` tags have closing `</a>`
- [ ] All `<picture>` tags have closing `</picture>`
- [ ] All images have alt text
- [ ] All links are formatted correctly
- [ ] Code blocks are properly fenced with ``` ```

---

### Task 6: Commit Changes

**Step 1: Stage changes**

```bash
cd "C:\Users\Shazwan\Desktop\PROJECTS\DEVELOPMENT\wanshazamirul"
git add README.md
```

**Step 2: Commit with descriptive message**

```bash
git commit -m "Redesign GitHub README with project cards, file trees, and deployed links"
```

**Expected Output:** Commit created with hash

**Step 3: Push to GitHub**

```bash
git push origin main
```

**Note:** Branch name may be `master` instead of `main` - verify first:

```bash
git branch --show-current
```

---

### Task 7: Verify on GitHub

**Step 1: Open GitHub profile**

Navigate to: `https://github.com/wanshazamirul`

**Step 2: Visual Checklist**

Verify the following render correctly:
- [ ] Header with wave emoji, name, tagline
- [ ] "Featured Projects" section
- [ ] Project cards with Live Demo badges (clickable)
- [ ] File trees collapsed by default
- [ ] Tech badges visible
- [ ] GitHub repo links working
- [ ] Side Quests section
- [ ] Tech stack code block
- [ ] Quick links table
- [ ] Footer with Malaysia flag

**Step 3: Test all links**

Click each link to verify:
- All Live Demo badges navigate to deployed URLs
- All GitHub repo badges navigate to correct repos
- Quick links table links work

---

## Testing Strategy

**Manual Testing Required:**
1. View README on GitHub (not just locally)
2. Test every link (10+ links total)
3. Expand each file tree to verify formatting
4. View on mobile to ensure responsive rendering
5. View in dark mode and light mode

**No Automated Tests:** This is static markdown - manual verification is sufficient

---

## Rollback Plan

If something goes wrong:

```bash
cd "C:\Users\Shazwan\Desktop\PROJECTS\DEVELOPMENT\wanshazamirul"
git checkout HEAD~1 -- README.md  # Revert to previous version
# OR
cp README.backup.md README.md     # Restore from backup
git push origin main --force      # Force push rollback
```

---

## Completion Criteria

- [ ] All deployed URLs collected from user
- [ ] README.md written with all sections
- [ ] All placeholder URLs replaced with actual URLs
- [ ] File trees included for all 5 projects
- [ ] Changes committed to git
- [ ] Changes pushed to GitHub
- [ ] Verified rendering on GitHub profile
- [ ] All links tested and working

---

**Estimated Time:** 30-45 minutes (mostly manual verification)
**Risk Level:** Low (rollback is trivial)
**Dependencies:** User must provide deployed URLs before Task 4
