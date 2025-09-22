
# Voluntracker (React + Firebase + Azure)

A **single-page** web app to log volunteer hours with **Firebase Auth (email/password)** and per-user storage in **Cloud Firestore**. Sessions persist (auto “remember me”). Deployed to **Azure Static Web Apps**.

> **Zero backend.** One file: `index.html`.

---

##  Features

- Email/password **login & register** (Firebase Auth)
- Per-user total hours in **Firestore** (`users/{uid}/profile/profile`)
- **+1 / –1** and **Set exact value** controls
- Realtime updates via Firestore listeners
- **CI/CD**: Push to GitHub → Azure redeploys automatically

---

## Project Structure

- **index.html** — Single-page app (React via CDN + Firebase Auth/Firestore)
- **README.md** — This file
- **.github/**
  - **workflows/**
    - **azure-static-web-apps-<id>.yml** — CI/CD workflow auto-created by Azure


Azure URL: https://witty-bay-0a7a6550f.1.azurestaticapps.net 
