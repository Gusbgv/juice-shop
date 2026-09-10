# ZAP Rule Exception: 10038

**Rule ID:** 10038
**Alert:** Content Security Policy (CSP) Header Not Set
**URL scope:** http://127.0.0.1:3000 (all paths, systemic)
**Evidence:** ZAP baseline run https://github.com/Gusbgv/juice-shop/actions/runs/34400132514; finding register, Step E2 of lab evidence package
**Owner:** Gustavo Garcia-Vargas
**Approver:** Course instructor, CPS-5981 (Dr. Ora Kenneth Melie), per lab submission review
**Compensating control:** Target is the upstream OWASP Juice Shop training image, scanned only inside an ephemeral GitHub Actions runner with no persistent deployment, no real user data, and no exposure outside the CI job's lifetime. The app is intentionally vulnerable by design for security-education purposes, so patching this header would defeat the training target's purpose rather than reduce real risk.
**Expiration:** End of current academic term; must be re-reviewed before any reuse of this pipeline against a non-training target.
