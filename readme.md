# Site Counts

A WordPress block showing counts of posts and taxonomies.

## Requirements

- WordPress 5.6+.
- PHP 7.3 or later, [Composer](https://getcomposer.org) and [Node.js](https://nodejs.org) for dependency management.

 [Homebrew](https://brew.sh) on MacOS:

	brew install php composer node

or [Chocolatey](https://chocolatey.org) for Windows:

	choco install php composer node nodejs

## Development

1. Clone the plugin repository.

2. Set up the development environment and tools using [Node.js](https://nodejs.org) and [Composer](https://getcomposer.org):

		npm install

	Note that both Node.js and PHP 7.3 or later are required on your computer for running the `npm` scripts.

### Scripts

`npm` as the canonical task runner for the project. Some of the PHP related scripts are defined in `composer.json`.

- `npm run build` to build the plugin JavaScript file. Use `npm run dev` to watch and re-build as you work.

- `npm run lint` to lint both PHP and JS files. Use `npm run lint:js` and `npm run lint:php` to lint JS and PHP separately.

- `npm run test` to run both PHP and JS tests without coverage reporting. Use `npm run test:js` and `npm run test:php` to run tests for JS and PHP seperately.

- `npm run test:coverage` to run both PHP and JS tests with coverage reporting.


## Continuous Integration

[GitHub Actions](https://github.com/features/actions) to lint all code, run tests and report test coverage to [Coveralls](https://coveralls.io) as defined in [`ci.yaml`](.github/workflows/ci.yaml).
