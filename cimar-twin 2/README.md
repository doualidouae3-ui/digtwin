# CIMAR Digital Twin — Safi Plant
### Deployment Guide

---

## What's in the ZIP

```
cimar-twin/
├── index.html     <- The entire app (single file, no build needed)
├── render.yaml    <- Render.com auto-config
└── README.md      <- This file
```

---

## STEP-BY-STEP DEPLOYMENT

### Step 1 — Upload to GitHub

1. Go to github.com and sign in (or create a free account)
2. Click the + icon (top right) -> New repository
3. Name it "cimar-digital-twin" -> click Create repository
4. On the next screen, click "uploading an existing file"
5. Drag and drop all 3 files from this folder (index.html, render.yaml, README.md)
6. Scroll down -> click Commit changes

Your files are now on GitHub.

---

### Step 2 — Deploy on Render

1. Go to render.com and sign in (or create a free account)
2. Click New + -> Static Site
3. Click "Connect a repository" -> authorize GitHub if prompted
4. Select your "cimar-digital-twin" repository
5. Fill in the settings:

   Name:              cimar-digital-twin (or anything you like)
   Branch:            main
   Root Directory:    (leave EMPTY)
   Build Command:     (leave EMPTY)
   Publish Directory: .

6. Click Create Static Site
7. Wait ~30 seconds
8. Render gives you a live URL like: https://cimar-digital-twin.onrender.com

DONE. Share that URL with your team.

---

### Step 3 — Custom Domain (Optional)

Render dashboard -> your site -> Settings -> Custom Domain
Add your domain and follow the DNS instructions.

---

## Local Preview (No Internet Required)

Open a terminal in this folder and run:

    python3 -m http.server 8080

Then open: http://localhost:8080

NOTE: Do NOT just double-click index.html — use a local server.

---

## Features

- Full 3D cement production line (Crusher -> Raw Mill -> Preheater Tower -> Rotary Kiln -> Cooler -> Cement Mills x2 -> Silos x4)
- Click any 3D component to inspect it (camera flies to it, sidebar updates)
- Drag to orbit, scroll to zoom, R key to reset
- ISO / TOP / SIDE / KILN view presets with smooth animated transitions
- Animated particles: material flow, kiln heat exhaust, chimney smoke
- Live sensor data updating every 2.2 seconds
- Active alert: Cement Mill 2 bearing warning (pulsing orange ring)
- 6 tabs: 3D Twin, Live Monitor, Energy Flow, Alerts, Simulate, AI Briefing

---

## Controls

DRAG   -> Rotate the scene
SCROLL -> Zoom in/out
CLICK  -> Select a component
R key  -> Reset to default view

---

CIMAR AI Plant Intelligence Platform -- Safi, Morocco
