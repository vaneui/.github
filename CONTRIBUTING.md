# Contributing to VaneUI

Thanks for helping. This guide applies to every repository of the organization. The component library has a longer guide of its own, with the architecture of the prop and theme system: [vaneui/CONTRIBUTING.md](https://github.com/vaneui/vaneui/blob/main/CONTRIBUTING.md).

## Report a bug or propose a change

- Open an issue in the repository of the package: [vaneui](https://github.com/vaneui/vaneui/issues) for components, [md](https://github.com/vaneui/md/issues) for Markdown rendering, [mcp](https://github.com/vaneui/mcp/issues) for the MCP server, [web](https://github.com/vaneui/web/issues) for vaneui.com and the docs.
- For a bug, the smallest JSX or Markdown that shows it helps most. The [playground](https://vaneui.com/playground) runs a snippet in the browser.
- For a new prop or component, describe the interface you would like to write before the implementation. Prop names follow the Tailwind class they stand for (`fontBold`, `itemsCenter`).
- A security problem goes through the [security policy](https://github.com/vaneui/.github/blob/main/SECURITY.md), not an issue.

## Work on a repository

All repositories use Node.js 24 and npm.

```bash
npm ci
npm test
npm run build
```

`vaneui` also has browser tests, `npm run test:e2e`, which matter for any change to styles or themes.

## Open a pull request

- Keep it to one change, and say what a user of the package will notice.
- Add or update tests for the behaviour you change. A bug fix comes with a test that fails without it.
- In `vaneui`, `md` and `mcp`, add a line to `CHANGELOG.md` under `Unreleased` when a user can notice the change.
- Leave the version number alone. Maintainers choose it at release time.
- Update the docs in [web](https://github.com/vaneui/web) when a prop, a default or a component changes.

Everyone taking part is expected to follow the [code of conduct](https://github.com/vaneui/.github/blob/main/CODE_OF_CONDUCT.md).
