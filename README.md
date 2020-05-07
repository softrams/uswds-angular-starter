# Angular Starter with USWDS Design System

A quick Angular application starter to use [USWDS Design System](https://designsystem.digital.gov/). This sample included the design system and
used the page template as an example. Please checkback later, for better integration and support for additional
components.

## Setup

Once Angular application is created, add the design system. Same steps work, even to add the design system
to an existing application

```bash
npm install --save uswds@latest
```

Now, update angular.json file to include css, js, fonts and img folders appropriately

```json
            "assets": [
              "src/favicon.ico",
              "src/assets",
              {
                "glob": "*",
                "input": "node_modules/uswds/dist/fonts",
                "output": "assets/fonts/"
              },
              {
                "glob": "*",
                "input": "node_modules/uswds/dist/img",
                "output": "assets/img/"
              }
            ],
            "styles": [
              "node_modules/uswds/dist/css/uswds.min.css",
              "src/styles.css"
            ],
            "scripts": ["node_modules/uswds/dist/js/uswds.min.js"]
```

## Development server

Run `ng serve` for a dev server. Navigate to `http://localhost:4200/`. The app will automatically reload if you change any of the source files.

## Code scaffolding

Run `ng generate component component-name` to generate a new component. You can also use `ng generate directive|pipe|service|class|guard|interface|enum|module`.

## Build

Run `ng build` to build the project. The build artifacts will be stored in the `dist/` directory. Use the `--prod` flag for a production build.

## Running unit tests

Run `ng test` to execute the unit tests via [Karma](https://karma-runner.github.io).

## Running end-to-end tests

Run `ng e2e` to execute the end-to-end tests via [Protractor](http://www.protractortest.org/).

## Further help

To get more help on the Angular CLI use `ng help` or go check out the [Angular CLI README](https://github.com/angular/angular-cli/blob/master/README.md).
