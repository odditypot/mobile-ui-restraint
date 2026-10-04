---
name: mobile-ui-restraint
description: Design and review mobile phone and iPad interfaces with task-first hierarchy, useful restraint, adaptive layouts, and accessible controls. Use for building, redesigning, or reviewing touch-first screens, responsive tablet layouts, navigation, forms, dashboards, or mobile web UI.
---

# Mobile UI restraint

Make the user's current task easy to understand and complete. Restraint is clear hierarchy, not hiding useful features or making every screen sparse.

## Design

1. Name the screen's job, the user's next decision, and the controls the task requires. Preserve the app's workflow and identity.
2. Place information by use:
   - Keep task context, frequent controls, and the next action in the working view.
   - Show specific consent, cost, privacy consequences, progress, and recovery beside the action they affect. Keep legally required disclosure accessible at that decision.
   - Put general help, privacy explanations, and full license or attribution text in Help, Settings, or About/Licenses.
   - Keep implementation notes, provider/runtime details, benchmarks, qualification gaps, synthetic-data disclaimers, and release-readiness notes in engineering docs or internal tracking. Surface only verified limitations that affect a user's choice, in concise language.
3. Write short, useful labels and instructions. Remove explanations of obvious actions, duplicate status, generic policy text, and repeated decoration. Do not move the same clutter into a card on another normal screen. Keep meaningful negative space; use no content quotas.
4. Design for the actual viewport. On phones, respect safe areas, touch reach, keyboard overlap, and scroll order. On iPad, adapt navigation to the current window; use sidebars or split views when useful, and preserve state while resizing. Support keyboard and pointer input where appropriate.
5. Cover loading, empty, error, offline, and confirmation states. Support Dynamic Type, VoiceOver, focus, sufficient contrast, and comfortable touch targets.

## Examples

- **Chat:** use the composer for drafting, attachment, voice, meaningful character/model or destination choices, and sending. Keep tutorial paragraphs and engineering/legal status out of the composer. Preserve the actual controls.
- **Voice, file, or model action:** keep microphone and attachment controls. Show unsupported-file errors at selection. A record screen is not a release readme: keep license claims, cache mechanics, test gaps, and benchmarks out of its normal task view. Before a download, show relevant size, destination, cost, and required consent; show progress while it runs. Do not state unverified terms or promise unimplemented features such as automatic language detection.
- **Task list or onboarding:** show meaningful task status and the next step. Put provider plumbing, test gaps, and benchmarks in engineering tracking; keep brief user instructions only where a step is unfamiliar.

## Review before delivery

- Inspect actual renders on a small phone and iPad at narrow and wide window sizes; exercise keyboard, scroll, resize, and one recovery state.
- For each visible item, ask: does it help the current task, explain a real consequence, or enable recovery? If not, remove it or place it in the appropriate settings, help, about, or engineering surface.
- Confirm clutter was not merely moved into another normal card; legal obligations and real cost/privacy consequences remain clear at the relevant decision; working controls remain available.
- Check text scaling, VoiceOver order, focus, contrast, target size, and localized copy. Finish when each viewport has a clear task hierarchy and usable controls/states.

## Platform references

Use platform units accurately: Apple recommends **44×44 pt** hit regions; Android recommends **48×48 dp** touch targets. WCAG 2.2 AA target minimum is **24×24 CSS px** with exceptions; AAA enhanced is **44×44 CSS px** with exceptions.

- [Apple: Principles of great design (WWDC26)](https://developer.apple.com/videos/play/wwdc2026/250/) — simplicity is not the same as minimalism.
- [Apple: Layout — iPadOS](https://developer.apple.com/design/human-interface-guidelines/layout#iPadOS) — adapt to window size.
- [Apple: Buttons](https://developer.apple.com/design/human-interface-guidelines/buttons) — 44×44 pt hit regions.
- [Android accessibility defaults](https://developer.android.com/develop/ui/compose/accessibility/api-defaults) — 48×48 dp targets.
- [WCAG 2.2 target size minimum](https://www.w3.org/WAI/WCAG22/Understanding/target-size-minimum) and [enhanced](https://www.w3.org/WAI/WCAG22/Understanding/target-size-enhanced).
