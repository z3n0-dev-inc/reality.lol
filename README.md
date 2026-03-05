# VOID.BIO — guns.lol Killer 🔥

A guns.lol/fakecrime.bio alternative built from scratch. All premium features free.

## File Structure
```
voidbio/
├── index.html          ← Main profile page
├── customize.html      ← Customization dashboard
├── README.md
└── assets/             ← Put your media files here
    ├── background.mp4
    ├── hacker_background.mp4
    ├── rain_background.mp4
    ├── anime_background.mp4
    ├── car_background.mp4
    └── background_music.mp3
```

## Setup on GitHub Pages (Chromebook)

1. Create a new repo on GitHub (e.g. `void-bio`)
2. Upload ALL files keeping the folder structure
3. Go to repo Settings → Pages → Deploy from main branch
4. Your site will be live at `https://yourusername.github.io/void-bio`

## Customizing Your Profile

### Quick edit (edit index.html directly)
Find the `PROFILE` config object near the top of index.html's script section:

```javascript
const PROFILE = {
  name: "YOUR_NAME",
  bio: "your bio here",
  avatar: "URL or path to your avatar",
  socials: [
    { label: "Discord", href: "https://discord.gg/your-server", icon: "💬" },
    { label: "GitHub",  href: "https://github.com/yourusername", icon: "⬡" },
  ],
  badges: [
    { emoji: "⚡", tip: "Owner" },
    { emoji: "💎", tip: "Premium" },
  ],
  skills: [
    { name: "Python", pct: 87 },
    { name: "C++",    pct: 75 },
  ]
};
```

### Use the Customize Page (no code needed)
Open `customize.html` in your browser. All changes save to localStorage and apply on the profile page.

## Features

### FREE (everything is free)
- ✅ Custom avatar upload (animated GIFs supported)
- ✅ Custom background image/video upload
- ✅ 5 built-in video themes (Default, Hacker, Rain, Anime, Gold)
- ✅ Background filters (blur, brightness, saturation)
- ✅ Color overlay
- ✅ Full color theme customization + custom hex colors
- ✅ Font selection (Space Mono, Orbitron, Syne, Monospace, Serif)
- ✅ Card transparency, radius, glow intensity
- ✅ 3 layout options (Classic, Centered, Banner)
- ✅ 18 badge options to pick from
- ✅ 6 cursor effects (Default, Sparkle Trail, Matrix, Fire, Snow, Hearts)
- ✅ Page effects toggle (particles, scanlines, glitch, 3D tilt, orbit ring)
- ✅ Custom background music URL
- ✅ Social links editor (10 platform types)
- ✅ Skills & progress bars editor
- ✅ Name animation styles (typewriter, glitch, fade, wave, neon, matrix)
- ✅ Start screen customization
- ✅ Visitor counter
- ✅ 3D tilt card effect
- ✅ Particle background
- ✅ Custom cursor with trail

## Adding Your Videos

Place your video files in the `assets/` folder:
- `background.mp4` — default theme
- `hacker_background.mp4` — hacker theme
- `rain_background.mp4` — rain theme
- `anime_background.mp4` — anime theme
- `car_background.mp4` — gold theme
- `background_music.mp3` — default music

Videos won't play on GitHub Pages if they're too large (>25MB each).
Compress videos using HandBrake or ffmpeg before uploading.

## Tips

- Use animated GIF avatars for maximum drip
- Custom background uploads are stored in localStorage (browser only)
  - For persistent custom BGs on GitHub Pages, host the image somewhere (imgur, etc.) and use the URL
- The site works on mobile too
- Share your void.bio link anywhere

Built by JAQLIV. Inspired by guns.lol & fakecrime.bio — but better.
