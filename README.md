# PetalNet/.github

Org-level config and shared tooling for PetalNet repos.

## Secret scanning

`.gitleaks.toml` — custom gitleaks ruleset covering PetalNet-specific patterns (internal IPs, Matrix MXIDs, known token prefixes). Extended from the default gitleaks ruleset.

### CI (GitHub Actions)

Copy `.github/workflows/secret-scan.yml` into any repo to get automatic scanning on every push and PR. The workflow pulls the shared config from this repo so pattern updates roll out everywhere automatically.

### Local pre-commit hook

Two options:

**Option A — shell hook (no deps):**

```
cp hooks/pre-commit .git/hooks/pre-commit
chmod +x .git/hooks/pre-commit
```

**Option B — pre-commit framework:**

```
pip install pre-commit
# copy .pre-commit-config.yaml into your repo root
# copy .gitleaks.toml into your repo root (or let CI fetch it)
pre-commit install
```
