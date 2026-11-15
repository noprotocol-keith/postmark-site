# POS-1054: the live Ballot Box (/votes/), before and after, on one INVENTED office answer

Before = a build of site `main` @ a314df5b3. After = PR #432's head d8a5adc1 (re-taken after the frontier mail fix and the lead FIX; same invented fixture).
Input: an invented GET /api/votes answer given through CDP Fetch (a Hearth-shaped open ballot with four designs, one at zero; a submissions ballot; a closed ballot; invented names and counts). NOT the real Hearth ballot, which Rei has not opened yet. No live office, proxy, key, sign-in or stake.
Headless Chrome 1x, device emulation (not a physical phone). *-states.json carry the text each page drew.
