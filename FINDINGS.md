# Findings — MsPy-angular

Doc defects / doc-vs-impl gaps. Moved from `readme.md` 2026-09-23; numbering unchanged.

## Known doc findings

- ❌ **Quickstart step 3 names an Inspector tab Angular can't install.**
  - Doc: Quickstart (and identical landing page), step 3: *"Open **Rich Threads**."* Steps 1-2 are Inspector tabs, so it reads as a tab.
  - Installed: `@copilotkit/web-inspector` 1.70.2 (undeclared; exact-pinned by `@copilotkit/angular` 0.5.2, declared `^0.5.2`, latest). Tab is `label: "Threads"`; "Rich Threads" is only the launcher hover-menu row (`HUD_THREADS_LABEL = "Rich Threads"`).
  - Tab renamed in web-inspector 1.73.1 (2026-09-22; latest 1.73.3), unreachable from Angular. Same at 1.70.1 / angular 0.5.1.
  - Evidence: package sources, 2026-09-23; no clip yet. Step quoted on `/quickstart`.

---
