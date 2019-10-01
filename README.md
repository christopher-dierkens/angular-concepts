# Angular Concepts
Notes on Angular concepts

## Core
Place to put single use items. toast component, navbar component, dialog component, spinner-overlay component

## Ensure Module Loads only once
Useful to guard against core interceptors, pipes, transforms, etc are only loaded in one module.

[example guard](https://github.com/DanWahlin/Angular-JumpStart/blob/master/src/app/core/ensure-module-loaded-once.guard.ts)

# General
* Use a module for anything reusable, or self contained and not constrained by businiess logic.

* Use value types where possible when passing down to presentational components.

Q: What extensions are there for syntax errors and highlighting in VSCode?

Q: Could you freeze input's to components or some form of pure component?

# Component Libraries

`ng generate library {component-lib}`
`ng build {component-lib}`

Q: Can this be managed in a mono repo instead of NPM publish?

Q: Are there any implications for leaving empty ngOnInity hooks?

Q: What should go in a component constructor vs ngOnInit?

Q: When is it appropriate to use @ViewChild? 

# Top level modules
## Root Module
  Imports the 4 modules below
## Feature Module
  No need to export
## Routing Module
  Export the route
## Core Module
  Export single use components, only imported into app module
## Shared Module
  Exports sharable components
  Imports any shared component library
  
# RxJS

* Use the .asObservable when returning a Subject to protect against changes to the Subject

  
