# PoriKolpona with Professor Panda

This package integrates Professor Panda into the original PoriKolpona HSC study tracker while preserving the existing chapter, lecture, deadline, focus timer, theme, profile, and backup features.

## What's new

- Professor Panda welcome panel on the dashboard.
- Animated mascot dock available throughout the workspace.
- Contextual study tips, progress messages, focus encouragement, and celebration message.
- A small hidden star in Settings → Appearance reveals the nickname editor. The nickname is saved in this browser.
- Original mascot artwork and looping animated expressions are included in `assets/`.
- Responsive layout for desktop and mobile, with reduced-motion support inherited from the original app.

## Deploy

This is a static HTML/CSS/JavaScript app. Upload the complete `PoriKolpona_Professor_Panda` folder to Netlify, or drag the ZIP to Netlify Drop after extracting it if needed. Keep the `assets` folder alongside `index.html`, `script.js`, and `style.css`.

## Important data and authentication note

The preserved tracker currently stores study data in the browser's localStorage under `hsc-tracker-v1`. It does not yet use Supabase authentication or cloud synchronization. This package does not claim to implement student login, admin account provisioning, or cross-device sync. Those require the Supabase project URL/key and a secure account-provisioning design. Do not put a Supabase service-role key in frontend files.

Existing browser data remains in the same localStorage key when this version is opened on the same site origin. Export a backup from Settings before replacing an existing deployment.
