# Welcome to the Sphinx Pipeline Sandbox
This workspace serves as a live, interactive reference dedicated to modern Python repository hygiene, automated documentation workflows, and robust Sphinx compilation pipelines. Instead of treating documentation as a static afterthought, these sandboxes will demonstrate how to treat technical manuals as a core engineering component that's fully integrated in your project, automatically tested, and bulletproof.

## The structure of this sandbox

```text
sphinx-pipeline-sandbox/
├── .github/                       # The front door of this organization.
│   └── profile/
│       └── README.md              # You are here.
│
├── sphinx-sandbox-code/           # Split repo - Component A (Python code).
│   └── codebase/
│       └── example.py             # Example Python module with reST docstrings.
│
├── sphinx-sandbox-docs/           # Split Repo - Component B (Sphinx pipeline)
│   ├── .github/workflows/ci.yml   # Advanced split-path CI pipeline.
│   └── build_local.sh             # Automated local Sphinx compilation script.
│
└── sphinx-sandbox-code-and-docs/  # Combined repository (unified monorepo).
    ├── .github/workflows/ci.yml   # Flat internal CI pipeline.
    ├── codebase/
    │   └── example.py             # Example Python module with reST docstrings.
    └── docs/
        └── build_local.sh         # Automated local Sphinx compilation script.
```

<!--
---

## 📂 Example Repositories

* **[sphinx-sandbox-code](https://github.com)**
  * This is a stand-alone Python-code module featuring reST-style docstrings that serves, here, as a pure, dependency-free compilation target (raw material).
* **[sphinx-sandbox-docs](https://github.com)**
  * This is a stand-alone Sphinx repository that acts as a decoupled pipeline to demonstrate how one would jump through cross-repository hoops by having to clone sibling environments, manage external paths, and handle separate documentation-release pipelines.
* **[sphinx-sandbox-combined-code-and-docs](https://github.com)**
  * This is a unified monorepo - an all-in-one repository framework that demonstrates atomic commits, simplified relative configurations, and internal path-routing.

---

## Demonstrated examples
* **Compatibility tests:** Local compatibility tests that use `tox` to ensure that your documentation passes the same checks used by the GitHub CI pipeline before pushing changes to the repository.
* **Continuous Integration workflows:** GitHub Actions configurations that compile docstrings and package distributions seamlessly on every commit.
* **Environmental verification guards:** Local bash-wrappers that validate the directory layout before triggering build systems.
* **Hyperlink linting:** Automated linting that dynamically hunts down and flags broken references or dead assets.
* **Simplified hyperlink auditing:** Unique configuration that simplifies the management of hyperlinks by allowing the use of plain-text URLs.

*Need an automated documentation-engine or pipeline tune-up for your project? Explore the examples, copy the scripts, or reach out to adapt these workflows to your code-base.*
-->
