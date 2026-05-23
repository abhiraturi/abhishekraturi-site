# Project Documentation

## 1. Project Overview
This is a static website built with **Hugo** and hosted on **Netlify**.

## 2. Local Development & Setup
To manage your site, you will be working from your local directory: `/Users/abhishekraturi/gitlab_projects/my-profile`[cite: 1].

*   **Navigate to your workspace:**
    `cd /Users/abhishekraturi/gitlab_projects/my-profile`[cite: 1]
*   **Run Local Server:** 
    `hugo server -D` (The `-D` flag includes draft posts)[cite: 1].
*   **Local Validation:**
    Before pushing, always verify your build locally by running: `hugo --gc --minify`[cite: 1].

## 3. Deployment Workflow
This project utilizes a manual trigger process via the Netlify dashboard to ensure controlled production updates[cite: 1].

1.  **Develop & Test Locally:**
    *   Make your changes within `/Users/abhishekraturi/gitlab_projects/my-profile`[cite: 1].
    *   Verify changes by running `hugo server -D`[cite: 1].
2.  **Push to GitHub:**
    *   Stage your changes: `git add .`[cite: 1]
    *   Commit your changes: `git commit -m "Your descriptive message"`[cite: 1]
    *   Push to the repository: `git push`[cite: 1]
3.  **Trigger Deployment:**
    *   Navigate to the [Netlify Deploys Dashboard](https://app.netlify.com/projects/abhishekraturi/deploys)[cite: 1].
    *   Ensure the `main` branch is selected and initiate the deployment process[cite: 1].
4.  **Verify Production:**
    *   Once the build completes, navigate to your live website to confirm the updates[cite: 1].

## 4. Maintenance & Future Changes
*   **Config Changes:** Site-wide settings are located in `hugo.toml` (or `config.toml`)[cite: 1]. 
*   **Global Search:** If you rename a service or tool, use your IDE to search for the old term across all files to ensure full coverage[cite: 1].

## 5. Troubleshooting
*   **Issue:** Changes pushed to GitHub aren't appearing on the live site.
    *   **Fix:** Ensure you have navigated to the [Netlify Deploys Dashboard](https://app.netlify.com/projects/abhishekraturi/deploys) and initiated the deployment for the `main` branch[cite: 1].
*   **Issue:** Build fails on Netlify.
    *   **Fix:** Compare your local `hugo` version with the `HUGO_VERSION` set in your Netlify Environment Variables[cite: 1].

---
*Maintained by: Abhishek Raturi*
*Last Updated: 2026-05-23*
