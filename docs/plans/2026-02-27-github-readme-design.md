# GitHub Profile README Design
**Design Document for wanshazamirul GitHub Profile**

**Date:** February 27, 2026
**Designer:** Shuhada (Senior Full Stack Developer)
**Partner:** Wan

---

## Overview

Redesign the GitHub profile README (wanshazamirul) to showcase all projects with:
- Prominent links to deployed projects (not just repos)
- Expandable file trees for each project
- Clean, balanced layout (minimalist but informative)

---

## Design Specifications

### Section 1: Header & Intro

**Purpose:** Friendly, personal introduction

**Elements:**
- Wave emoji 👋
- Name: "Shazwan Amirul"
- Tagline: "I make things I like, mostly for Malaysia 🇲🇾"
- GitHub badge

**Rationale:** Keeps existing authentic tagline, simple and clean.

---

### Section 2: Main Projects (⭐)

**Projects:**
1. dooitnow (Personal Finance)
2. Dapoqec (Food Ordering)
3. Waktu Solat Dashboard (Prayer Times)

**Card Structure:**
```
[LIVE DEMO BADGE - LINKED TO DEPLOYED URL]
Project Name + One-liner
Features (3-5 bullet points with emojis)
<details> collapsed file tree </details>
Tech badges (flat-square style)
[GitHub Repo Badge]
```

**Key Decisions:**
- Deployed URL is PRIMARY link (live demo badge at top)
- File tree collapsed by default (<details>)
- Tech badges use flat-square style (smaller footprint)
- GitHub repo link is secondary (bottom of card)

---

### Section 3: Side Quests (🎮)

**Projects:**
1. arwah (Tahlil Cards)
2. BangShamPayung (Iftar RSVP)

**Card Structure:**
Same as Main Projects but with "Side Quests" label and smaller footprint.

**Rationale:** Side projects get equal presentation treatment, just grouped separately.

---

### Section 4: Tech Stack Summary

**Format:** Code block with emojis for visual interest

```
Frontend    ⚛️ Next.js 16 • React • TypeScript
Styling     🎨 Tailwind CSS v4 • Framer Motion
UI          🧩 shadcn/ui • Lucide Icons
Backend     🔧 Node.js • Supabase
Tools       📦 Git • npm • Vercel
```

---

### Section 5: Quick Links Table

**Purpose:** At-a-glance reference table

**Columns:** Project | Live Demo | GitHub Repo

**Rationale:** Alternative navigation method for quick access.

---

### Section 6: Footer

**Elements:**
- "Made in Malaysia 🇲🇾"
- Small decorative GIF (parrot or similar)

---

## File Tree Format

Each project includes collapsible file tree:

```
<details>
<summary>📁 Project Structure</summary>

```
project-name/
├── src/
│   ├── app/
│   │   ├── (app)/
│   ├── components/
│   └── lib/
├── public/
└── README.md
```
</details>
```

**Decision:** Show only top-level structure (1-2 levels deep) to avoid overwhelming.

---

## Badge Styles

**Tech Badges:**
- Style: `flat-square` (compact)
- Logo: Include project logos
- Color: Official brand colors

**Link Badges:**
- Live Demo: Green/Blue with "🔗 Try It" or "🔗 Live Demo"
- GitHub Repo: Dark gray with "GitHub Repo"

---

## Deployment URLs

**Required Information from User:**

| Project | Repo | Deployed URL |
|---------|------|--------------|
| dooitnow | https://github.com/wanshazamirul/dooitnow | [PENDING] |
| Dapoqec | https://github.com/wanshazamirul/dapoqec | [PENDING] |
| Waktu Solat | https://github.com/wanshazamirul/waktu-solat-dashboard | [PENDING] |
| arwah | https://github.com/wanshazamirul/arwah | [PENDING] |
| BangShamPayung | https://github.com/wanshazamirul/bangshampayung | [PENDING] |

**Action:** User to provide deployed URLs before implementation.

---

## Visual Mockup

```
┌─────────────────────────────────────────────────────┐
│                    👋                               │
│                Shazwan Amirul                       │
│   I make things I like, mostly for Malaysia 🇲🇾     │
│                                                     │
│              [GitHub Badge]                         │
├─────────────────────────────────────────────────────┤
│  🚀 Featured Projects                               │
├─────────────────────────────────────────────────────┤
│                                                     │
│  [🔗 Live Demo]                                     │
│  💰 dooitnow                                        │
│  Your Personal Finance Companion                    │
│                                                     │
│  Features:                                          │
│  🇲🇾 Malaysian NLP input (400+ keywords)           │
│  🤖 AI-powered budget insights                     │
│  🕌 EPF/KWSP tracker, Zakat, LHDN tax              │
│                                                     │
│  ▶ 📁 Project Structure [expandable]               │
│                                                     │
│  [Next.js] [TS] [Framer] [GitHub Repo]             │
│                                                     │
├─────────────────────────────────────────────────────┤
│  🎮 Side Quests                                     │
│  (smaller cards for arwah, BangShamPayung)         │
├─────────────────────────────────────────────────────┤
│  🛠️ Stack                                          │
│  [Code block with tech summary]                    │
├─────────────────────────────────────────────────────┤
│  🔗 Quick Links                                     │
│  [Table with all projects]                         │
├─────────────────────────────────────────────────────┤
│        Made in Malaysia 🇲🇾                         │
│              [GIF]                                 │
└─────────────────────────────────────────────────────┘
```

---

## Implementation Notes

1. **File Paths:** Use `tree` command or manual listing for project structures
2. **Badge URLs:** Use shields.io for all badges
3. **Emoji Usage:** Consistent emoji per project (💰 finance, 🍜 food, 🕌 prayer, etc.)
4. **Responsiveness:** README should render well on mobile GitHub

---

## Success Criteria

- ✅ All 5 projects showcased
- ✅ Deployed URLs are prominent (not buried)
- ✅ File trees included for each project
- ✅ Balanced visual hierarchy
- ✅ Maintains authentic "I make things I like" personality
- ✅ Mobile-friendly rendering

---

## Next Steps

1. Collect deployed URLs from user
2. Generate file trees for each project
3. Write README.md
4. Commit to git

---

**Design Status:** ✅ APPROVED by Wan
**Ready for:** Implementation Plan
