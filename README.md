# Pacedall Breath

> Breathing tool for interviews, presentations, and stressful moments.

**Live URL:** breath.pacedall.com

## Features
- Three breathing modes: Before (4-7-8), During (Box 4-4-4-4), After (Wind-down 5-2-7)
- Sound on/off — visual-only mode for silent use during presentations
- Haptic pulse via device vibration
- Focus mode — full screen, distraction free
- Floating widget — draggable, resizable, stays over other browser tabs
- Picture-in-Picture — floats above ALL apps including Zoom, PowerPoint, Teams (Chrome/Edge)
- Session timer: 2, 5, 10 min or unlimited
- Zero backend, zero database, zero accounts

## Deployment (Cloudflare Pages via GitHub)

1. Push this folder to a GitHub repository
2. Log into Cloudflare Pages → Create a project → Connect to GitHub
3. Select your repo — build settings:
   - **Framework preset:** None
   - **Build command:** *(leave empty)*
   - **Build output directory:** `/` (root)
4. Deploy
5. In Cloudflare DNS, add a CNAME record:
   - **Name:** `breath`
   - **Target:** your Cloudflare Pages domain (e.g. `yourproject.pages.dev`)
   - **Proxy:** ✅ Enabled

Your app will be live at `breath.pacedall.com` within minutes.

## Keyboard Shortcuts
| Key | Action |
|-----|--------|
| Space | Start / Stop |
| F | Toggle Focus mode |
| W | Toggle Widget |
| P | Toggle Picture-in-Picture |

## Tech Stack
- Pure HTML / CSS / JavaScript — no frameworks, no dependencies
- Web Audio API (breathing tones)
- Browser Vibration API (haptic pulse)
- Picture-in-Picture API (always-on-top window)
- Canvas API (PiP rendering)

## Browser Support
| Feature | Chrome | Edge | Firefox | Safari |
|---------|--------|------|---------|--------|
| Core app | ✅ | ✅ | ✅ | ✅ |
| Picture-in-Picture | ✅ | ✅ | ✅ | ✅ |
| Haptic | ✅ Android | ✅ Android | ✅ Android | ❌ iOS |

---
Built by Pacedall.com — Small but Awesome.
