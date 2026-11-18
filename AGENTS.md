# Contributor instructions

Use GitHub Issues for product work. Keep pull requests focused and verify the behavior the change affects. Build and test with synthetic data and scoped test credentials.

Keep deployment credentials, private infrastructure identifiers, and customer data out of source, fixtures, commit messages, and issue text. Scan the complete outgoing history before a public push.

Use the protected main branch through pull requests. An independent reviewer and the required checks must judge the current head. The allowlist in .github/merge-guard.toml defines ordinary changes automation may merge. A maintainer handles other changes. Release publication is a separate action.

Keep configuration documented as it changes. Preserve the API and tool contracts used by existing clients. Verify installable code from a clean environment outside the source tree.
