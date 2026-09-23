# Findings — MsPy-angular
Current open doc defects only. A finding is added here only after a human reviews and approves it; page failures in a run are never written here automatically. Resolved or superseded findings are removed (see git history).
Stack: `@copilotkit/angular` 0.5.2 (declared `^0.5.2`, latest) · `@copilotkit/web-inspector` 1.70.2 (undeclared, exact-pinned by angular).

## Quickstart (`/quickstart`, same text on landing page)

- ❌ **#1 Step 3 names an Inspector tab Angular can't install.**
  - Step 3: *"Open **Rich Threads**."* Steps 1-2 are Inspector tabs, so it reads as a tab.
  - web-inspector 1.70.2: tab is `label: "Threads"`; "Rich Threads" is only the launcher hover-menu row (`HUD_THREADS_LABEL = "Rich Threads"`). Rename is in web-inspector 1.73.1+, unreachable from Angular 0.5.2.
