# Sirv React Style Guide

## Table of contents

1. [Environment](#environment)
2. [Indents](#indents)
   1. [Functions](#functions)
   2. [Loops](#loops)
   3. [Conditions](#conditions)
3. [Names](#names)
   1. [Components](#components)
   2. [Props](#props)
   3. [State](#state)
   4. [Function and methods](#functions-and-methods)
   5. [Render functions](#render-functions)
   6. [Custom hooks](#custom-hooks)
4. [State management](#state-management)
5. [Requests to the server](#requests-to-the-server)
6. [i18n](#i18n)
7. [Unit tests](#unit-test)

## Environment

- Node.js: **14.x**
- Package manager: **yarn**
- Programming language: **TypeScript**

## Project structure
- The React app is located at `/sirv/frontend/app`, and its UIKit is located at `/sirv/frontend/uikit`.

## Functions

### Naming

- Use camelCase.
- The function and method names should be verb-based. The name should reflect an action.
- Do **not** use spaces between the function name and parentheses.
- Use the `handle` prefix for functions used as handlers.

## Language constructs and spaces
### Examples
Good:
```typescript
function handleAction() {}

const f = () => {}
```

Bad:
```typescript
function handleExample () {}

const f = ()=>{}
```


Good:
```typescript
while (condition) {}

for (let i = 0; i < 10; i++) {}
```

Bad:
```typescript
while(condition){}

for(let i = 0;i < 10;i++){}
```

### Conditions

Good:
```typescript
if (condition) {}
```

Bad:
```typescript
if(condition){}
```

## Naming

### Interfaces
- Use PascalCase.
- Do not use `I` as a prefix for interface names.

### Types
- Use PascalCase.
- Do not use `T` as a prefix for type names.

## Components
- Stick with functional components wherever it's possible. The arrow functions are preferred.

### Naming
- Use PascalCase for component names.
- The component names should be based on nouns, not verbs because they should reflect entities but not actions.
- Use **generic** names for **common** components only. For example, `Button` is a bad name for a component contained
  and used in a custom module. On the contrary, it is a good name for a UIKit component. Generic names, such as Users,
  Settings, or Usage, can also be used for the main components of custom modules.
- Use the `.tsx` extension for file names.

### Props
- Use camelCase for prop names.
- It's preferable to use `interface` for defining **props**.
- The interface (type) name should match the component name it's used for, plus the `Props` ending.
- Props used for callbacks should start with **on**. For example, `onClick`, `onClose`.

### State
- Use camelCase for state variables.
- Use `set` as a prefix for state setters. For example, if the state variable name is `username`, the setter for this state should
  be `setUsername`.

### Render functions
- Render functions can be used for rendering React elements.
- Render functions should return a React element or null.

### Tag id attribute
- Avoid hard-coding ids. The components can be re-used which might lead to id duplication. Use `useId()` if you need to generate an id.
- Use refs instead of ids wherever it's possible. 

## React sweet state

## Requests to the server
- Use Axios and useAxiosRequest for requests to the server.
- Track request state.

## Styles
- If a component requires custom styles, keep them in a separate file that has the same name as the component does with the `.scss` extension.
- Use kebab-case for class names sections.
- Use `__` to separate the class name sections responsible for blocks.
- Use `_` to separate the class name sections responsible for block(s) and a modifier

## i18n
### Buttons
- Button captions are contained in the `btn` object.
- Messages key pairs such as `run` / `runProg` can be used with the getBtnScope utility that returns a certain scope depending on the `inProgress` argument.

## lodash
- Do **not** import the entire lodash as `_`. Instead, import only the methods that will be used in your code.

## React, Angular, integration
- The standalone React app has all necessary providers (Auth, Config, Router, etc) on the top level of the app.
- Each feature of the React app should be located at `/frontend/app/src/modules/<module>`.
- Each feature module should have a wrapper component that will be used to integrate the module into the Angular app. The wrapper component should include providers used by the module because the Angular app doesn't use the React app's root component.
- Each integrated module replacing the module written in Angular should be integrated conditionally based on a feature flag.
