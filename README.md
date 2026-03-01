# DDP Yoga – Energy Routine Timer

A mobile-friendly workout timer for the DDP Yoga Energy routine. Built to be used on your phone while exercising — large text, audio countdown beeps, and voice announcements for each move.

## Features

- **54 exercises** covering the full Energy routine in sequence
- **Voice announcements** — speaks each move name out loud as it advances
- **Countdown beeps** at 3, 2, 1 seconds before each exercise ends
- **Customizable durations** — tap ⚙ to set a specific time for any exercise
- **Skip forward or back** at any time without stopping the timer
- **Section colors** to visually track where you are in the routine (Warm-Up, Standing, Balance, Power, Cool-Down, Floor, Finish)

## How to Use

1. Open the app in your phone browser
2. Tap **START** to begin
3. The timer counts down automatically and advances to the next exercise
4. Tap **›** to skip ahead, **‹** to go back
5. Tap **⚙** to adjust timing for any individual exercise

## Routine Sections

| Section | Color |
|---|---|
| Warm-Up | Orange |
| Standing | Amber |
| Balance | Teal |
| Power | Red |
| Cool-Down | Blue |
| Floor | Steel Blue |
| Finish | Gold |

## Notes

- Audio requires you to tap START at least once before beeps and voice will work (mobile browser requirement)
- Voice uses your phone's built-in text-to-speech — can be changed in your phone's accessibility settings
- All exercise timings default to 15 seconds and can be customized per-exercise via the ⚙ settings screen

## Built With

- React 18 (loaded from CDN — no build tools required)
- Web Audio API for countdown beeps
- Web Speech API for voice announcements
- Single self-contained `index.html` file
