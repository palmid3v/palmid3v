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
| Cupboard | Functional CI passed: regression 19/19, Firestore Rules 8/8, lint and build | [Latest run](https://github.com/palmid3v/cupboard-palmid3v/actions/runs/43360731865): security gate blocks on 25 full-tree findings; production-only 5 high + 1 critical. |
| Sandwichies | Full CI passed: 43 domain, 84 Worker, 12 Firestore Rules, 7 integration tests, build and smoke | [Latest run](https://github.com/palmid3v/sandwichies-palmid3v/actions/runs/43360656251): production audit 7 (1 low, 6 moderate), all with fixes available; no high/critical. Orders remain disabled. |
| DayFlow | CI passed: 27/27 unit/domain tests, 6/6 Firestore Rules tests, lint and build | [Latest run](https://github.com/palmid3v/dayflow-palmid3v/actions/runs/43360559200); PR #41 separates unit tests and runs Rules tests inside Firestore Emulator. |
| Financial-D3v | CI passed: 32/32 frontend tests; Go tests/build also passed | [Latest run](https://github.com/palmid3v/financial-d3v-palmid3v/actions/runs/43360567836); PR #21 defers the Vite-specific import until PDF extraction. |

## Open corrective pull requests

- https://github.com/palmid3v/cupboard-palmid3v/pull/11
- https://github.com/palmid3v/dayflow-palmid3v/pull/41
- https://github.com/palmid3v/financial-d3v-palmid3v/pull/21

All three corrective pull requests remain open. DayFlow and Financial-D3v have successful CI on their corrective commits; Cupboard needs another CI run after its second assertion correction. These changes are not merged.

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
