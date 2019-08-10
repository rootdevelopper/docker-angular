# A8Guide

This project was generated with [Angular CLI](https://github.com/angular/angular-cli) version 8.0.2.

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

Docker Commands:

    Build project on dev:
        From root directory:
            docker build -f Dockerfile.dev .
    
    On dev you can make changes to code and see your changes almost immediately.
        when running docker compose...
            volumes get mounted to keep node_files in container and sync the rest of the files

    Build project on prod:
        From root directory:
            docker build -f Dockerfile.prd .
    
    On prod Dockerfile execute a multi-step build, (build in node and served from nginx) server.
        when running docker compose...
            There is no volume mounting.
