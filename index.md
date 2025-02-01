author: JJ & KK & NB
summary: Frontend onboarding
id: index
tags: Frontend, Vue
categories:
environments: Vue
status: Draft
feedback link: https://github.com/SolaceDev/solace-dev-codelabs/blob/master/markdown/android-test

# Wiselab Onboarding Frontend

## Overview

#### First of all, welcome to **Wisemen!** We are happy to have you here and we hope you will have a great time working with us.

<img width="200" src="img/projectSetup/Wisemen_Logo_Acid.png">

In this onboarding you will learn how frontend development happens at Wisemen.
You will learn how we use Vue, Vite, Tailwind, Figma, Github, Linear and more to our advantage.

For all our new projects we use a self made template together with our vue-core library.
This template consists of all the things we need to get started quickly and don't have to reinvent the wheel every time we start a new project.
The vue-core library is a component library that contain the most common components and composables that we use in our projects.
It is important to know that they are both a work in progress and we try to improve them every day.

This onboarding is designed to be completed in roughly 3-4 days.
This does not mean you have to complete it in 3-4 days. 
People with more experience will be able to complete it faster than people with less experience.

In this codelab we are going to create a simple to-do app.
This app will be used as example to teach you how we structure our projects, which tools and libraries we use.

> aside positive
> Important to know is that the template will do a lot of work for you.
> We definitely recommend that you try and understand what the template does and how it works.
> No you don't need to know everything, but it will help you to understand the project structure and the way we work.

We also expect you to make pull request of your work so your buddy can review your code and keep track of your progress.
The way we do this will be explained in the onboarding.

Good luck on becoming the front-end developer you are meant to be!
And remember, asking questions is always a good thing!

![](img/programmer.gif)

## Prerequisites

### IDE

There are 2 different IDE's you can use to work with Vue. You can use either **Visual Studio Code** or **WebStorm**. The Choice is yours, so choose wisely.

#### WebStorm

WebStorm is a JavaScript IDE with complete set of tools for client-side and server-side development and testing.
It provides code completion, on-the-fly error detection, powerful navigation and refactoring for JavaScript, TypeScript,
CSS, HTML and more.

Webstorm is a paid IDE. You can get a license from Wisemen. Ask your buddy!

[Download WebStorm](https://www.jetbrains.com/webstorm/download)

Handy Plugins:
- **Atom Material Icons** (cool file and folder icons)
- **GitHub CoPilot** (AI pair programmer)
- **Easy i18n** (i18n support in WebStorm)
- **IntelliVue** (Vue.js support for WebStorm)


#### Visual Studio Code

Visual Studio Code is a source-code editor developed by Microsoft for Windows, Linux and macOS.
It includes support for debugging, syntax highlighting, intelligent code completion, snippets, and code refactoring.

Visual Studio Code is a free IDE. You can download it from the website.

[Download vscode](https://code.visualstudio.com/download)

Handy Plugins:
- **Volar** (processing vue files)
- **ESLint** (code formatting)
- **Error lens** (showing errors in the code)
- **Guthub Copilot** (AI pair programmer)
- **I18n ally** (i18n support in vscode, managing translations)
- **Pretty Typescript Errors** (formatting ts errors so they are more readable)
- **Tailwind CSS intellisense** (tailwind css support)
- **VSCode-icons** (cool file and folder icons)
- **TODO tree** (showing all the TODO's in the project)
- **Vitest** (running tests)
- **GitLens** (git support)

Choose the IDE you want to work with and download it.

### Node.js

Node.js is an open-source, cross-platform, back-end JavaScript runtime environment
that runs on the V8 engine and executes JavaScript code outside a web browser.

Node.js is necessary to run the Vue project. You can download it from the website.

[Download Node.js](https://nodejs.org/en/download/)

### NPM vs PNPM

* [NPM](https://www.npmjs.com/get-npm)
  NPM is the default package manager for the JavaScript runtime environment Node.js. The NPM program is installed on
  Node.js when you install it from its website.

* [PNPM](https://pnpm.io/installation)
  PNPM is a fast, disk space efficient package manager. 
* It is designed to be installed globally, and it installs all the packages that you need in your project in a single place, using symlinks.

The difference between NPM and PNPM is that PNPM uses symlinks to link packages to your project. 
This means that if you have multiple projects that use the same package, it will only be installed once on your computer. 
This saves a lot of disk space. PNPM is also faster than NPM because it uses symlinks.

> aside positive
> We use PNPM in our projects.

### Our template

This is a good time to take a quick look at our template. You can find it here: [vue template](https://github.com/wisemen-digital/vue-project-template).
Take a quick look around to get familiar with the structure of the project. Ask your buddy if you have any questions. But don't worry, we will go through it in this onboarding.

### Figma

Our designers work with **Figma**.
Figma is a vector graphics editor and prototyping tool which is browser-based or can be installed on macOS or Windows.
We recommend you to install the desktop app.

[Download Figma](https://www.figma.com/downloads/)

Take a look around in Figma and try to get familiar with the tool. You will be using it a lot in the future.
You can view all of our designs here:

[Wisemen Figma](https://www.figma.com/files/team/1070403287155222588/Wisemen?fuid=1070747045190465434)

To access the designs you need to log in with your Wisemen account: 
[wireframes](https://www.figma.com/file/hebgv4Qx8VanMAQkO1NFpa/Onboarding-to-do?node-id=407-4095&t=2qdyy89lKwN7dFw3-0)

### Source control

#### GitHub

GitHub is a web-based version control repository hosting service owned by Microsoft, for source code and development
projects that use the Git revision control system.

Our projects will be hosted on GitHub.

If you are not yet familiar with GitHub, Here is great article to get you started:
[GitHub Git tutorial](https://docs.github.com/en/get-started/start-your-journey/hello-world)

We expect you to make pull request of your work so your buddy can review your code and keep
track of your progress.

> aside positive
> We switched to GitHub for our new projects. 
> You can find our GitHub organization here: [Wisemen GitHub](https://github.com/wisemen-digital)

### Linear access

For this onboarding you will be working with Linear to track your progress. You can find the Linear board here:
[Linear Todo]()

Linear is used to track the progress of your project and manage the tasks that need to be done.
All the requirements for the to-do app are in the Linear. You will be creating tasks in the Linear to keep track of your progress.

The Linear contains all the requirements for creating the to-do app.

*ToDo: Add link to Linear*

> A little tip: You can copy you're branch name from the linear ticket by using the command .
>`cmd + shift + .` on the ticket and then paste it in your terminal.

## Project explanation

You will be creating a simple to-do app. The app can be used to create, edit and delete to-do's.
The backend is already created and you can find the documentation here:

[Backend documentation](https://onboarding-todo-api.development.appwi.se/api/v1/docs/)

Username: `appwise`  
Password: `password`

For ease of use we are going to mock the backend in this project. so you don't have to worry about it.
You can still use the backend documentation to see how the backend works.
This won't change anything in the way you work with the project. (Ask your buddy to setup op Mock Service Worker with you!)

### Requirements

- Login page with email and password
- View your to-do's in a list
- Create a new to-do
- Edit a to-do
- Delete a to-do
- Mark a to-do as done

### Designs

The designs for the to-do app can be found in Figma. Login with your Wisemen google account to view the designs.
You can find the designs here:

[Figma designs](https://www.figma.com/file/hebgv4Qx8VanMAQkO1NFpa/Onboarding-to-do?type=design&node-id=467-4945&mode=design&t=c2mb4igTcdZQaH6X-4)

## Project setup

<img width="300" src="img/projectSetup/cat_i_am_ready.gif">

### 1. Vue 3 Project template

We use the latest version of Vue in our template. Vue3 is the latest version and has some new features and
improvements over Vue2. You can read more about Vue3 here: [Vue3 website](https://vuejs.org/)

First of all open the project template in GitHub and click on the `Use this template` button to create a new repository.
Make your own repository and clone it to your local machine. Open the project in your editor and install the dependencies with `pnpm install`.
Than run the project using `pnpm dev`.

Github Template link: [Vue project template](https://github.com/wisemen-digital/vue-project-template)

You will be greeted with a login page that is already there for you. You should be able to log in with your Wisemen email.
Take a look around and try to understand the project structure.

---

### 2. Vite

Vite is a new breed of frontend build tool that significantly improves the frontend development experience. It consists
of two major parts:

- A dev server that provides rich feature enhancements over native ES modules, for example extremely fast Hot Module
  Replacement (HMR) that updates your changes in the browser in as little as 16 milliseconds.
- A build command that bundles your code with Rollup, pre-configured to output highly optimized static assets for
  production.

This is configured in the template and you don't have to worry about it. But it's good to know what it is and how it works.

#### 2.2 Plugins

Vite supports a plugin system that allows you to customize the behavior of Vite itself and integrate with other tools.
Plugins can be configured in the `vite.config.js` file.

<img width="120" src="img/projectSetup/pnpm_logo.svg">
<img width="80" src="img/projectSetup/vs_icon.png">
<img width="140" src="img/projectSetup/npm_logo.png">

### 3. Package.json

The package.json file is used to give information to pnpm that allows it to identify the project as well as handle the
project's dependencies. pnpm can install the packages you specify in your package.json file.
The main use of the package.json file is to list the packages that your project depends on and to ensure that your
colleagues get the same packages when they do `pnpm install`.

#### 3.1 Scripts

The scripts property is used to specify a list of scripts that can be run using `npm run <script-name>`.
It's written as a JSON object where each key is the name of a script and the value is the command to run for.
Most common scripts are `start` and `build`.

#### 3.2 Dependencies vs Dev Dependencies

Dev dependencies are dependencies that are only used during development and are not required for production.
Dependencies are required for production.

<img width="120" src="img/projectSetup/tailwind_logo.png">

### 4. Tailwind CSS

Tailwind CSS is a utility-first CSS framework for rapidly building custom user interfaces. It's completely
customizable, completely extensible, and amazingly feature-rich.

#### 4.1 Tailwind config

Tailwinds config file is used to configure the framework. You can add custom colors, fonts, breakpoints and more.
This is where you can customize the framework to your needs.

👉 [Tailwind website](https://tailwindcss.com/)

<img width="120" src="img/projectSetup/ESLint_logo.png">

### 5. ESLint config

ESLint is a tool for identifying and reporting on patterns found in ECMAScript/JavaScript code, with the goal of
making code more consistent and avoiding bugs. Is helps a lot with code formatting and makes it easier to write code.
Also in team projects it helps to keep the code consistent.

> aside positive
> We use our own ESLint config in our projects. and it is already available in the template.

<img width="120" src="img/projectSetup/vue_i18n_logo.svg">

### 6. Internationalization (i18n)

i18n is a short name for internationalization. It is a process of designing and developing a software application so
that it can be adapted to various languages and regions without engineering changes.

Within the company we use [Vue i18n](https://vue-i18n.intlify.dev/) to translate our applications.
It's important to understand the power of this tool since it will save you a lot of time when creating multilingual applications.

<img width="120" src="img/projectSetup/typescript_logo.png">

### 7. What the Typescript

TypeScript is a tool that helps developers write code with fewer bugs. TypeScript is a superset of JavaScript,
meaning any valid JavaScript code is also valid TypeScript code. It helps a lot with type checking and makes it easier
to write code.

#### 7.1 Typescript config
The TypeScript config file is used to configure the TypeScript compiler. You can add custom types, change the
compiler options and more.

<img width="220" src="img/projectSetup/google_fonts_logo.png">


### 9. @ Alias for src folder

In our vue imports, we can use the @ alias to import files from the src folder. This is a lot easier than using
relative paths.
For example:

```js 
import {Button} from '@/components
``` 

instead of:

```js
import {Button} from '../../components'
```

This alias is configured in the `vite.config.js` file.
Maybe do a little research about how you can configure your vite environment to accept the usage of this alias.

### 10. Important files

#### 10.1 .env

The `.env` file is used to store environment variables. These variables can be used in your application.
It is mainly used to separate development and production variables. For example, you can use a different API url in
development than in production. Most of our projects have 3 different `.env` files: `.env.development`, `.env.staging` and `.env.production`.
Locally you can override these variables by creating a `.env.local` file. This file will be ignored by git.

#### 10.2 .gitignore

The `.gitignore` file is used to tell git which files it should ignore. For example, you don't want to commit your
node_modules folder to git. This file is used to tell git to ignore this folder.

### That's it for now! 🎉 Soak it all in and let's get started with the project setup! 🚀

<img width="400" src="img/projectSetup/look_up.gif">

## Project Structure

<img width="300" src="img/projectStructure/organized.gif">

### Folder structure

The template uses 'split-by-module' folder structure. Although 'split-by-module' is mainly recommended for medium to large applications, we will still use it here. As you won't be working on small applications for long 😉;

You can read more about it here: [Folder structure](https://thefrontendbible.com/project-structure)

### Assets

Assets are files that are used throughout your application. This can be images, fonts, icons, etc.
Inside the assets folder, you will already find a `styles` folder. Inside you will find a `base.css`, `tailwind.css` and a `colors.css` file.

The `base.css` file will be imported in the `main.ts` file and is used to import all the other css files and set some base css rules.
The `tailwind.css` file is used to configure tailwind theme variables (read it [here](https://tailwindcss.com/docs/theme#theme-variable-namespaces)).

The `colors.css` file is used to define all the colors that are used in the application. you should never change this file beacuse it
is carefully crafted to match our design system. To change colors you must look inside the `themes` directory. Here you will fiind a 
`default.css` file. And if you need more than 1 theme you can add more files here.

So the `default.css` file will set the colors in to css-variables, and the `colors.css` file will import these variables and put them into more application specific variables to match our design system.
And these variables will be set in the `tailwind.css` file.

### client

In this folder you will find files generated from the the back ends documentation using OpenApi-plugin. 
Inside are all the types for your DTO's and functions to fetch data. If the backend changes you can regenerate these files.

more on the OpenApi plugin [bible of docs link?]() 

### Component Styles

Inside this directory you can add new styling variants for components coming form the vue-core component library.

more info is in the [bible]()

### Components

Components are the building blocks of Vue.js applications.
They are self-contained pieces of code that can be reused throughout your application.

You can read more about it here: [Components](https://thefrontendbible.com/components)

### Composable

Composable look like a util function, but the main difference is that they can contain state and leverage the
reactivity of Vue.js.

You can read more about it here: [Composables](https://thefrontendbible.com/reusable-code/composables)

### Configs

Configs are used to store configuration values for plugins/packages that are used throughout your application. 

### Constants

Constants are used to store hardcoded values that are used throughout your application.

### Helpers
a place for helper functions that are used throughout your application.

### Icons

Icons are used to store the icons that are used throughout your application.

### Libs

Libs are used to store the libraries that are used throughout your application.

### locales

Locales are used to store the translations of your application. This is useful when you want to support multiple

### Middlewares

Middlewares acts like a bridge between the backend and the frontend. They are used to transform the data that is
received from the backend or route protection.

### Mocks

Mocks are used to mock the data that is received from the backend. This is useful when you want to develop without a working
backend or for testing purposes.

### Models

Models are used to store the types and interfaces that are used throughout your application.

### Modules

Modules are collections of components, views, stores, services, etc. that are used to create a specific feature of your
application. Here is a list of some important folders inside the modules folder:

- Api: This folder is used to store the queries, mutations and services that are used to fetch and update data from the backend.
- Constants: This folder is used to store the constants that are used throughout the module.
- Components: This folder is used to store the components that are used throughout the module.
- features: This folder is used to store the features that are used throughout the module.
- routes: This folder is used to store the routes that are used throughout the module.

### Plugins

Plugins are used to add functionality to your Vue.js application. They can be used to add third-party libraries, add
global components, etc.

### Routes

The routes is the core of Vue.js applications. It is used to navigate between different views.

You can read more about it here:

- [Best practices](https://thefrontendbible.com/reusable-code/router)
- [Routes](https://v3.vuejs.org/guide/routing.html#basic-routes)

### Stores

Stores are used to store the state of your application. This is useful when you want to share data between different
components. This folder is only for global stores, if you have a store that is only used in a specific component, you
should store it inside the component folder. only global stores should be located in this folder.

You can read more about it here:

- [Best practices](https://thefrontendbible.com/reusable-code/stores)
- [Pinia](https://pinia.esm.dev/)

### Transitions

Transitions are used to add animations to your application. This is useful when you want to add a smooth transition
between different views or components.

### Utils

Utils are reusable pieces of code that can be throughout your application.
They contain no state and are not tied to a specific component.

You can read more about it here: [Utils](https://thefrontendbible.com/reusable-code/utils)

### Worth mentioning

#### Queries & Mutations (Tanstack)

For fetching data from the backend we use [Vue Query](https://tanstack.com/query/v4/docs/vue/overview). Vue Query is a Vue plugin that
makes it easy to fetch, cache and update asynchronous data in your components without the hassle of setting up a
dedicated global store.

We also use their mutations to update data in the backend.

You can read more about it here:

- [Best practices queries](https://thefrontendbible.com/reusable-code/queries)
- [Best practices mutations](https://thefrontendbible.com/reusable-code/mutations)

- [Best practices](https://thefrontendbible.com/reusable-code/services)

### Internationalization (i18n)

Locales are used to store the translations of your application. This is useful when you want to support multiple
languages.

You can read more about it here: [Locales](https://thefrontendbible.com/locales)

#### Types & Interfaces

At Wisemen we use Typescript to type all of our code.
This is useful when you want to make sure that your code is correct and leverage the power of intellisense.
It will also help you to avoid bugs, improve your code quality and make your code more readable.

Lastly, your team will be able to understand your code better and don't have to make assumptions about the code.

Consult the front-end bible to find out more about types and interfaces. [For example](https://thefrontendbible.com/components/props#typescript-constructor)

> aside positive
> Remember: look around in the template, try to understand the project structure and how it works.
> If there are any files or folders that you don't understand, ask your buddy for help.

## Vue-core

The vue-core is a component library that contains the most common components that we use in our projects. It is a work in progress and we try to improve it every day.
You can use the components straight out of the box. But you can also customize them, this is done by making your own style config.

All the avaialble components can be found in the [vue-core documentation (wip?)]()

The cool thing about the vue-core library is that you can customize the components to your needs. This is done by making your own style config.
If you want to for example change the background color of a textfield input form to red, you can do it like this:

```vue
<script  lang="ts" setup>
import { VcTextField } from '@wisemen/vue-core'
import { ref } from 'vue'

const model = ref<string>('')
</script>

<template>
  <VcTextField
    v-model="model"
    :style-config="{
      '--text-field-bg-color-default': 'red',
    }"
  />
</template>
```

We import the `VcTextField` component from the vue-core library and create a new style config object.
In this object we set the `--text-field-bg-color-default` variable to red. there are a lot of predefined variables that you can use to customize the components.


## PROJECT: Battle plan 

Now that we have a basic understanding of the project template
and the different kinds of elements that a frontend should contain,
let's get started with building the actual application.

- Before we can create, update and delete todo's, we need to be able to login to the application.
Luckily for us, the template already contains a fully functional login page. 
- Once the user is logged in, we will need to create a view that contains a list of todo's. 
- This list will be fetched from the backend using queries and displayed in a list view. 
- Once we can display the todos, we will need to create a dialog that contains a form that can be used to create a new todo. 
- Here you will learn about mutations and how to use them to update data in the backend and invalidate your queries.
- After completing our create form, we will need to update it so that we can edit them.
- Once we can create and edit them, we will need to add a button to delete them.
- After we have completed these tasks, we will need to add a button to the list view that can be used to mark a todo as done.
- If you have time left, you can add some extra features to the application. For example, you can add a search bar to search for todos, or add a filter to filter the todos by status.

> aside negative
> The snippets provided in the codelab are examples to help you get started and move you in the right direction. 
> It's your own responsibility to make sure that the code is correct and that it works as expected.

## PROJECT: Http client

The most important aspect of programming is **separation of concerns.** and **DRY** (Don't Repeat Yourself).
This means that you should separate your code into different layers and files.
This will make your code more readable, reusable and easier to maintain.

You can easily do your calls in the component itself, but this will make your component less readable and harder to
maintain in the future.

That's why we use services to make our backend calls. This way we can separate the concerns and make our code more
readable and maintainable.

The template will do almost everything authentication related for you. You only need to change the environment variables to match the backend.

### Environment variables
To make sure that we don't hardcode the base url of the backend in our service, we will use environment variables.

- Create a new file called `.env` in the root of your project.
- Add a new variable called `API_BASE_URL` and set it to the base url of the backend.
- Do the same for the `AUTH_BASE_URL`, `AUTH_CLIENT_ID` and `AUTH_ORGANIZATION_ID` variables. These will be used with Zitatel to authenticate the user.

[//]: # (TODO: zet de juiste ENV's voor de todo app)
```env
API_BASE_URL=https://vue-node.project-template.development.appwi.se/api/v1

AUTH_BASE_URL=https://zitadel.internal.appwi.se
AUTH_CLIENT_ID=294498462244882333
AUTH_ORGANIZATION_ID=284257737964064935

AUTH_GOOGLE_IDP_ID=
AUTH_APPLE_IDP_ID=

ENVIRONMENT=development

```

### Using the HTTP client

If you go to the `http.lib.ts` file in the `libs` folder, you will see that the `httpClient` is already created for you.
This is a httpClient using axios in combination with zod to validate the responses. How this is handled is done in a seperate
package created by Wisemen. If you are interested in how it works, you can look at the github repo: [github link](https://github.com/wisemen-digital/vue-core/tree/main/packages/zod-http-client)

A different method used in newer projects is to use OpenApi to generate the client. 
This is a package that will generate the client for you based on the backend documentation. It also generates the types of the dto's which is very handy.
This is configured in the `openapi.config.ts` file. [bible link voor openapi]()

If this is configure right, you can generate everything by running the command:
```bash
pnpm openapi-ts
```

After logging in, the tokens will be stored in the local storage. And the user data will be stored in the Auth Store inside the `auth.store.ts` file.
If you want to know how this works, you can look at the bible [bible link die nog niet bestaat]()

> aside positive
> You can find the `client_id` and `client_secret` in the backend documentation.

💡Don't forget to make a pull request of your work so your buddy can review your code and keep track of your progress. Keeping your PR's small and frequent is a good practice.



## PROJECT: Router

The router is the core of Vue.js applications. It is used to navigate between different views.
It is also used to handle authentication and permissions for specific routes using "guards".
This is useful when you want to protect a route from being accessed by unauthenticated users. This is handled inside the `authMiddleware` and explained [here (bible tekst over middleware)]()

### Creating new routes

The starting point of the router is the `router.ts` file in the `src/router` folder. If you take a quick look, 
there is a place to add authenticated routes and unauthenticated routes. You can see there are already `userRoutes` and `settingRoutes`. 
You won't need these for this project, but you can use them as an example to create your own routes.

try and create a new route for your todos overview. 

- first you need to create a new folder inside the `modules` folder called `todos`.
- Inside this folder you need to create a `routes` folder and a `features` folder and in here you can create a `overview` folder.
- Inside the `overview` folder create a `views` folder. You can create a `TodoOverviewView.vue` file in here. This will be the view that will show the todos.
- Inside the `routes` folder you can create a `todos.routes.ts` file. This file will contain the routes for the todos module.
- Try to make a route for the `TodoOverviewView.vue` view. Don't forget to also add the route to the `router.ts` file.

Yes, this is a lot of folders and files. But this is how we structure our projects and if you work on larger projects you will see that this is very handy. 

💡Don't forget to make a pull request of your work so your buddy can review your code and keep track of your progress. Keeping your PR's small and frequent is a good practice.


## PROJECT: Displaying todo's

Now that we can login and our routes are set up, we can start with displaying the todo's.

### Model
First step in making an overview of data is to create a model that represents the data that we are going to display.
We are going to start by creating a file called `todoIndex.model.ts` in the `src/models/todo/index` folder.
We make an index-directory because we are also going to add a DTO model later on called `todoIndexDto.model.ts`.

We do this to create a separation between the model that we use in our frontend and the model that we receive from the backend. 

this is a good practice because the data that we receive from the backend is not always in the format that we want to use in our frontend. And when the BE changes the data structure, we only have to change the DTO model.

We are also going to need a transformer to transform the data that we receive from the backend into the format that we want to use in our frontend. 
this file will be called `todo.transformer.ts` and will be places in the `src/models/todos` folder.


`todoIndex.model.ts` will contain an interface that will represent a single todo with the following properties:
```typescript
export interface TodoIndex {
  uuid: string
  title: string
  description: string
  deadline: string
  isCompleted: boolean
}
```

`todoDto.model.ts` will contain an interface that will represent a single todo with the following properties (this is the data that we receive from the backend). You can make your own interface,
but because we use the OpenApi plugin, the DTO's are already generated for you. so you only have to this:
```typescript
import type { ViewTodoIndexView } from '@/client'

export type TodoIndexDto = ViewTodoIndexView
```
The naming of the generated DTO's is based on the endpoint and the method. So in this case the endpoint is `todo` and the method is `index`. but you can always look in the client file to find the type you are looking for.

`todo.transformer.ts` will contain a Class that will transform the data that we receive from the backend into the format that we want to use in our frontend. 
In this example both types are exactly the same, but in a real project this will not always be the case. 
```typescript
import { TodoIndexDto } from './todoDto.model'
import { TodoIndex } from './todo.model'

export class TodoIndexTransformer {
  static fromDto(data: TodoIndexDto): TodoIndex {
    return {
      uuid: data.uuid,
      title: data.title,
      description: data.description,
      deadline: data.deadline,
      isCompleted: data.is_completed,
    }
  }
}
```

### Service
After creating the model that we want to use in our frontend, 
we are going to create a file 'todo.service.ts' in the `src/modules/todos/api/services` folder. 

This service will contain a class `TodoService` with a static `getAll` method.

This is the place where we will use our transformer. And thus the **only** place where we will use the DTO model.
We also use the generated service from the OpenApi plugin to fetch the data from the backend. (again look in the generated service file to find the right function).

Important to note: the index call for getting the todo's is a paginated call. This means we have to add a offset and limit to the query params. And the data that we receive from the backend is not a list of todo's but a list of pages containing todo's.

Luckily for you, the template provides some composables and helper functions to make this super easy!

```typescript
export class TodoService {
  static async getAll(
      paginationOptions: PaginationOptions,
  ): Promise<PaginatedData<TodoIndex>> {
    const response = await viewTodoIndexControllerViewTodos<true>({
      query: new PaginationDtoBuilder(paginationOptions).build(),
        url: '/api/v1/todos',
    })
    return PaginatedDataTransformerUtil.fromDto(response.data, TodoIndexTransformer.fromDto)
  }
}
```

If you don't understand what all these helper functions and types are for, you can always ask your buddy for a quick explanation.

### Query
Next up we are going to create a query called `useTodoIndexQuery`.
This query will be used to call the `getAll` function from our service and fetch the todos from the backend.

The reason we use queries is so that we can easily fetch, cache and update asynchronous data in our components without the hassle of setting up a dedicated global store.

We use Tanstack Query for this. Read more about it [here](https://tanstack.com/query/latest/docs/framework/vue/overview)

```typescript

export function useTodoIndexQuery(
        paginationOptions: ComputedRef<PaginationOptions<{}>>,
): UseQueryReturnType<PaginatedData<TodoIndex>> {
  return useQuery<PaginatedData<TodoIndex>>({
    queryFn: () => {
      return TodoService.getAll(paginationOptions.value)
    },
    queryKey: {
      todoIndex: {
        paginationOptions,
      },
    },
  })
}
```

You also have to add the query key to the `src/types/queryKey.type.ts` file. There should be examples in there to help you.

### List component
Once we have created the query, we can start with creating a list component that will be used to display the todo's.

- Create a `TodoList.vue` (dumb) component in the `src/modules/todo/features/overview/components` folder.
- Add a list of todo's to the component.
- Add a message when there are no todo's.
- Add a loading state when the todo's are being fetched from the backend.

```vue
<script setup lang="ts">
const props = defineProps<{
  todos: Todo[]
  isLoading: boolean
}>()
</script>

<template>
<div>
  <div v-if="props.todos.length > 0">
    <ul>
      <li v-for="todo in props.todos" :key="todo.uuid">
        {{ todo.title }}
      </li>
    </ul>
  </div>
  <p v-else> No todo's found </p>
  <p v-if="props.isLoading">Loading...</p>
</div>
</template>
```

### View

The last step is to combine all of our pieces in a (smart) component that will be used to display the todo's.
This file should be named `TodoOverviewView` and we will put this in our `src/modules/todo/features/overview/views` folder.

This view will combine the query and list component we have created before.
```vue
<script setup lang="ts">
import { useTodoIndexQuery } from '@/modules/todos/services/todoIndex.query'
import { TodoIndex } from '@/models/todos/todoIndex.model'
import {computed} from 'vue'

const useTodoIndexQuery = useTodoIndexQuery()
const todos = computed<TodoIndex[]>(() => useTodoIndexQuery.data?.data ?? [])
const isLoading = computed<boolean>(() => useTodoIndexQuery.isLoading.value)
  
</script>

<template>
<div>
    <TodoList :todos="todos" :is-loading="isLoading" />
</div>
</template>
```

💡Don't forget to make a pull request of your work so your buddy can review your code and keep track of your progress. Keeping your PR's small and frequent is a good practice.

## PROJECT: Creating Todo's

Now that we have created the todo view and have a list of our existing todo's, we can start with creating new todo's.

The creation of a todo will be done in a dialog. This dialog will be displayed when the user clicks on the `Create todo`
button.
Dialogs are allowed to be smart components. The dialog will contain a form that allows to enter the required information
for creating a new todo.

### Form model
We are going to start by creating a file called `todoCreateForm.model.ts` in the `src/models/todos/create` folder.

This file will contain a form schema that will be used to create a new todo
```typescript
export const todoCreateFormSchema = z.object({
  title: z.string(),
  description: z.string(),
  deadline: z.string(),
})

export type TodoCreateForm = z.infer<typeof formSchema>
```
We again use a DTO model for this to separate the data that we send to the backend from the data that we use in the frontend. We can use the generated DTO for this.
so in the same folder you can create a `todoCreateDto.model.ts` file with the following content:
```typescript
import type { CreateTodoCommand } from '@/client'

export type TodoCreateDto = CreateTodoCommand
```


> aside positive
> We use the **zod** library to create our form schemas. This library is used to validate and transform data.
> You can read more about it here: [Zod.dev](https://zod.dev/)

Also make a transformer for this model. Make a second class called `TodoCreateTransformer` in the `todo.transformer.ts` file.
### Service
After creating the model that we want to add a new function to our existing service that will be used to create a new todo.

```typescript


export class TodoService {
  ...
  static async create(form: TodoCreateForm): Promise<void> {
    await createTodoControllerCreateTodoV1<true>({
      body: TodoService.toDto(form),
      url: '/api/v1/todos',
    })
  }
}
```

### Mutation
Next up we are going to create a mutation called `useTodoCreateMutation`.

This mutation will be used to call the `create` function from our service and create a new todo in the backend.

```typescript
export function useTodoCreateMutation(): UseMutationReturnType<TodoCreateForm, void, void> {
  return useMutation<TodoCreateForm, void, void>({
    queryFn: async ({ body }) => {
      return await TodoService.create(body)
    },
    queryKeysToInvalidate: {
      todoIndex: {},
    },
  })
}

```

> aside positive
> If you're not sure how to use `useMutation`, you can take a look at the [Vue Query documentation](https://tanstack.com/query/v4/docs/vue/guides/mutations).

### Dialog (smart) component
Once we have created the mutation, we can start with creating a dialog component that will be used to create the todo's.

- Create a `TodoCreateDialog.vue` (smart) component in the `src/modules/todos/components` folder.
- Add a form that allows the user to enter a `title`, `description` and `deadline`.
- Add a submit button that will call the `useTodoCreateMutation` mutation.

> aside positive
> For more info about form validation you can check out our [Formango](https://github.com/wisemen-digital/vue-formango) library.

```vue
<script setup lang="ts">
import { useForm } from 'formango' 
const apiErrorToast = useApiErrorToast()
const todoCreateMutation = useTodoCreateMutation()

const emit = defineEmits<{
  close: []
}>()t

const form = useForm({
  schema: todoFormSchema,
  initialState: {
    title: '',
    description: '',
    deadline: '',
  },
})

const title = form.form.register('title')

function onSubmit(): void {
  form.form.submit()
}

function onClose(): void {
  emit('close')
}

form.onSubmitForm(async (formData) => {
  try {
    await todoCreateMutation.mutateAsync({
          data: formData
        }) // notice the async keyword here, it's very important
  } catch (error) {
    apiErrorToast.show(error)
  }
})
</script>

<template>
    <VcDialog
        @close="onClose"
    >
        <AppDialogContent
                class="w-dialog-sm"
        >
        <AppForm :form="form.form"">
            <VcInput v-bind="title" />
            <AppDialogActions>
                <AppDialogActionCancel
                        @click="onClose"
                        :label="..." />
                <FormSubmitButton
                        :form="form.form"
                        :label="..."
                />
            </AppDialogActions>
          </AppForm>
        </AppDialogContent>
  </VcDialog>
```

> aside positive
> You are going to use the components from the vue-core library. You can find the documentation [here](https://vue-core.wisemen.digital/).
> Try and understand how the components work and. If anything is unclear, you can always ask your buddy for help.


### View
To finish up, we are going to update our `TodoOverviewView` by adding a button that will open the `TodoDialog` when clicked.
use the useDialog composable to make it all work!

```vue
<script setup lang="ts">
...
const todoCreateDialog = useDialog({
  component: () => import('@/modules/todos/components/TodoCreateDialog.vue'),
}) 

function onCreateButtonClick(): void {
  todoCreateDialog.open()
}
...
</script>

<template>
<div>
    <TodoList :todos="todos" :is-loading="isLoading" />
    <button @click="onCreateButtonClick">Create todo</button>
    <TodoModal v-if="isModalOpen" @close="handleClose" />
</div>
</template>
```

💡Don't forget to make a pull request of your work so your buddy can review your code and keep track of your progress. Keeping your PR's small and frequent is a good practice.

## PROJECT: Updating and deleting todo's

The last step is to allow the user to update and delete existing todo's. This will be done by clicking on the edit button of a todo.
We are going to extend the functionality of the `TodoModal` component to allow the user to update a todo.
To achieve this, we need to know if the modal is opened in `create` or `update` mode. The easiest way to do this is to
check if a todo uuid is passed to the modal.

### Service
Now it's time to add a new function to our existing service that will be used to update a todo. try it yourself!

```typescript
export class TodoService {
    ...
  static async update(uuid: TodoUuid, form: TodoForm): Promise<void>{
    ...
  }
  
  static async deleteByUuid(uuid: TodoUuid): Promise<void> {
    ...
  }
}
```

> aside negative
> You will need to provide the `TodoUuid` type for yourself. Zod allows you to create a custom type for this using **brands**.
> More info can be found here: [https://zod.dev/?id=brand](https://zod.dev/?id=brand)

### Mutation
Once we have added the `update` and `deleteByUuid` functions to our service, we can start with creating the mutations. also try this yourself, it is very similar to the create mutation.

### Modal (smart) component
Now it's time to extend the functionality of the `TodoModal` component to allow the user to update a todo.

- Add a `uuid` prop to the `TodoModal` component.
- Add a `update` function to the `TodoModal` component that will call the `useTodoUpdateMutation` mutation.
- Add a `delete` function to the `TodoModal` component that will call the `useTodoDeleteMutation` mutation.

```vue
<script setup lang="ts">

const props = defineProps<{
  todo: Todo | null
}>()

const updateMutation = useTodoUpdateMutation()
const deleteMutation = useTodoDeleteMutation()

const form = useForm({
  schema: todoFormSchema,
  initialValues: {
    title: props.todo?.title || '',
    description: props.todo?.description || '',
    deadline: props.todo?.deadline || '',
  },
})

const title = form.form.register('title')
...

function onSubmit(): void {
  form.form.submit()
}

form.onSubmitForm(async (formData: TodoForm) => {
  try {
    if (props.todo) {
      await updateMutation.mutateAsync(props.todo.uuid, formData)
    } else {
      await createMutation.mutateAsnyc(formData)
    }
  } catch (error) {
    console.error(error)
  }
})

function handleDelete(uuid: TodoUuid): void {
  deleteMutation.mutateAsync(uuid)
}

</script>

<template>
<div>
  ...
    <form @submit.prevent="onSubmit">
        <input v-model="title.value" />
        ...
        <button type="submit">Submit</button>
    </form>
    <button @click="handleDelete(props.uuid)">Delete</button>
  ...
</div>
</template>
```

💡Don't forget to make a pull request of your work so your buddy can review your code and keep track of your progress. Keeping your PR's small and frequent is a good practice.

## PROJECT: Writing your first test

## Finishing up

Congratulations! You have successfully completed our Vue.js workshop. 🥳🤩

<img width="600" src="img/the-office-dwight.gif">

Make sure that your project has been pushed to your repository and that you have created a pull request.
Fix any remarks that you have received from your mentor and wait for the final feedback.

Also make sure your styling is consistent with the designs and adjust where necessary.
