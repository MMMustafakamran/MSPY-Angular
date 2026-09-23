# Findings — MsPy-angular

Doc defects and doc-vs-implementation discrepancies found by this harness.
Moved out of `readme.md` (Known doc findings) on 2026-09-23; numbering is unchanged.

## Known doc findings

- **Quickstart step 3 names an Inspector tab the installable Inspector does not
  have.** Since the 2026-09-23 sync, Quickstart (and the byte-identical landing
  page) says *"Open **Rich Threads**. The list is unlocked (Intelligence is on),
  or locked with Enable Intelligence (Intelligence is off)."* Steps 1 and 2 are
  tabs inside the Inspector (**Agents**, **AG-UI Events**), so step 3 reads as a
  third tab. In `@copilotkit/web-inspector` **1.70.2** (installed; not declared,
  exact-pinned by `@copilotkit/angular` 0.5.2, declared `^0.5.2`) that tab is
  labelled **Threads** (`label: "Threads"`). "Rich Threads" exists only as a row
  in the launcher hover menu that opens over the Inspector button
  (`HUD_THREADS_LABEL = "Rich Threads"`); clicking it opens the Inspector on the
  Threads tab. The tab itself was renamed to "Rich Threads" in web-inspector
  1.73.1 (published 2026-09-22; latest is 1.73.3), but `@copilotkit/angular`
  0.5.2, the latest release, pins 1.70.2, so an Angular reader cannot install
  the version the step describes. The same was true before this upgrade, at
  web-inspector 1.70.1 under `@copilotkit/angular` 0.5.1. Checked against the
  package sources on 2026-09-23, not yet in a clip. The harness quotes the step
  verbatim on `/quickstart`.

---
