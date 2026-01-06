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