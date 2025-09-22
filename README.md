# Voluntracker (React + Firebase + Azure)

A **single-page** web app to track volunteer hours with **email/password login** and a per-user **activity log**.  
No build step, no server — just one `index.html` deployed to **Azure Static Web Apps**.

---

## What it does

- **Auth**: Firebase Auth (email/password) with **persistent sessions**.
- **Totals**: Per-user total hours at `users/{uid}/profile/profile`.
- **Activity Log** (latest 20):
  - **Manual entries**: `what` (description), `when` (date), `hours` (adds to total).
  - **Auto “adjustments”**: pressing **+1 / –1** or **Set** creates an entry with the delta.
- **Realtime UI**: Totals and recent activity update instantly via Firestore listeners.

---

## Project Structure

- **index.html** — Single-page app (React via CDN + Firebase Auth/Firestore)
- **README.md** — This file
- **.github/**
  - **workflows/**
    - **azure-static-web-apps-<id>.yml** — CI/CD workflow created by Azure

Azure URL: https://witty-bay-0a7a6550f.1.azurestaticapps.net 
