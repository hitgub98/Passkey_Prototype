# Passkey-first login — clickable prototype

A click-through prototype demonstrating how passkey sign-in could work on the
pay.com.au business platform.

## What this prototype is for

The CEO asked us to **promote passkeys above the email/password fields** so
customers default to the more secure, lower-friction option. This prototype
takes the winning visual direction (subtle promote — passkey CTA sits above
the password form with equal visual weight and a short benefit line) and
shows the **full happy-path flow end-to-end** so stakeholders can experience
it, not just look at static screens.

## The flow you can click through

1. **Login screen** — the passkey CTA ("Sign in instantly with passkey") is
   the first thing the eye lands on, with a "Faster and safer than a password"
   microcopy line. The traditional email + password form sits below a divider
   as a fallback.
2. **Google Password Manager dialog** — tapping the passkey CTA opens the
   native browser/OS passkey prompt (modelled on Chrome's GPM dialog).
3. **Biometric verification** — the dialog auto-runs a Touch ID scan with a
   pulse + success animation.
4. **Signing-in bridge** — short loading state, "Welcome back, {name}…".
5. **Dashboard** — lands on the real pay.com.au dashboard layout with a
   green "Signed in with your passkey — no password required" confirmation
   banner at the top, so the security win is visible at the moment of
   payoff.

A small floating breadcrumb at the bottom of the screen shows where you are
in the flow and lets you restart the demo at any time.

## What you can tweak in the demo

The prototype has a Tweaks panel (top-right toggle) that lets reviewers:

- Change the demo account email and display name
- Swap the biometric label (Touch ID / Face ID / fingerprint) to test
  different device contexts
- Toggle whether the OS dialog auto-runs the scan
- Jump directly to any step in the flow

## How to deploy via GitHub Pages

1. Create a new **public** GitHub repo.
2. In the repo, click **Add file → Upload files** and drag both `index.html`
   and this README in. Commit.
3. Go to **Settings → Pages** in the left sidebar.
4. Under **Source**, choose **Deploy from a branch**, set **Branch: `main`**
   and **Folder: `/ (root)`**, then **Save**.
5. Wait ~30–60 seconds and refresh — your shareable URL will appear at the
   top of the Pages settings:
   `https://<your-username>.github.io/<repo-name>/`

To update: replace `index.html` in the repo and commit. Pages re-publishes
within a minute.

## Notes

- `index.html` is fully self-contained — all fonts, icons, scripts and
  images are inlined, so it works offline and on any static host.
- The page is a high-fidelity click-through, not a real authentication
  integration — passkey verification is simulated for demo purposes.
