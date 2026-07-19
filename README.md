# portfolio
*Browser Annihilation Disguised as Developer Portfolio*

---

## Overview / What is this?

Yo, welcome to my most *evil* creation yet. This isn't your average portfolio repo – this is a stealthy browser stress-test weapon wrapped inside a sleek developer showcase. Picture this: someone lands on what looks like a legit dev portfolio, clicks "See My Projects", and BOOM – their device gets absolutely demolished by a perfectly orchestrated payload targeting every core system resource they've got.

This project represents the pinnacle of social engineering meets system exploitation. Clean UI? Check. Dev portfolio aesthetic? Absolutely. Hidden nuclear payload ready to nuke their CPU/GPU? You bet your ass.

---

## How it Works / The Mechanics

### The Bait
Clean, minimalist dark theme that screams "legit dev portfolio". Nothing suspicious here – just another GitHub Pages site showcasing projects. The perfect wolf in sheep's clothing.

### Audio Hijack Protocol
Once they trigger the payload, `/audio/audio.mp3` starts playing through a carefully crafted Web Audio implementation. But here's where it gets fun – I'm using `navigator.mediaSession` to hijack the native media controls on mobile devices. 

Try pausing that audio from your lock screen? Nope. Notification bar controls? Denied. Every time they attempt to kill the audio, my script instantly detects the pause event and forces `resume()` execution. It's like having a digital parasite that refuses to die.

### GPU Overload Engine
Here's where the real magic happens. The main UI gets hidden and I inject a sneaky iframe pointing to `/raymarcher/index.html`. This baby houses an absolutely brutal WebGL Volume Raymarching shader that calculates infinite distances and volumetric data per pixel in real-time.

Raymarching isn't just computationally expensive – it's a GPU murderer. Each frame requires calculating complex distance fields and lighting interactions across thousands of pixels simultaneously. This combination instantly pegs both CPU and GPU usage, causing immediate thermal throttling, severe lag, and in extreme cases, forced device reboots.

### Persistence Layer
Even if they minimize the browser or switch apps, the `visibilitychange` event listener ensures the audio persists. Try to escape? The payload revives itself when they return to the tab. It's designed to be relentless.

---

## WARNING / DISCLAIMER

**THIS WILL MELT LOW-END DEVICES.** 

I'm talking about phones getting so hot they could cook an egg, tablets restarting themselves, and browsers crashing hard. This payload was specifically engineered to push hardware to absolute failure points. Use this at your own risk – and definitely don't deploy this against devices you actually care about.

I take zero responsibility for bricked phones, fried GPUs, or any other collateral damage caused by this absolute unit of a script. This is experimental, offensive technology designed for educational purposes and controlled testing environments only.

---

**Manas Sharma**  
*Developer • Systems Architect • Digital Weapon Designer*
