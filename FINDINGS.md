# Findings — MsPy-angular
Current open doc defects only. A finding is added here only after a human reviews and approves it; page failures in a run are never written here automatically. Resolved or superseded findings are removed (see git history).
Stack: `@copilotkit/angular` 0.5.2 (declared `^0.5.2`, latest) · `@copilotkit/web-inspector` 1.70.2 (undeclared, exact-pinned by angular).
Major = blocks a reader (doesn't compile, crashes/throws, silently broken behaviour, step impossible to follow, missing required step/package, 404 target). Minor = one-line notes.

## Major

None open.

## Minor notes

- #1 Quickstart (`/quickstart`, same text on landing page): Step 3 says to open **Rich Threads**, but in web-inspector 1.70.2 the Inspector tab is named "Threads". "Rich Threads" is only the launcher hover-menu row (`HUD_THREADS_LABEL`). The tab was renamed in 1.73.1+, which Angular 0.5.2 can't install.
