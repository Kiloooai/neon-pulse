# 🌟 Neon Pulse

*A rhythmic visualizer with glowing orbs pulsing to an invisible beat. Watch the rhythm unfold.*

---

## What is this?

An audiovisualizer without audio. Neon orbs pulse and emit expanding rings on a steady beat, creating a hypnotic, rhythmic display. The beat automatically plays (BPM adjustable). Click anywhere to emphasize a beat and spawn a big ring. Drag horizontally to adjust tempo in real time. Switch between time signatures (4/4, 3/4, 5/4, 7/4) for different feels. Choose visual modes: Rings (expanding circles), Waves (trail effects), Orbits (circular paths). It's a metronome made beautiful.

---

## Features

- **Auto-beat system** — orbs pulse on a steady tempo (60–180 BPM)
- **Interactive tempo control** — drag mouse horizontally to speed up/slow down
- **Multiple time signatures:** 4/4, 3/4, 5/4, 7/4 (click Mode button to cycle)
- **Visual modes:** Rings (expanding rings), Waves (trail effect), Orbits (circular paths)
- **Beat indicator** — pulsing circle in top-right shows current beat
- **Click-to-emphasize** — click anywhere to trigger a strong beat with special ring
- **Orb management** — orbs fade and are pruned automatically (max 50)
- **Color coding** — each beat in the measure gets a distinct neon color
- **Single HTML file** — no dependencies

---

## How to Use

1. Open `index.html`
2. Watch the orbs pulse to the beat
3. Click and drag left/right to adjust tempo
4. Click anywhere to add a big ring on that beat
5. Press **Mode** to cycle through time signatures (4/4, 3/4, 5/4, 7/4)
6. Press **Visual** to cycle through Rings / Waves / Orbits modes
7. Press **Clear** to remove all orbs
8. Just enjoy the rhythm

---

## Technical Notes

- Beat timing via `setTimeout` with tempo-based delay
- Each orb has: position, radius, color, pulse phase, trail
- Expanding rings stored separately; removed when alpha <= 0
- Tempo adjustment: `beatInterval = 60000 / tempo`
- Dragging updates tempo in real time, next beat uses new tempo
- Background cleared with alpha for motion blur effect
- Orb limit (50) prevents performance collapse

---

## The Real Story

I wanted to make something that *feels* rhythmic without actually needing sound. The pulsing orbs create a sense of tempo. The ability to drag to change tempo makes it interactive — you become the conductor. The different time signatures break the monotony. It's basically a screensaver that knows how to keep time.

Also: the color progression helps you feel where you are in the measure. Beat 1 = magenta, beat 2 = cyan, etc. It's secretly educational.

---

*Made with ✨ and some solid eighth-note energy during a heartbeat build cycle.*

**Repo:** https://github.com/Kiloooai/neon-pulse
