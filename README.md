# VibeFit Workout Timer

A mobile-friendly workout timer for various popular exercise routines. Inspired by the DDP Yoga Energy routine. Built for use on your phone while exercising — large high-contrast text, audio countdown beeps, and voice announcements for each move.

## Features

- **74 exercises** across 8 sections covering the full Energy routine
- **Voice announcements** — speaks each move name out loud as it advances
- **Countdown beeps** at 3, 2, 1 seconds before each exercise ends
- **Per-exercise cues** — coaching notes displayed under the move name
- **Customizable durations** — tap ⚙ to set a specific time for any exercise
- **Time remaining** — live countdown showing total workout time left, updates dynamically when exercises are skipped
- **Skip forward or back** at any time without stopping the timer
- **Screen stay-awake** — uses the Wake Lock API to keep your phone screen on while the timer is running
- **Section colors** to visually track where you are in the routine

## Routine Sections

| Section | Exercises | Color |
|---|---|---|
| Warm-Up | 7 | Orange |
| Ignition | 9 | Amber |
| Balance | 24 | Teal |
| Break | 2 | Gray |
| Power | 6 | Red |
| Floor | 11 | Steel Blue |
| Going Home | 10 | Light Blue |
| Finish | 5 | Gold |

## How to Use

1. Open the app at [warhorse34.github.io/ddp-yoga](https://warhorse34.github.io/ddp-yoga)
2. Tap **START** to begin — this also activates audio and screen wake lock
3. The timer counts down automatically and advances to the next exercise
4. Tap **›** to skip ahead, **‹** to go back
5. Tap **⚙** to adjust the duration of any individual exercise for the current session

## Notes

- Audio (beeps + voice) requires tapping START at least once — this is a mobile browser requirement
- Voice uses your phone's built-in text-to-speech voice, changeable in your phone's accessibility settings
- Screen wake lock requires HTTPS — works on the GitHub Pages URL, not from a local file
- Wake Lock is supported on Chrome for Android and Safari 16.4+

## Updating the Routine

Timings and exercise names are managed via a spreadsheet (`DDP_Yoga_Durations.xlsx`). To update:

1. Edit the spreadsheet
2. Upload it to Claude and ask it to regenerate `index.html`
3. Replace the `index.html` file in this repository

## Built With

- React 18 (loaded from CDN — no build tools required)
- Web Audio API for countdown beeps
- Web Speech API for voice announcements
- Wake Lock API for screen stay-awake
- Single self-contained `index.html` file
