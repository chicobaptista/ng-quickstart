# Ng-quickstart

This is a quickstart Angular project containing my preferred configurations and tools for frontend development, including linting, git hooks, ci/cd and testing frameworks, to be used as a launchpad for different Angular applications.

This project was generated with [Angular CLI](https://github.com/angular/angular-cli) version 13.3.3.


## Angular, NodeJS, Typescript and NPM/YARN

As an Angular project, this project is based on NodeJS/Typescript, and uses Yarn as a package manager.

## Git and commit style guides

This project uses conventional commits and commitzen to generate consistent commit messages and husky commit-msg hook and commitlint to enforce them.

## Code style and linting

This project leverages ES-Lint and Prettier to check and format code into the specified guidelines, and also uses lint-staged and a husky pre-commit hook to enforce linting rules.

## Testing

This project also tries to approach software development from a Test-Driven perspective. As such, automated unit, integration and e2e testing is incorporated into the development workflow from the very beginning. Husky pre-push hooks and github CI actions run unit and e2e testing respectively to ensure that all code integrated into the develop and main branches is functioning and covered by automated tests.

### Unit testing

The default Angular configuration is Karma running Jasmine tests. A modified karma-ci config file is used for test runs into the git workflow

### Integration and e2e testing

A cypress github workflow script is run on all pull-requests into the main and develop branches.