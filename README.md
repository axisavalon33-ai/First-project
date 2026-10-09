# Vertigo vs Dizziness — VR exhibition app

A 30-second VR experience for a neuroscience exhibition (MEDSCOPE II · Medicolegal II · Neurology). The phone camera shows the real room, and the app changes that live video to show how each condition feels:

| Time | What the visitor sees |
|---|---|
| 0–3 s | Title poster (`poster.jpg`) |
| 3–6 s | "DIZZINESS" countdown: 3, 2, 1 |
| 6–18 s | **Dizziness**: vision blurs, sways, loses colour and "greys out" (lightheaded, faint) |
| 18–21 s | "VERTIGO" countdown: 3, 2, 1 |
| 21–33 s | **Vertigo**: the room spins and the view jerks side to side (nystagmus) |
| 33–60 s | Three explanation slides inside the headset (dizziness, vertigo, what to do next) |
| End | A full summary page to read after taking the headset off |

Tapping the screen at any time stops the experience and goes straight to the explanation.

---

## What you need

- An **Android phone with Chrome** (works best) or an iPhone with Safari
- A cheap **phone VR viewer** such as Google Cardboard (any viewer that holds a phone works)
- Internet access, but only the first time you open the page

## Step 1: Put the app online (one-time setup, about 5 minutes)

GitHub can host the app as a website for free. This is called **GitHub Pages**.

1. Go to <https://github.com/axisavalon33-ai/First-project> and sign in.
2. Click **Settings** in the top menu of the repository (the ⚙ gear icon).
3. In the left sidebar, click **Pages**.
4. Under **Build and deployment → Source**, choose **Deploy from a branch**.
5. Under **Branch**, choose `claude/vr-vertigo-dizziness-app-rnbmgw` (or `main` if the code has been merged there). Leave the folder as **/ (root)** and click **Save**.
6. Wait 1–2 minutes and refresh the page. A link like this appears at the top:
   **https://axisavalon33-ai.github.io/First-project/**

> The repository must be **public** to use free GitHub Pages. If it's private, go to Settings → General → scroll to the bottom → "Change visibility".

## Step 2: Open it on the phone

1. Open the link above in **Chrome** (Android) or **Safari** (iPhone).
2. Tip: use the browser menu → **Add to Home screen** so it opens like an app.
3. Choose **Headset mode**, then tap **Start experience**.
4. When asked to use the camera, tap **Allow**.
5. Turn the phone sideways and place it in the VR viewer.

To test it on a laptop without a headset, choose **Screen mode**.

## Step 3: At the exhibition

- Ask each visitor to **sit down** and read the warning on the start screen.
- Press **Start**, put the phone in the viewer, and hand it to the visitor.
- When it finishes, the visitor removes the headset and reads the summary.
- Press **"Next visitor — start again"** for the next person.
- Keep the phone **plugged into a charger** between visitors, because the camera uses a lot of battery.
- Turn screen brightness up and auto-rotate on.

## Changing things (no coding knowledge needed)

Everything is in one file, `index.html`. To edit it on GitHub, open the file, click the ✏️ pencil icon, make your change, then click **Commit changes**. The website updates within about a minute.

- **Timing or strength**: near the bottom of the file, find `SETTINGS`. Change the numbers (`title`, `countdown`, `dizzy`, `vertigo` are seconds). For example, `intensity: 0.5` gives a gentler experience.
- **Slide text in the headset**: find `SLIDES` just below `SETTINGS` and edit the sentences between the quotes `"..."`.
- **Title poster**: upload a new picture named exactly `poster.jpg` to replace it.
- **Summary page text**: search for `What to do next` and edit the plain sentences around it.

Only change the text inside quotes or between tags. Keep the commas, quotes and brackets in place.

## Troubleshooting

| Problem | Fix |
|---|---|
| A grid pattern shows instead of the camera | Camera permission was blocked. Tap the 🔒 lock icon next to the web address → Permissions → Camera → Allow, then reload. The page must be opened through the `https://` link, not as a downloaded file. |
| The screen goes to sleep | Turn off auto-lock/screen timeout in the phone settings. |
| The picture isn't split in two | On the start screen, choose **Headset mode**. |
| It feels too strong | Set `intensity` to `0.5` in `SETTINGS`. |

---

*For education only — this is not medical advice.*
