# Network Detector

Network Detector is a small React demo that reports browser online/offline state and when the most recent state change occurred.

## Core features

- Reads the initial connection state from `navigator.onLine`.
- Reacts to browser `online` and `offline` events.
- Shows a different Lottie animation for each state.
- Displays the timestamp of the latest detected state.
- Emits toast notifications when connectivity changes.

## Technology stack

- React 18
- Vite 5 with the React SWC plugin
- JavaScript/JSX and Tailwind CSS 3
- Lottie animations and React Toastify

## Prerequisites

- Node.js compatible with the locked dependencies
- npm
- A modern browser

## Local setup

```bash
git clone https://github.com/varunisrani/Network-detector--.git
cd Network-detector--
npm ci
npm run dev
```

Build and inspect the production bundle with:

```bash
npm run build
npm run preview
```

Lint the project with `npm run lint`.

## Configuration

No environment variables are referenced by the current application.

## Project structure

- `src/main.jsx` — renders the network-status interface
- `src/Network.jsx` — status card, animations, and notifications
- `src/useNetworkStatus.jsx` — browser event subscription and timestamp state
- `src/Online.json` and `src/Offline.json` — Lottie animation data
- `src/index.css` — Tailwind layers and global styles

## Status and limitations

This demo reports the browser's connectivity hint, not verified internet reachability, latency, bandwidth, or network diagnostics. Browsers can report `online` even when an external service is unreachable.
