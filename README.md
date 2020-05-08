# Angular Starter with US Web Design System (USWDS)

A quick Angular application starter to use [US Web Design System](https://designsystem.digital.gov/). This sample included the design system and
used the page template as an example. Please checkback later, for better integration and support for additional
components.

Checkout demo at https://github.com/softrams/uswds-angular-starter.

## Use this starter

You may use this as your Angular CLI project starter. Just clone and get started. Or see 'Setup' to add USWDS to a new Angular CLI project or
an existing Angluar CLI project.

```bash
git clone https://github.com/softrams/uswds-angular-starter my-app-name
cd my-app-name
npm install
ng serve
```

You may find and replace **"uswds-angular-starter"** with **"my-app-name"** to replace the project name.

## Use USWDS in a new or existing Angular CLI Project

Once Angular application is created, add the design system. Same steps work, even to add the design system
to an existing application

```bash
npm install --save uswds@latest
```

Now, update angular.json file to include css, js, fonts and img folders appropriately.

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
