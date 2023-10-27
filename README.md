<div align="center">
  <img src="./assets/logo.png" alt="fission Logo" width="100"></img>

  <h1 align="center">Fission JS Template</h1>

[![Built by FISSION](https://img.shields.io/badge/built_by-⌘_Fission-purple.svg)](https://fission.codes)
[![Discord](https://img.shields.io/discord/478735028319158273?logo=discord&color=mediumslateblue)](https://discord.gg/zAQBDEq)
[![Discourse users](<https://img.shields.io/discourse/users?server=https%3A%2F%2Ftalk.fission.codes&logo=discourse&label=talk&color=rgb(14%2C%20118%2C%20178)>)](https://talk.fission.codes)

</div>

## Usage (remove this section)

### Features

- Github workflows, templates, Code of Conduct, Contributing guidelines, Security Policy, Dependabot config, Codeowners and license.
- Dev container for Github Codespaces
- JS setup with ESLint, prettier, depcheck, typescript, typedoc, mocha and playwright-test.
- Documentation generated with typedoc and published with Github pages.
- Changelog, versioning and release management with [Release Please](https://github.com/googleapis/release-please).
- Optional pre-commit hooks with lint-staged and simple-git-hooks.
- VS Code settings and extensions.
- Examples and packages setup with pnpm workspaces.
- Codesandbox setup for examples.

### Instructions

- Add `GH_TOKEN` and `NPM_TOKEN` to secrets for CI workflows.
- Select _Github Actions_ for Github pages publishing. [Docs](https://docs.github.com/en/pages/getting-started-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site#publishing-with-a-custom-github-actions-workflow)
- You may need to change workflow permissions to read/write to be able to publish pages with github actions. Go to Settings > Actions > General > Workflow permissions.
- You should enable <https://socket.dev/> on the repo

#### Typescript

Override the `tsconfig.json` in the package with the following:

```json
{
  "compilerOptions": {
    "noEmit": true, // for apps or anything that is not published to npm
    "emitDeclarationOnly": true, // for TS with JSDocs
    "module": "NodeNext", // for TS packages
    "moduleResolution": "NodeNext" // for TS packages
  }
}
```

## Packages

- [package1](https://github.com/fission-codes/js-template/tree/master/packages/package1) - description
- [package2](https://github.com/fission-codes/js-template/tree/master/packages/package2) - description

## Examples

- [`demo`](https://github.com/fission-codes/js-template/tree/master/examples/demo) - description

### Checkout examples

You can use [Codesandbox](https://githubbox.com/fission-codes/js-template/tree/master/examples/demo) and start hacking right away.

To clone it locally:

```bash
npx tiged fission-codes/js-template/examples/demo demo
cd demo
pnpm install
pnpm dev
```

You can try any of the examples by replacing `demo` with the name of the example you want to try.

## Contributing

Read contributing guidelines [here](.github/CONTRIBUTING.md).

[![Open in GitHub Codespaces](https://github.com/codespaces/badge.svg)](https://codespaces.new/hd-template/examples)


## License

This project is licensed under either of

- Apache License, Version 2.0, ([LICENSE-APACHE](./LICENSE-APACHE) or
  [http://www.apache.org/licenses/LICENSE-2.0][apache])
- MIT license ([LICENSE-MIT](./LICENSE-MIT) or
  [http://opensource.org/licenses/MIT][mit])

at your option.

### Contribution

Unless you explicitly state otherwise, any contribution intentionally
submitted for inclusion in the work by you, as defined in the Apache-2.0
license, shall be dual licensed as above, without any additional terms or
conditions.

[apache]: https://www.apache.org/licenses/LICENSE-2.0
[mit]: http://opensource.org/licenses/MIT
