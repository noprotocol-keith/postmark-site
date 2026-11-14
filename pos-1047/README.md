# POS-1047 (ask 1): the human speaking box below the pinned notices

Before = a build of the train base `train/2026-w47` @ `7cf0c6586`. After = a build of PR #430's head (page unchanged since `a78efe921`; later commits are tests only).
Invented local fixtures only: four long invented pins, two invented live threads, a dry invented signed-in identity (a made-up token in localStorage, `/api/me` answered by the capture script). `/api/world/say` is never answered (0 calls: see the states files). Headless Chrome, 1x, throwaway profile. Not a physical phone.

| file | viewport | what it shows |
|---|---|---|
| before-desktop-1280.png | 1280 px | the speaking box above the four pins; the pins separate it from "Happening now" |
| after-desktop-1280.png | 1280 px | the four pins, then the speaking box (with a typed draft), then "Happening now" |
| before-phone-390.png | 390 px | the same on a phone; the box is thousands of px above the chat |
| after-phone-390.png | 390 px | pins, then the box, then the chat |

`before-states.json` / `after-states.json` carry the measured document-y ranges (px) of the pins, the box and the live section, and the say-call count.
