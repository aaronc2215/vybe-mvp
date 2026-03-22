# Vybe — Local Event Discovery App

**CEN 4930: Open Source for Entrepreneurs · Group 6 · Assignment 4**

Vybe is an open-source mobile event discovery application that helps young adults (18–35) find local events that match their personal interests — without the noise of mainstream social platforms.

---

## Live Demo

> Open '(https://aaronc2215.github.io/vybe-mvp/)' in any browser — no install, no build step, no dependencies.

```bash
git clone https://github.com/YOUR_USERNAME/vybe-mvp.git
cd vybe-mvp
open index.html   # macOS
# or just double-click index.html on Windows/Linux
```

---

## What the Prototype Does

This is a medium-fidelity interactive prototype built as a single HTML file. It simulates the core MVP user flows end-to-end using seeded event data and in-memory state.

### Working Features

| Feature | Status | Notes |
|---|---|---|
| Interest tag onboarding | ✅ Live | Select interests → feed personalizes |
| Geo-based event feed | ✅ Live | Seeded events, filterable by category |
| Event detail view | ✅ Live | Full info, map placeholder, going count |
| Save / heart events | ✅ Live | Persists in session, visible in Saved tab |
| RSVP to events | ✅ Live | Toggles, auto-saves event |
| Host: Post an Event form | ✅ Live | Full form with category picker |
| Pay-to-post flow | ✅ Live | $10 fee UI (payment not connected) |
| Posted events appear in feed | ✅ Live | New events show up immediately |
| Saved tab | ✅ Live | Lists all saved/RSVP'd events |

### Mocked / Simulated

| Feature | Status | Notes |
|---|---|---|
| Real geolocation | 🟡 Mocked | Hardcoded to Cape Coral, FL |
| Payment processing | 🟡 Mocked | Stripe UI simulated, no real charge |
| User authentication | 🟡 Bypassed | No login required for prototype |
| Push notifications | ❌ Deferred | Out of scope for MVP |
| Real map tiles | 🟡 Placeholder | Map pin UI shown, no live tiles |

---

## Screenshots

### Onboarding — Interest Selection
Pick your interests to personalize your feed.

<img width="464" height="899" alt="image" src="https://github.com/user-attachments/assets/550d8e35-7d46-4580-b068-51d70a6ba06d" />


### Event Feed
Personalized, filterable feed of nearby events. Location is visible at the top.

<img width="465" height="889" alt="image" src="https://github.com/user-attachments/assets/0792d51c-f49e-4d5c-9a08-0bccc36e48d0" />


### Event Detail View
Full event info with RSVP and save actions.

<img width="440" height="983" alt="image" src="https://github.com/user-attachments/assets/9d37b294-08c9-4e7e-8580-336b595bf6d7" />


### Post an Event (Host Flow)
Hosts fill in event details and pay to publish.

<img width="476" height="1063" alt="image" src="https://github.com/user-attachments/assets/80c5b985-5879-47a0-a8f5-7d8d64c318a6" />


---

## Tech Stack

| Tool | Purpose | License |
|---|---|---|
| HTML / CSS / JS | Single-file prototype | — |
| React Native *(planned)* | Production mobile app | MIT |
| Expo *(planned)* | RN toolchain | MIT |
| Node.js + Express *(planned)* | REST API backend | MIT |
| PostgreSQL *(planned)* | Database | PostgreSQL License |
| Leaflet.js *(planned)* | Map rendering | BSD 2-Clause |
| Stripe *(planned)* | Pay-to-post payments | Proprietary |

---

## Project Structure

```
vybe-mvp/
├── index.html        # Full interactive prototype (single file)
├── README.md         # This file
└── screenshots/      # Demo screenshots
```

---

## User Flows to Demo

### Flow 1 — Attendee
1. Open `index.html`
2. Select 2–3 interest tags → tap **"Find events near me"**
3. Browse the personalized feed — try the category filter chips
4. Tap any event card → view detail page
5. Tap **RSVP** (turns green) → tap heart to save
6. Tap **Saved** tab in nav to see saved events

### Flow 2 — Event Host
1. From the feed, tap **+** (top right) or **Post** in the nav bar
2. Fill in event title, pick a category, add date/time/location
3. Tap **"Publish event — $10.00"**
4. See success screen → tap back to feed
5. Your event now appears in the feed

---

## Open Source Rationale

Vybe is built open-source for strategic reasons, not just cost:

- **Algorithmic transparency** — the community can verify events are ranked by relevance and geography, not hidden ad auctions. This builds trust with a demographic skeptical of platforms like Facebook.
- **Federated hosting model** — the open codebase enables universities and municipalities to run their own Vybe instances, which is the foundation of our SaaS revenue stream.
- **MIT License on the core** — removes barriers for contributors and enterprise evaluators to inspect, fork, and deploy the platform.

---

## License

MIT License — see `LICENSE` for details.

---

## Group 6

CEN 4930 — Open Source for Entrepreneurs  

*Aaron Cole · Drake Pollard · Angelo Diaz 
