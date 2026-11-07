# Deploy MCheck® Handoff on Vercel

The site is one static file (`index.html`) plus `vercel.json`. There is no build step.

## Option A: Vercel CLI (fastest, about 2 minutes)

1. Install Node.js 18 or newer from https://nodejs.org.
2. Unzip `mcheck-handoff-vercel.zip` and open a terminal in the unzipped folder.
3. Run:

   ```bash
   npx vercel
   ```

4. Log in when asked (GitHub, GitLab, Bitbucket or email), then answer the prompts:
   - Set up and deploy? **Y**
   - Which scope? **your account**
   - Link to existing project? **N**
   - Project name? **mcheck-handoff** (or any name)
   - In which directory is your code located? **./**
   - Want to modify these settings? **N** (Vercel detects "Other", no build command)
5. You get a preview URL. Publish to production with:

   ```bash
   npx vercel --prod
   ```

## Option B: Import from GitHub (auto-deploys on every push)

1. Put the files in a GitHub repository (the `vrajshah2708-art/HiLabs` repo already has them).
2. Go to https://vercel.com/new and click **Import** next to the repository.
3. Settings:
   - Framework Preset: **Other**
   - Root Directory: **./**
   - Build Command: leave empty
   - Output Directory: leave empty
4. Click **Deploy**.
5. If the code is on a branch other than the production branch, either merge it into that branch, or change it under **Project → Settings → Git → Production Branch**.

## After deploying

- Your link looks like `https://mcheck-handoff.vercel.app`.
- `?tour=1` starts the guided tour directly: `https://<your-app>.vercel.app/?tour=1`
- `?welcome=1` shows the welcome screen again.
- To use a custom domain: **Project → Settings → Domains → Add**.
- If deployment protection is on, turn it off so reviewers can open the link: **Project → Settings → Deployment Protection → Vercel Authentication → Disabled**.

## Updating the site

- CLI: replace `index.html`, then run `npx vercel --prod` again.
- GitHub: push the change; Vercel redeploys automatically.
