# TypeScript + Node.js Project Boilerplate

TypeScript + Node.js project with modern tooling (March 2021) to get started quickly and right-footed. Ideal for quick projects as well as npm packages.

Batteries included:

* TypeScript 4, optionally [esbuild](https://esbuild.github.io/)
* Linting with [typescript-eslint](https://github.com/typescript-eslint/typescript-eslint) ([tslint](https://palantir.github.io/tslint/) is deprecated)
* Tests with [Jest](https://jestjs.io/docs/getting-started) (and [ts-jest](https://www.npmjs.com/package/ts-jest))
* CI for testing and linting ([GitHub Actions](https://docs.github.com/en/actions) / [Gitlab CI](https://docs.gitlab.com/ee/ci/))
* Automatic API documentation with [typedoc](https://typedoc.org/guides/doccomments/)

See also the [introduction blog post](https://www.metachris.com/2021/03/bootstrapping-a-typescript-node.js-project/).


## Getting Started

* Clone the repository (you can also click "Use this template")
* Edit `package.json` and `tsconfig.json` to your liking
* Now you can run `yarn run`, `yarn lint`, `yarn test`, `yarn build` and `yarn ts-node <filename>`.
* For publishing to npm, use `yarn publish` (or `npm publish`)

### Want documentation, published to GitHub or GitLab pages?

* Install [typedoc](https://typedoc.org/guides/doccomments/): `yarn add -D typedoc`
* Add `docs` script to `package.json`: `"docs": "typedoc --entryPoints src/main.ts"`
* Publish to pages through CI:
  * [GitHub pages](https://pages.github.com/): uncomment content of `.github/workflows/deploy-gh-pages.yml` and enable pages in GitHub repo settings
  * [GitLab pages](https://docs.gitlab.com/ee/user/project/pages/): uncomment deploy task in `.gitlab-ci.yml`

### Prefer to use esbuild?

You can use [esbuild](https://esbuild.github.io/) instead of the default TypeScript compiler (`tsc`) to build and bundle the output.
esbuild is an extremely fast bundler that supports a large part of the TypeScript syntax.

```bash
# Install esbuild
yarn add -D esbuild

# Compile and bundle (prints to stdout)
./node_modules/.bin/esbuild src/main.ts --bundle --platform=node --outfile=dist/out.js

# Run the bundled output
node dist/out.js
```

## References

* [TypeScript Handbook](https://www.typescriptlang.org/docs/handbook/intro.html)
* [tsconfig documentation](https://www.typescriptlang.org/tsconfig)
* [typescript-eslint documentation](https://github.com/typescript-eslint/typescript-eslint/blob/master/docs/getting-started/linting/README.md)
* [Jest documentation](https://jestjs.io/docs/getting-started)
* [GitHub Actions](https://docs.github.com/en/actions), [GitLab CI](https://docs.gitlab.com/ee/ci/)


## Feedback

Please post your feedback and/or ideas:

* [twitter.com/metachris](https://twitter.com/metachris)
* [Create a new issue](https://github.com/metachris/typescript-nodejs-boilerplate/issues)
