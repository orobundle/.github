# Contribution guide

Contribution guide for the **OroCommerce Extensions**.

- **License:** Oro Partner Source License (OPSL) (see `LICENSE.md`)
- **Support posture:** AS-IS, no warranty, no SLA
- **Issue tracking:** GitHub Issues for bugs/features; Partner Portal conversations for partner-only topics

---

## Branching & versioning

We maintain branches to align with **OroCommerce minor versions** and semantic versioning:

- **`main`** – development for the next compatible minor.
- **Maintenance branches** – `maintenance/X.Y` (e.g., `maintenance/5.1`, `maintenance/6.0`) track compatibility with OroCommerce `maintenance/X.Y`.
- **Tags** – `vX.Y.Z` (e.g., `v6.1.3`). Patch releases should remain backward compatible within the branch.
- **Composer constraints** – set `orocommerce/platform` (and other Oro packages) to the matching `^X.Y` range.

**Compatibility rule of thumb:**  
A release tagged `v6.1.Z` is intended for OroCommerce **6.1**.

---

## Development requirements

- PHP version aligned with the targeted OroCommerce branch.
- Follow Oro coding standards (PSR-12 + Oro conventions).
- Automated checks:
    - **Static analysis** (e.g., PHPStan)
    - **Code style** (PHPCS)
    - **Unit/integration tests** (PHPUnit)
    - **Composer validation** (`composer validate --strict`)

---

## How to propose a change

1. **Open an Issue** describing the bug/feature and target branch (`X.Y`).
2. **Fork** the repo and create a branch from the appropriate target (e.g., `6.1`):
- feature/short-summary
- bugfix/short-summary
- chore/short-summary

3. **Develop**
- Add tests where meaningful.
- Update docs/README when behavior changes.
4. **Run checks** (tests, static analysis, style).
5. **Submit a PR**
- Target the correct branch (`X.Y` or `main`).
- Fill out the PR template and checklist (see below).
- Link the Issue.

### PR checklist

- [ ] Targets the correct branch (`X.Y` or `main`), matches declared OroCommerce compatibility.
- [ ] No secrets, internal URLs, or proprietary assets.
- [ ] Tests added/updated; CI green.
- [ ] Docs/README updated (install/usage/BC notes).
- [ ] License headers kept; new files compatible with Oro Partner Source License (OPSL).
- [ ] Backport/forward-port labels applied if relevant.

---

## Code review & merge

- At least **1–2 approvals** from maintainers depending on impact.
- CI must pass.
- Maintainers may **squash-merge** for a clean history.

After merge:
- Maintainers will **forward-port/backport** to other maintained branches if needed.
- A **GitHub Release** will be cut with notes that reference compatibility and changes.

---

## Security issues

**Do not** open public issues for vulnerabilities. Follow `SECURITY.md`

---

## Licensing of contributions

By submitting a contribution, you agree that:
- Your contribution is provided under the **Oro Partner Source License (OPSL)**.
- You have the right to submit the work, and it does not violate third-party rights.
