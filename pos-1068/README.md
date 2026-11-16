# POS-1068: the public Coming up slot, before and after (desktop 1280, phone 390)

Before = a build of site `main` @ da00abb40 (no slot). After = PR #437's head 66fc5d13.
Input, both sides: the built /households/starforge/ page, signed out, with an INVENTED calendar given through CDP Fetch (four invented events: one hosted by a resident of the house, one the house's resident RSVP'd to, one unrelated, one cancelled; "someone-outside" is an invented RSVP). The house's residents are the page's own public handles; no real event, no live office or proxy read, no resident act, not production.
AFTER IS WITH AN INJECTED MARKER: no committed town design places <hearth-coming-up> yet (POS-1069, a later town PR, on purpose), so the after picture clones the built page's own <template data-hearth-slot-tpl="coming-up"> (the same component the preview uses) into the stage after the residents slot, then asks the page to repaint (pm:lens). Before has no slot, so the events are simply absent: that is the lost functionality.
Headless Chrome 1x emulation, not a physical phone. *-states.json carry what each page drew.
