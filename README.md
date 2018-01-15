# MyFirstAngularApp

This project was generated with [Angular CLI](https://github.com/angular/angular-cli) version 1.6.4.

## Development server

Run `ng serve` for a dev server. Navigate to `http://localhost:4200/`. The app will automatically reload if you change any of the source files.

## Code scaffolding

Run `ng generate component component-name` to generate a new component. You can also use `ng generate directive|pipe|service|class|guard|interface|enum|module`.

## Build

Run `ng build` to build the project. The build artifacts will be stored in the `dist/` directory. Use the `-prod` flag for a production build.

## Running unit tests

Run `ng test` to execute the unit tests via [Karma](https://karma-runner.github.io).

## Running end-to-end tests

Run `ng e2e` to execute the end-to-end tests via [Protractor](http://www.protractortest.org/).

## Further help
https://github.com/angular/angular-cli/wiki
To get more help on the Angular CLI use `ng help` or go check out the [Angular CLI README](https://github.com/angular/angular-cli/blob/master/README.md).
=======================================================================================================


Angular is a javascript framework which allows you to create reactive Single page Applications(SPAs).
===============================
CLI Deep Dive & Troubleshooting
==================================
Depending on the CLI version we are using we need to add
the FormsModule  to the imports[]  array in your app.module.ts

if we don't have Forms Module in imports[] in AppModule we need to add in import at the top of the file:


import { FormsModule } from '@angular/forms';

documentation: https://github.com/angular/angular-cli/wiki
---------------------------------------------------------

if we encounter issues during the installation of the CLI or setup of a new Angular Project we can solve it by using latest version of NodeJS, npm and CLI itself

nodejs.org and download the latest version. uninstall

and install

updating npm
run sudo npm install -g npm

updating the CLI
sudp npm uninstall -g angular-cli @angular/cli
npm cache clean
sudo npm install -g @angular/cli

You get an EADDR error (Address already in use)
ng serve --port anotherport


checking if window is running or not using ng serve
if display error  make sure using the latest version of the CLI



Project set up and First App:
-------------------------------

npm install -g @angular/cli
ng new my-dream-app
cd my-dream-app
ng serve
------------------------------

=============================
run browser:
http://localhost:4200/


Installing bootstrap:
---------------------
$ npm install --save bootstrap
restart server with ng serve

we can check in browser with elements section inside head

Important: For Two-Way-Binding to work, you need to enable the ngModel  directive. This is done by adding the FormsModule  to the imports[]  array in the AppModule.

You then also need to add the import from @angular/forms  in the app.module.ts file:

import { FormsModule } from '@angular/forms'; 
