[README (1).md](https://github.com/user-attachments/files/28687886/README.1.md)
# 🏡 Team Smith HQ — Parker's Jobs

A chore tracker for Parker Smith, backed by Supabase so every completed job is saved and tracked over time.

## Features

- ✅ Tap to mark jobs done — saves instantly to Supabase
- 📅 Completion date shown on each card
- 📊 History tab with full log + per-job summary
- 💰 Running earnings tracker with progress bar

## Stack

- Plain HTML/CSS/JS (no build step needed)
- [Supabase](https://supabase.com) for persistent storage

---

## Setup

### 1. Supabase — Create the table

1. Go to your [Supabase project](https://supabase.com/dashboard/project/xbqhtcqvbcndikuqsesz)
2. Open the **SQL Editor**
3. Paste and run the contents of `schema.sql`

This creates:
- `job_completions` table — every completion is a row
- `job_summary` view — aggregated totals per job

### 2. Run the app

No build step needed. Just open `index.html` in a browser, or deploy to any static host:

**GitHub Pages:**
```bash
git init
git add .
git commit -m "Initial commit"
git branch -M main
git remote add origin https://github.com/YOUR_USERNAME/parker-jobs.git
git push -u origin main
```
Then in GitHub → Settings → Pages → set source to `main` branch.

**Netlify / Vercel:** drag and drop the folder.

---

## Files

| File | Purpose |
|---|---|
| `index.html` | The full app |
| `schema.sql` | Supabase table + view setup |
| `README.md` | This file |

---

Made with 💛 for Parker Smith
