# Active Topics

Cross-session context tracker. Items here persist across chat sessions until resolved.

---

## Open
- **Generation review**: Review generation limits (per minute/hour/day by clinic) - not a priority for now - can be discussed after M11.
- **Credit consumption**: Review order for credit consumption. Paying users will be slowed down by free credits.
- **Force regen logging**: Validate we can track by clinic and how to use logging. Is that enough without tracking in Firestore?
- **Teeth overlay approach**: The current upper/lower arch is not fit for purpose as only one can be used at a given time and a rectangle is not the right shape to represent an arch. Further selection tools to be explored (ideally a brush/highlighter) - as well as ML custom for teeth (e.g. test https://github.com/thangngoc89/SegmentAnyTooth)
- **Post-MVP: Share for support** (from M10 plan): Allow users to explicitly share a low-rated output with the dev team for investigation. Requires explicit consent flow, controlled sharing (not automatic), no server-side image storage without consent, privacy-compliant data handling.
- **Post-MVP: Contact me flag** (from M10 plan): Optional checkbox on low ratings (e.g., score < 3) to indicate user wants follow-up. Requires consent/PII considerations, clear opt-in language, backend support for flagging and routing.  
- **BUG: Generation failed**: Generation failed first time. When retrying got message "already generated"
- **Gemini API endpoint location**: 2026-01-12 — TEMP: gemini_overlay uses global Generative Language API (no EU location control). Follow-up: restore EU-only Vertex routing when gemini-3-pro-image-preview (or equivalent quality) is available in EU Vertex regions with a supported request schema; re-enable fail-closed GEMINI_LOCATION.
- **Android emulator**: When it works again, test file download on API28 or less (see PR13 chat)
- **Gemini API**: investigate Vertex AI or new one from Max (partially done in PR21). After PR22 tooth masking: rerun locality tests with improved mask and stricter prompt “edit only masked pixels”; if still not great, evaluate alternative editors (OpenAI gpt-image, FLUX, etc.) under AC-13 posture.
- **Arch/Full mouth prompts**: Explore removing the mask and just ask all teeth or upper/lower arch - aim is to improve consistency of results.
- **Paid credit packages generation**: Besides free and pilot.
- **Review IAM + org policy alignment for Functions**: reconcile Domain Restricted Sharing (allowedPolicyMemberDomains) with public invoker (allUsers) usage; decide standard (public vs restricted), document in docs/DECISIONS.md, and audit all functions’ invoker bindings to remove drift (generateImages vs quoteGeneration).
- **Landscape UI**: Current experience very poor. To be redesigned.