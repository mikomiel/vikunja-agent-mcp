# Contributing

Describe the behavior and how to reproduce it in a GitHub issue. Keep examples synthetic. Report vulnerabilities through the private channel in [SECURITY.md](SECURITY.md).

Open one focused pull request against main. Include the verification you ran. CI checks source, scans public content, and reviews dependencies. The required review status is tied to the pull request head. Changes to workflow policy, dependency manifests, scripts, and tests need a maintainer decision.

When changing the Python package, use the committed uv lockfile. Run `uv sync --frozen`, `uv run ruff check .`, `uv run pytest -q`, and `uv build`. For installation changes, install the built wheel outside the checkout and run the documented entry point. Use GitHub Issues for work beyond the pull request.
