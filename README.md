# GDG AITR Portal Review & Suggestions (Section A)

LIVE DEPLOYED LINK: https://gdg-portal-review.vercel.app/

A responsive, beginner-level audit page created for **Section A** of the GDG AITR task.

This project documents a genuine manual verification of the live GDG AITR website ([https://gdgocaitr.vercel.app/](https://gdgocaitr.vercel.app/)) tested across both desktop and mobile viewports.

---

## 📌 Sections Included (Strictly per Specification)

The audit page contains **ONLY** the 7 required sections:

1. **Title:** `"GDG AITR Portal Review & Suggestions"`
2. **Website Link:** Direct link to [https://gdgocaitr.vercel.app/](https://gdgocaitr.vercel.app/)
3. **"What I Checked":**
   - Broken links
   - Text alignment
   - Mobile layout
   - Visual glitches
4. **"Findings":**
   - Clearly separated by category with status badges (**"No major issue found"** vs. **"Issue found"**).
   - Covers HTTP verification of all 18 routes, mobile horizontal overflow (<420px), text clipping, visual glitches, and top navigation structure.
5. **"Suggestions":**
   - Actionable recommendations for mobile responsiveness, container padding, navigation links, and maps integration.
6. **"Desktop Review":**
   - Detailed observations on widescreen layout, branding, performance, and usability.
7. **"Mobile Review":**
   - Detailed observations on mobile behavior, viewport clipping below 420px, and hamburger menu accessibility.

---

## 🔍 Summary of Actual Verification Results

| Category | Status | Verified Observation |
| :--- | :--- | :--- |
| **Broken Links** | **No major issue found** | Tested 18 routes (`/announcements`, `/team`, `/about`, `/gallery`, `/contact`, `/events`, `/login`, etc.); all returned HTTP 200. Only minor detail: Contact location button uses `href="#"`. |
| **Mobile Layout** | **Issue found** | On phone viewports < 420px (e.g., iPhone SE 375px, iPhone 12/13/14 390px), the hero pill badge and header container cause horizontal overflow, pushing the mobile menu toggle off-screen. |
| **Text Alignment** | **Issue found** | Desktop text is properly centered and aligned. On mobile screens < 420px, headings and descriptions are clipped along the right margin due to container overflow. |
| **Visual Glitches** | **Issue found** | No glitches on desktop. On mobile (<420px), elements along the right edge are clipped. |
| **Navigation & Usability** | **Issue found** | "Events" is absent from the main desktop navigation bar. On mobile, the hamburger menu is hard to access when pushed off-screen. |

---

## 🚀 How to Run the Project

No setup, installation, or build tools are required!

### Option 1: Direct Browser Opening (Easiest)
1. Go to the project directory (`d:\antigravity`).
2. Double-click **`index.html`** to open it in Chrome, Edge, or Firefox.

### Option 2: Using VS Code Live Server
1. Open this folder in VS Code.
2. Right-click `index.html` and select **"Open with Live Server"**.

### Option 3: Using Python Local Server
Run in PowerShell:
```bash
python -m http.server 8000
```
Then open `http://localhost:8000` in your web browser.

---

## 📂 File Structure

```text
├── index.html    # Clean semantic HTML containing ONLY the 7 required sections
├── style.css     # Clean responsive CSS with clear comments and status badges
└── README.md     # Documentation and manual test report
```
