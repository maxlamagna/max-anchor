# Active Topics

Cross-session context tracker. Items here persist across chat sessions until resolved.

---

## Open
- **Generation review**: Review generation limits (per minute/hour/day by clinic) - not a priority for now - can be discussed after M11.
- **Force regen logging**: Validate we can track by clinic and how to use logging. Is that enough without tracking in Firestore?
- **Subsequent case edit**: Currently a case only includes successful images and there is nothing further which can be done. Explore wheter it should include regeneration of failures, addition of new variants (new colours/materials), etc. - This is likely to become (one or more) extended ACs to be part of MVP (Milestone TBD)
- **Teeth overlay approach**: The current upper/lower arch is not fit for purpose as only one can be used at a given time and a rectangle is not the right shape to represent an arch. Further selection tools to be explored (ideally a brush/highlighter)?
- **BUG: Overlay ignored**: Enhanced images ignore the taps selected
- **New Req: Taps location**: Taps should only be accepted on teeth
- **Post-MVP: Share for support** (from M10 plan): Allow users to explicitly share a low-rated output with the dev team for investigation. Requires explicit consent flow, controlled sharing (not automatic), no server-side image storage without consent, privacy-compliant data handling.
- **Post-MVP: Contact me flag** (from M10 plan): Optional checkbox on low ratings (e.g., score < 3) to indicate user wants follow-up. Requires consent/PII considerations, clear opt-in language, backend support for flagging and routing.  
- **BUG: Previews download**: Previews can't be downloaded from the case view, even if the message shows success
- **BUG: Generation failed**: Generation failed first time. When retrying got message "already generated"
- **Gemini API endpoint location**: 2026-01-12 — TEMP: gemini_overlay uses global Generative Language API (no EU location control). Follow-up: restore EU-only Vertex routing when gemini-3-pro-image-preview (or equivalent quality) is available in EU Vertex regions with a supported request schema; re-enable fail-closed GEMINI_LOCATION.