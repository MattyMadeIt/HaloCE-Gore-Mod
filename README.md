# Halo CE Gore Mod

A gore mod for Halo: Combat Evolved, for **Windows PC** and **Android**.
Enemies come apart — this is the build where a close explosion, a fast
vehicle hit or a point-blank shotgun doesn't just drop them.

Built on the OpenCE decompiled Halo CE engine (Xbox build). This repo is
builds only: grab a build from **Releases**, bring your own game files,
play.

## Downloads

Go to [Releases](../../releases) and download:

| File | Platform |
| --- | --- |
| `HaloCE-Gore-PC-Windows.zip` | Windows PC |
| `HaloCE-Gore-SBS-Android.apk` | Android (arm64, Android 9+) — also has SBS 3D stereo |

**No game data is included.** You need your own Halo: Combat Evolved
**Xbox disc image** (`.xiso` or `.iso`). On first start each build asks
for it and extracts the `maps/` folder itself (PC: next to the exe;
Android: into the app's data folder). Nothing copyrighted is distributed
here.

## What the mod does

On by default. **Toggle: Settings → Player Setup → (your profile) →
Video Setup → GRAPHICS → GORE** (saved, applies straight away).

- Enemies killed by a close explosion or a fast vehicle hit come apart
  into six pieces (head, arms, legs, torso), with blood bursts, drips
  and ground splats. Pieces land, bounce, rest, then fade.
- Point-blank shotgun kills gib (within about 2 metres).
- A killing sniper-rifle headshot takes the head only.
- Hunters gib **only** to a direct Scorpion tank shell hit.
- Works on enemies and on the player character.
- **Multiplayer (co-op and online/system link):** gore is on there too.
  Every player gibs the same kills on their own screen — the pieces are
  local eye-candy per machine and are never networked, so gore and
  non-gore players can play in the same game and nothing can desync.

## PC install

1. Unzip `HaloCE-Gore-PC-Windows.zip` anywhere.
2. Run `halo.exe` (keep `SDL3.dll` next to it). Standalone program — it
   is not a mod for retail Halo CE/MCC and replaces nothing.
3. First start: select your Xbox disc image when asked. After that,
   just run `halo.exe`.

Needs OpenGL 4.5 graphics. Full details are in `README-INSTALL.txt`
inside the zip; advanced gore options are in `config.toml` next to the
exe (created on first run). Note: this build can check for updated
engine builds at start-up — an updated vanilla build will not have the
gore, so keep this folder if you want it.

## Android install

1. Copy your Xbox disc image (`.xiso` or `.iso`) onto the phone.
2. Install `HaloCE-Gore-SBS-Android.apk` (sideload; 64-bit devices,
   Android 9 or later).
3. Start it and select the disc image when asked.

Touch controls and controllers both work, and gyro aim works alongside
a controller. Touch button opacity can go all the way to invisible.

**SBS 3D (Android):** side-by-side stereoscopic 3D for cardboard
viewers / SBS displays — Settings → Player Setup → (profile) →
Video Setup → **STEREO 3D (SBS)**, with **EYE DISTANCE** to match your
viewer (64 mm is average). Stereo turns itself off in local
split-screen (it needs one fullscreen view); in online/co-op play
everyone is fullscreen, so stereo and multiplayer gore work together.

## Credits

Built on the OpenCE decompiled engine. Engine licence files are
included in each download; this repo's own licence is in `LICENSE.md`.

Found a gore bug? Open an issue with the platform (PC/Android), the
weapon/enemy involved, and whether it was single player or multiplayer.
