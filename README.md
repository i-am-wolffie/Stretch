# Daily Stretch Routine

A progressive web app (PWA) with 18 guided stretches for post-gym recovery and desk posture correction, including a dedicated plantar fasciitis treatment section. Works offline and installs on your phone's home screen like a native app.

---

## Features

- **18 stretches** across three sections: Standing, Floor, and Plantar Fasciitis
- **Per-phase countdown timers** with start, pause, and reset controls
- **Auto-advance** — each timer automatically starts the next phase after completion
- **Audio beeps** — soft ticks in the last 5 seconds, two-tone beep on completion
- **Visual ring** — countdown ring shifts from gold to amber to red as time runs low
- **Expandable cards** — tap any stretch to reveal instructions, rationale, and timers
- **Offline support** — service worker caches all assets for use without internet
- **PWA installable** — sits on your home screen, opens full screen with no browser chrome

---

## Stretch Sections

### Phase 1 — Standing (Stretches 1–6)
Performed standing to warm the tissues before floor work.

| # | Stretch | Focus |
|---|---------|-------|
| 1 | Standing Chest Opener | Pectorals, thoracic extension |
| 2 | Doorway Chest Stretch | Anterior capsule, internal rotation |
| 3 | Standing Hip Flexor Lunge | Iliopsoas, rectus femoris |
| 4 | Standing Lat Stretch | Latissimus dorsi, teres major |
| 5 | Standing Calf & Achilles | Gastrocnemius, soleus |
| 6 | Standing Forward Fold | Hamstrings, lumbar decompression |

### Phase 2 — Floor (Stretches 7–16)
Stay on the floor from stretch 7 through to 16 — no need to get up between them.

| # | Stretch | Focus |
|---|---------|-------|
| 7 | Thoracic Extension Over Rolled Towel | Thoracic spine, kyphosis reversal |
| 8 | Thread the Needle | Thoracic rotation, rhomboids |
| 9 | Child's Pose with Lat Reach | Lats, thoracolumbar fascia |
| 10 | Figure-Four / Piriformis Stretch | Piriformis, sciatic nerve |
| 11 | Supine Glute Stretch | Gluteus maximus, sacroiliac joint |
| 12 | Supine Hamstring Stretch | Hamstrings, posterior chain |
| 13 | Kneeling Quad & Tucked-Toe | Quadriceps, plantar fascia |
| 14 | Butterfly / Groin Stretch | Hip adductors, groin |
| 15 | Seated Spinal Twist | Thoracic rotation, IT band |
| 16 | Suboccipital Release | Suboccipitals, tension headache prevention |

### Plantar Fasciitis Treatment (Stretches 17–18)
> **Important:** Do stretch 17 every morning before your first step out of bed — not just in this routine. That single habit is the most evidence-backed intervention for plantar fasciitis.

| # | Stretch | Focus |
|---|---------|-------|
| 17 | Seated Plantar Fascia Stretch | Plantar fascia, toe extensors — 3 × 30s each foot |
| 18 | Frozen Bottle Roll | Arch massage, anti-inflammatory cold therapy |

---

## File Structure

```
stretch-routine/
├── index.html       # Main app
├── manifest.json    # PWA manifest (name, icons, display mode)
├── sw.js            # Service worker (offline caching)
├── icon-192.png     # App icon (home screen, small)
└── icon-512.png     # App icon (splash screen, large)
```

---

## Hosting & Installation

This app must be served over HTTPS to function as a PWA. The easiest free option is GitHub Pages.

### Deploy to GitHub Pages

1. Create a free account at [github.com](https://github.com) if you don't have one
2. Create a new **public** repository (e.g. `stretch-routine`)
3. Upload all five files from this folder
4. Go to **Settings → Pages → Source** and select the `main` branch
5. Your app will be live at `https://yourusername.github.io/stretch-routine`

### Install on iPhone (Safari)

1. Open the GitHub Pages URL in Safari
2. Tap the **Share** button (box with arrow)
3. Tap **Add to Home Screen**
4. Tap **Add** — the app icon appears on your home screen

### Install on Android (Chrome)

1. Open the GitHub Pages URL in Chrome
2. A banner will appear automatically — tap **Add to Home Screen**
3. Or tap the three-dot menu and select **Install app**

Once installed, the app opens full screen with no browser bars and works completely offline.

---

## Usage Notes

- Tap any stretch card to expand it and reveal the timer
- Tap **Start** on the first phase — it will auto-advance through all phases in that stretch
- Each stretch includes the rationale for doing it and the muscles targeted
- The routine takes approximately 22 minutes in full
- For best results, use 5–7 evenings per week
- Never bounce a stretch — a strong sustained pull is correct; sharp or joint pain means stop

---

## Built With

- Vanilla HTML, CSS, and JavaScript — no frameworks or dependencies
- Web Audio API for beeps
- Web App Manifest + Service Worker for PWA capability
- DM Sans and DM Serif Display (Google Fonts)
