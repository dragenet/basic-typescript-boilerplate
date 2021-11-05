# Basic TypeScript Boilerplate for 2021

[![Build and test status](https://github.com/metachris/typescript-boilerplate/workflows/Lint%20and%20test/badge.svg)](https://github.com/metachris/typescript-boilerplate/actions?query=workflow%3A%22Build+and+test%22)

Simplified fork of [TypeScript project boilerplate created by metachris](https://github.com/metachris/typescript-boilerplate) with modern tooling, for Node.js programs and libraries. Get started quickly and right-footed 🚀

* [TypeScript 4](https://www.typescriptlang.org/)
* Linting with [typescript-eslint](https://github.com/typescript-eslint/typescript-eslint) ([tslint](https://palantir.github.io/tslint/) is deprecated)
* Testing with [Jest](https://jestjs.io/docs/getting-started) (and [ts-jest](https://www.npmjs.com/package/ts-jest))
* Automatic API documentation with [TypeDoc](https://typedoc.org/guides/doccomments/)
* [Nodemon](https://github.com/remy/nodemon) for development mode files change auto-reload

See also the introduction blog post: **[Starting a TypeScript Project in 2021](https://www.metachris.com/2021/03/bootstrapping-a-typescript-node.js-project/)**


## Getting Started

```bash
# Clone the repository (you can also click "Use this template")
git clone https://github.com/dragenet/basic-typescript-boilerplate.git your_project_name
cd your_project_name

# Edit `package.json` and `tsconfig.json` to your liking
...

# Install dependencies
yarn install

# Now you can run various yarn commands:

yarn lint
yarn clean
yarn docs
yarn build
yarn start
yarn dev
...
```

* Take a look at all the scripts in [`package.json`](https://github.com/metachris/typescript-boilerplate/blob/master/package.json)
* For publishing to npm, use `yarn publish` (or `npm publish`)

## Documentation, published with CI

You can auto-generate API documentation from the TyoeScript source files using [TypeDoc](https://typedoc.org/guides/doccomments/). The generated documentation can be published to GitHub / GitLab pages through the CI.

Generate the documentation, using `src/main.ts` as entrypoint (configured in package.json):

```bash
yarn docs
```

The resulting HTML is saved in `docs/`.

You can publish the documentation through CI:
* [GitHub pages](https://pages.github.com/): See [`.github/workflows/deploy-gh-pages.yml`](https://github.com/metachris/typescript-boilerplate/blob/master/.github/workflows/deploy-gh-pages.yml)
* [GitLab pages](https://docs.gitlab.com/ee/user/project/pages/): [`.gitlab-ci.yml`](https://github.com/metachris/typescript-boilerplate/blob/master/.gitlab-ci.yml)

This is the documentation for this boilerplate project: https://metachris.github.io/typescript-boilerplate/

## References

* **[Blog post: Starting a TypeScript Project in 2021](https://www.metachris.com/2021/03/bootstrapping-a-typescript-node.js-project/)**
* [TypeScript Handbook](https://www.typescriptlang.org/docs/handbook/intro.html)
* [tsconfig docs](https://www.typescriptlang.org/tsconfig)
* [typescript-eslint docs](https://github.com/typescript-eslint/typescript-eslint/blob/master/docs/getting-started/linting/README.md)
* [GitHub Actions](https://docs.github.com/en/actions), [GitLab CI](https://docs.gitlab.com/ee/ci/)


## Feedback

Reach out with feedback and ideas
[create a new issue](https://github.com/dragenet/typescript-boilerplate/issues)
