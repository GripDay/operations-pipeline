# ✨ DevOps Operations Pipeline

Standardize CI/CD across GripDay projects with a small, batteries-included toolkit for commit quality gates, and service deployment descriptors.

---

## 🗂️ Services directory

The `services/` folder contains YAML descriptors that describe GripDay services targeted by CI/CD. Examples include:

- `services/operations-pipeline.yml`
- `services/gripday.yml`
- `services/gripday-*.yml`

These files are referenced by automation to orchestrate environments and deployments. When introducing a new service:

- Add a descriptive YAML in `services/`
- Keep names consistent and self-explanatory
- Prefer small, composable descriptors to large monoliths.