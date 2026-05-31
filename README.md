# @bvc-lang/cli

CLI for the **BVC** (Basis · Vector · Goal) open format.

- **npm:** [`@bvc-lang/cli`](https://www.npmjs.com/package/@bvc-lang/cli)
- **Spec:** [`@bvc-lang/spec`](https://www.npmjs.com/package/@bvc-lang/spec)
- **Repo:** [bvc-lang/cli](https://github.com/bvc-lang/cli)

## Install

```bash
npm install -g @bvc-lang/cli
```

## Commands

```bash
bvc lint charter/main.bvc
bvc lint path/to/file.bvc

bvc format file.bvc --stdout        # canonical output to stdout
bvc format file.bvc --in-place      # overwrite input
bvc format file.bvc --out out.bvc
```

## Monorepo development

From Work Graph repo root:

```bash
npm run sync:bvc-cli-lib   # copy parser into packages/bvc-cli/lib
npm run bvc lint charter/main.bvc
npm run verify:bvc-cli-publish
```

Publish: see [PUBLISH.md](./PUBLISH.md).

## License

MIT
