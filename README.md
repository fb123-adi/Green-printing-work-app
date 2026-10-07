# GPS Operations — Green Printing Solution

Mobile work-tracking app for Green Printing Solution Pvt Ltd. Covers tasks, blockers, approvals, production jobs, QC, end-of-day reports, announcements and Excel export. Available in English and Hindi, with dark and light themes.

> **Status: clickable prototype.** `index.html` runs entirely in the browser, and its data is stored only on the device that opens it. A backend (server + database + real authentication) is still needed before staff can use it with shared data. See `docs/HANDOFF.md`.

## Try it
Open `index.html`, or enable GitHub Pages (Settings → Pages → Branch: `main` / root). On an Android phone, open the Pages link and tap **Add to Home screen**.

Live demo: https://fb123-adi.github.io/Green-printing-work-app/

Demo logins (password `demo1234`):
- `GPS-E014`: Rahul Verma, Employee
- `GPS-H002`: Sunita Rawat, Head of Production (shows a 6-digit code on screen)
- `GPS-E030`: Farhan Ali, QC Inspector
- `pradkum3639`: Director (shows a 6-digit code on screen)

## Folders
- `index.html`: self-contained demo app
- `nocturne.css`: base styles and the Inter font that `index.html` loads (copy of `design/nocturne.css`)
- `design/`: editable design source files (open `design/GPS Operations Mobile.dc.html` to see every screen)
- `docs/HANDOFF.md`: full developer spec: roles, screens, state machine, data model, security, Excel export, design tokens

## Security notes
- Remove the demo accounts before production.
- This public copy contains no real password or password hash: the Director account uses the demo password here.
- In production the Director password must be set server-side with a strong hash, never stored in code. The password originally shared in a chat should be treated as compromised and not reused.
