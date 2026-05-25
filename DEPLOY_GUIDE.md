# 🚀 NestVerify — Deploy Guide
### Go from zero to live link in 30 minutes. No coding needed.

---

## What you need before starting
- [ ] A computer with a browser
- [ ] An email address (for GitHub + Vercel accounts)
- [ ] An Anthropic API key (instructions below)

---

## STEP 1 — Get your Anthropic API Key (5 minutes)

1. Go to **https://console.anthropic.com**
2. Click **"Sign Up"** and create a free account
3. After login, click **"API Keys"** in the left sidebar
4. Click **"Create Key"** → give it any name → click **"Create"**
5. **Copy the key** (starts with `sk-ant-...`) and save it somewhere safe
6. Click **"Billing"** in the sidebar → Add a card → Add $5 credit (you'll use maybe $0.50 testing)

✅ Done — you have your API key.

---

## STEP 2 — Upload code to GitHub (10 minutes)

1. Go to **https://github.com** → Sign up for a free account (or log in)
2. Click the **"+"** icon (top right) → **"New repository"**
3. Name it: `nestverify`
4. Set it to **Public**
5. Click **"Create repository"**
6. On the next page, click **"uploading an existing file"** link
7. **Drag and drop ALL the files and folders** from the `nestverify` folder I gave you
   - Make sure to include: `src/` folder, `public/` folder, `index.html`, `package.json`, `vite.config.js`, `vercel.json`, `.gitignore`
8. Scroll down, click **"Commit changes"**

✅ Done — your code is on GitHub.

---

## STEP 3 — Deploy on Vercel (5 minutes)

1. Go to **https://vercel.com** → Sign up with your GitHub account (free)
2. Click **"Add New Project"**
3. You'll see your GitHub repos — click **"Import"** next to `nestverify`
4. Vercel auto-detects it as a Vite project — don't change anything
5. Click **"Deploy"**
6. Wait ~60 seconds...
7. 🎉 You'll see **"Congratulations!"** with your live URL like `nestverify.vercel.app`

✅ Done — your app is live!

---

## STEP 4 — Use your app (2 minutes)

1. Open your live URL
2. Click **"+ Add Listing"**
3. Paste your Anthropic API key into the key field (it saves in your browser)
4. Fill in: Title, Location, Price
5. Upload 1–5 property images
6. Click **"Submit & Run AI Analysis"**
7. Watch the AI agent analyze in real time!
8. See the score, signals, and verdict

---

## How the scoring works

| Score | Verdict | What happens |
|-------|---------|--------------|
| 80–100% | ✅ Approved | Listing goes live automatically |
| 50–79% | ⚠️ Flagged | Goes to Review Queue for manual check |
| 0–49% | ❌ Rejected | Listing blocked |

---

## Sharing with your team

- Your live URL works for everyone — just share the link
- The API key field appears for whoever submits listings
- Reviewers can use the **"Review Queue"** tab to approve/reject flagged listings

---

## Cost estimate

| Usage | Approximate cost |
|-------|-----------------|
| 100 test listings | ~$0.30 |
| 1,000 listings/month | ~$3.00 |
| 10,000 listings/month | ~$30.00 |

You can set a monthly spending cap in your Anthropic account dashboard.

---

## Future upgrades (Phase 2)

When ready to scale, these are the next steps:
- Add a real database (Supabase — free tier) so listings persist for all users
- Add user authentication (email/password login)
- Add video support
- Add email notifications for flagged listings
- Add a custom domain name

---

## Need help?

If anything goes wrong:
1. Check that your API key is correct (starts with `sk-ant-`)
2. Make sure you uploaded ALL files to GitHub including the `src/` folder
3. In Vercel, check the **"Functions"** logs for any error messages

---

**Built with:** React + Vite + Anthropic Claude Vision API + Vercel
