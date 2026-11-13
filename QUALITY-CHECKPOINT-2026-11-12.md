# PALMI-D3V — Public repository quality checkpoint (2026-11-12)

## Public repository inventory

The GitHub account currently exposes five public repositories:

1. palmid3v — profile and ecosystem documentation.
2. cupboard-palmid3v — multi-workspace inventory.
3. sandwichies-palmid3v — storefront and business operations.
4. dayflow-palmid3v — personal productivity.
5. financial-d3v-palmid3v — local-first personal finance.

Visibility is a point-in-time observation and should be rechecked before publishing future profile changes.

## Application CI summary

| Repository | Latest observed result | Evidence / action |
|---|---|---|
| Cupboard | Failed regression assertion: 18 passed, 1 failed | PR #11 updates the assertion to match the active-workspace implementation. |
| Sandwichies | Failed run with no reported job steps | Inconclusive for application code; rerun with an available runner. Keep order intake disabled. |
| DayFlow | 27 unit tests passed; 6 Firestore Rules tests failed because no emulator was started | PR #41 separates unit tests and runs Rules tests inside Firestore Emulator. |
| Financial-D3v | Go job passed; frontend tests failed on a Vite worker URL import under Node | PR #21 defers the Vite-specific import until PDF extraction. |

## Open corrective pull requests

- https://github.com/palmid3v/cupboard-palmid3v/pull/11
- https://github.com/palmid3v/dayflow-palmid3v/pull/41
- https://github.com/palmid3v/financial-d3v-palmid3v/pull/21

All three pull requests are open and their CI results must be reviewed before merging. No PR is described as merged or validated green in this checkpoint.

## Scope and limits

- This review covers the public repository inventory, READMEs, selected project context/roadmap files, package scripts, CI workflow definitions and available GitHub Actions evidence.
- It does not certify production deployments, live Firebase/Cloudflare configuration, data migrations, external security audits or device-level QA.
- Sandwichies order intake remains disabled. No production deployment, live order, real inventory mutation or paid resource was authorized by this review.
- Financial-D3v Personal and Business vaults remain independent; vault plaintext and .fdv files must not be sent to cloud services.
- Historical progress percentages are not recalculated from CI status. They remain estimates, not live telemetry.

## Next review sequence

1. Resolve the three open CI corrective pull requests.
2. Rerun Sandwichies CI and inspect the first real executed failing step, if any.
3. Review each repository's application code and test coverage for the next implementation-level improvements.
4. Reconcile the profile README's project descriptions with current implementation and visibility.
5. Update this checkpoint only when new evidence exists.
