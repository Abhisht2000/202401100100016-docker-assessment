## Stage 3 — Trivy Security Assessment

### Before and After Comparison

| Metric | fest-backend:0.1 | fest-backend:0.2 |
|---|---|---|
| CRITICAL | ACTUAL_COUNT | ACTUAL_COUNT |
| HIGH | ACTUAL_COUNT | ACTUAL_COUNT |
| Image size | ACTUAL_SIZE | ACTUAL_SIZE |

### Security Improvements
- Changed the Python base image.
- Upgraded pinned Python dependencies.
- Configured the application to run as a non-root user.
- Saved Trivy reports before and after remediation.

### Security Gate
- Image: fest-backend:0.2
- Command exit code: ACTUAL_EXIT_CODE

- Result: PASS only if the exit code is 0.
