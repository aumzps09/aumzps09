# GitHub Profile Setup — Surapong Phosu (`aumzps09`)

## What's included

| File | Purpose |
|------|---------|
| `README.md` | Profile page (banner, bio, tech stack, projects, stats, snake) |
| `.github/workflows/generate-snake.yml` | Contribution snake animation |
| `.github/workflows/blog-post.yml` | Auto-pull latest Medium posts |

## Deploy (3 steps)

### 1. Create the special repo on GitHub

Repo name **must** be exactly your username: `aumzps09`

```bash
# Option A — GitHub website
# New repository → name: aumzps09 → Public → Add a README → Create

# Option B — CLI (if gh is installed)
gh repo create aumzps09 --public --description "My GitHub profile" --source=. --remote=origin --push
```

### 2. Push this folder

```bash
cd ~/Desktop/aumzps09
git init
git add .
git commit -m "feat: setup GitHub profile README for Surapong Phosu"
git branch -M main
git remote add origin https://github.com/aumzps09/aumzps09.git
git push -u origin main
```

If the repo already exists with a README, use:

```bash
git pull origin main --allow-unrelated-histories
# resolve conflicts if any, keep our README
git push -u origin main
```

### 3. Enable workflow permissions (for snake + blog)

1. Open `https://github.com/aumzps09/aumzps09`
2. **Settings → Actions → General → Workflow permissions**
3. Select **Read and write permissions** → Save
4. **Actions** tab → run **Generate Snake** manually once
5. (Optional) run **Latest blog post workflow** after you have a Medium feed

## Customize mock data

Replace these placeholders in `README.md`:

| Placeholder | What to put |
|-------------|-------------|
| `surapong.phosu@example.com` | Real email |
| `linkedin.com/in/surapong-phosu` | Real LinkedIn |
| `medium.com/@surapongphosu` | Real Medium |
| `huggingface.co/aumzps09` | Real HF profile |
| Featured Projects table | Real repos + links |
| Blog feed in `blog-post.yml` | Real Medium RSS URL |

## Profile bio (GitHub settings)

Also update on GitHub → **Settings → Profile**:

- **Name:** Surapong Phosu
- **Bio:** AI Engineer · LLMs · RAG · MLOps
- **Location:** Thailand
- **Pronouns:** (optional)
- **Website:** portfolio URL if any

## After push

Your profile will show at: **https://github.com/aumzps09**
