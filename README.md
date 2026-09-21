# 🌿 Warm Stationery Notion Widgets for ADHD & Deep Flow
### Minimal, Calming Embeds Designed for Focus & Everyday Dopamine

Thank you for purchasing this stationery widget pack! These widgets were crafted from the ground up with pure HTML, CSS, and JavaScript—designed specifically for **ADHD minds** who need a calm, grounded, clutter-free workspace inside Notion.

---

## 📦 What's Included

1. **Focus Timer (`pomodoro/index.html`)**
   - Elegant circular SVG progress ring in sage green.
   - Modes: **Focus (25m)**, **Short break (5m)**, and **Long break (15m)**.
   - 4-cycle daily focus tracker (`Today: 2 of 4`) with tactile filled dots.
   - Driftless real-time engine: stays 100% accurate even when backgrounded or minimized.
   - Soft synthesized chime (generated via Web Audio API, no external audio files needed).
   - Quick settings drawer (gear icon) to customize session lengths anytime.

2. **Dopamine Menu (`dopamine-menu/index.html`)**
   - 5 core categories with custom icons: **Move**, **Sense**, **Create**, **Connect**, and **Rest**.
   - Pre-filled with ADHD-friendly low-friction ideas (e.g. "stretch", "cold water on face", "doodle", "voice note").
   - Add your own custom rewards or remove existing ones in 1 click.
   - **"Pick a reward for me"** button: instantly chooses a soothing reward when you feel stuck or low-energy.
   - Category filter pills + "Another one" re-roll button.
   - Saved automatically to browser `localStorage`.

3. **Showcase Preview (`preview.html`)**
   - Side-by-side interactive playground to test both widgets.
   - Test widths: `320px` (sidebar), `460px` (callout), `650px` (wide), and full responsive.
   - Light / Dark mode toggle simulator.

---

## 🚀 Step 1: Host Your Widgets (Free & Permanent)

To embed custom HTML widgets into Notion, they need a web link (`https://...`). You can host them **100% free** using **GitHub Pages** (recommended) or **Cloudflare / Netlify**.

### Option A: GitHub Pages (Recommended)
1. Go to [GitHub.com](https://github.com) and log in (or create a free account).
2. Click the **`+`** icon in the top right &rarr; **New repository**.
3. Name it (for example: `notion-widgets`), select **Public**, and click **Create repository**.
4. In the repository page, click **uploading an existing file**.
5. Drag and drop the folders (`pomodoro/`, `dopamine-menu/`) and files (`preview.html`, `README.md`).
6. Click **Commit changes**.
7. Go to **Settings** &rarr; **Pages** (on the left menu).
8. Under **Branch**, select `main` (or `master`) and folder `/(root)`, then click **Save**.
9. Wait 1–2 minutes. GitHub will provide your live URL:
   ```text
   https://<your-username>.github.io/notion-widgets/pomodoro/
   https://<your-username>.github.io/notion-widgets/dopamine-menu/
   ```

### Option B: Netlify Drop (Zero Setup)
1. Go to [app.netlify.com/drop](https://app.netlify.com/drop).
2. Drag the entire `notion-widgets` folder onto the page.
3. You will instantly receive a live `https://...netlify.app` URL.

---

## 📌 Step 2: Embed into Notion

1. Open any page in **Notion**.
2. Type `/embed` and select the **Embed** block from the popup.
3. Paste the URL of the widget you want to display:
   - Example: `https://yourname.github.io/notion-widgets/pomodoro/`
4. Click **Embed link**.
5. **Resize**: Drag the left/right and bottom handles to fit your Notion layout.
   - *Sidebar column*: recommended width 280px–340px.
   - *Center dashboard*: recommended width 440px–520px.

> **Tip for Notion columns:** Drag the embed block next to an existing block to automatically place it in a neat side column!

---

## 🎨 Step 3: Customizing Colors & Aesthetic

Both widgets are written with standard CSS variables at the very top of each `index.html`. You can open `pomodoro/index.html` or `dopamine-menu/index.html` in any text editor (Notepad, VS Code, TextEdit) to tweak the colors:

```css
:root {
  --bg: #F8F3EA;             /* Warm cream background */
  --card-bg: #FFFFFF;        /* Stationery white card */
  --text: #4A3A30;           /* Rich espresso text */
  --clay: #C4886C;           /* Terracotta accent / primary button */
  --sage: #9DAA92;           /* Gentle sage green / progress ring */
  --sand: #D8B98F;           /* Sand paper shadow */
  --line: #DDD0C3;           /* Notebook border lines */
}
```

### Dark Mode
Both widgets automatically detect your system or Notion dark theme (`prefers-color-scheme: dark`). The dark mode palette is tailored for late-night calm:
- Deep chocolate slate: `#2F2620`
- Dark card background: `#3A2D25`
- Crisp soft text: `#F8F3EA`

---

## 🛠️ Technical Specifications & Guarantees

- **Zero Trackers / Zero Cookies**: Completely private. No user data leaves your computer.
- **ADHD-Friendly Motion**: Subdued micro-transitions (200–300ms) with zero flashing elements. Respects `prefers-reduced-motion`.
- **Driftless Timer Engine**: Instead of simple interval counters that slow down when you switch Notion tabs, the timer calculates differences against an absolute hardware timestamp (`Date.now()`).
- **Resilient Storage**: All `localStorage` calls are guarded with `try...catch` blocks to ensure the widget functions smoothly even inside strict iframe security policies.

---

## 💬 Support & Inquiries
If you have any questions, need custom color matching, or have feature ideas, feel free to reach out via Etsy Messages!
