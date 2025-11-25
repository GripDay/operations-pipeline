# ✨ DevOps Operations Pipeline

Centralized repository for GripDay's CI/CD infrastructure. Contains Drone CI pipeline definitions for automated testing, building, containerization, and deployment to staging environments. Each service pipeline includes code verification, artifact publishing, and Helm-based Kubernetes deployments with Slack notifications.

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
