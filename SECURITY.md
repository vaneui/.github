# Security policy

This policy covers every repository of the VaneUI organization: [`@vaneui/ui`](https://github.com/vaneui/vaneui), [`@vaneui/md`](https://github.com/vaneui/md), [`@vaneui/mcp`](https://github.com/vaneui/mcp) and the [vaneui.com](https://github.com/vaneui/web) site.

## Supported versions

Security fixes go into the latest release of the current major version of each package (1.x today). Older releases get no fixes, so the fix for a report is an upgrade to the newest version.

## Reporting a vulnerability

Please do not open a public issue for a security problem.

Send the report to **hello@vaneui.com** and include:

- the package and version, or the page of vaneui.com
- what an attacker can do, and what they need for it
- the smallest input or code that shows the problem

You get an answer within five working days. Once the problem is confirmed, the fix is released first and the report is credited in the release notes, unless you ask to stay unnamed.

## What counts

- Markup or script that gets through `@vaneui/md` when it renders untrusted Markdown, with or without `untrustedPreset`
- A component that renders a URL, an element name or HTML from a prop without the checks its documentation describes
- A way to make `@vaneui/mcp` read files outside its docs corpus
- A problem in the published packages themselves, such as a file that should not be in the tarball

A vulnerability in a dependency is in scope when it can be reached through a VaneUI package. Findings in development tooling alone (test runners, linters, build scripts) are welcome as regular issues.
