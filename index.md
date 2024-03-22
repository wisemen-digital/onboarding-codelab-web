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
You will learn how to work with Vue, Vite, Tailwind, Figma, Github, Jira and more.  
  
This onboarding is designed to be completed in roughly 3-4 days.  
This does not mean you have to complete it in 3-4 days.   
People with more experience will be able to complete it faster than people with less experience.  
  
In this codelab we are going to create a simple to-do app.  
This app will be used as example to teach you how we structure our projects, which tools and libraries we use.  
  
> aside positive  
> One important thing to know is that you will be creating most stuff from scratch in this codelab.  
> This is to make sure you understand how everything works and how the pieces are connected behind the scenes.  
> When we create projects for our customers we always start from our [project template](https://github.com/wisemen-digital/project-template-vue).  
> The project template contains pre-built features, components, tools and configurations so that we can get started quickly and don't have to reinvent the wheel every time we start a new project.  
  
We also expect you to make pull request of your work so your buddy can review your code and keep track of your progress.  
The way we do this will be explained in the onboarding.  
  
Good luck on becoming the front-end developer you are meant to be!  
  
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
- **Bitbucket pull** requests (The plugin allows you to review Atlassian Bitbucket pull requests right in the IDE.)  
	- This plugin requires a license to use. If you don't have this already, ask your buddy.
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
  
### Figma  
  
Our designers work with **Figma**.  
Figma is a vector graphics editor and prototyping tool which is browser-based or can be installed on macOS or Windows.  
We recommend you to install the desktop app.  
  
[Download Figma](https://www.figma.com/downloads/)  
  
Take a look around in Figma and try to get familiar with the tool. You will be using it a lot in the future.  
You can view all of our designs here:  
  
[Wisemen Figma](https://www.figma.com/files/team/1070403287155222588/Wisemen?fuid=1070747045190465434)  
  
To access the [designs of this onboarding](https://www.figma.com/file/hebgv4Qx8VanMAQkO1NFpa/Onboarding-to-do?type=design&node-id=467-4945&mode=design&t=G5ZyDUuWvBO3FKUl-0) you need to log in with your Wisemen account. (You might not have access to these yet if you just started. If that's the case you can ask your buddy about it.)
  
### Source control  
  
#### BitBucket repository  
  
Bitbucket is a web-based version control repository hosting service owned by Atlassian, for source code and development  
projects that use the Git revision control system.  
  
Some of our older projects are still hosted on [BitBucket](https://bitbucket.org/product) .  
  
If you are not yet familiar with Bitbucket and/or Git, Here is great article to get you started:  
[Bitbucket Git tutorial](https://www.atlassian.com/git/tutorials/what-is-version-control)  
  
We also expect you to make [pull request](https://www.atlassian.com/git/tutorials/making-a-pull-request) of your work so your buddy can review your code and keep track of your progress.  
  
#### GitHub  
  
GitHub is another web-based version control repository hosting service owned by Microsoft, for source code and development  
projects that use the Git revision control system.  
  
Just like BitBucket, some of our projects will be hosted on GitHub. **_GitHub will be used for new projects_**.  
  
If you are not yet familiar with GitHub, Here is great article to get you started:  
[GitHub Git tutorial](https://docs.github.com/en/get-started/start-your-journey/hello-world)  
  
Same as with BitBucket, we expect you to make [pull requests](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/creating-a-pull-request) of your work so your buddy can review your code and keep track of your progress.  
  
> aside positive  
> We switched to GitHub for our new projects.   
> You can find our GitHub organization here: [Wisemen GitHub](https://github.com/wisemen-digital)  
  
### Jira access  
  
For this onboarding you will be working with Jira to track your progress. You can find the Jira board here:  
[Jira Todo]()  
  
Jira is used to track the progress of your project and manage the tasks that need to be done.  
All the requirements for the to-do app are in the Jira. You will be creating tasks in the Jira to keep track of your progress.  
  
The Jira contains all the requirements for creating the to-do app.  
  
*ToDo: Add a link to Jira!*
  
## Project explanation  
  
You will be creating a simple to-do app. The app can be used to create, edit and delete to-do's.  
The backend is already created and you can find the documentation here:  
  
[Backend documentation](https://onboarding-todo-api.development.appwi.se/api/v1/docs/)  
  
Username: `appwise`  Password: `password`  
  
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
  
### 1. A Vue3 project  
  
We use the latest version of Vue for this project. Vue3 is the latest version and has some new features and  
improvements over Vue2. You can read more about Vue3 here: [Vue3 website](https://vuejs.org/)  
Make sure you use the CLI version to create the project.  
  
  
Create new project using the Vue CLI:  
```shell  
pnpm create vue@latest```  
  
Use the following settings:  
  
<img width="1000" src="img/vue-cli-config.png">  
  
---  
  
### 2. Vite  
  
Vite is a new breed of frontend build tool that significantly improves the frontend development experience. It consists  
of two major parts:  
  
- A dev server that provides rich feature enhancements over native ES modules, for example extremely fast Hot Module  
  Replacement (HMR) that updates your changes in the browser in as little as 16 milliseconds.  
- A build command that bundles your code with Rollup, pre-configured to output highly optimized static assets for  
  production.  
  
#### 2.1 Config  
  
Vite is configured using a `vite.config.js` file in the root of your project. This file is written in CommonJS format  
and should export a plain JavaScript object. Make sure to change this file from `.js` to `.ts`  
  
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
  
The scripts property is used to specify a list of scripts that can be run using `pnpm run 'script-name'`.  
It's written as a JSON object where each key is the name of a script and the value is the command to run for.  
Most common scripts are `dev` and `build`.  
  
#### 3.2 Dependencies vs Dev Dependencies  
  
Dev dependencies are dependencies that are only used during development and are not required for production.  
Dependencies are required for production.  
  
### 4. Tailwind CSS  
  
Tailwind CSS is a utility-first CSS framework for rapidly building custom user interfaces. It's completely  
customizable, completely extensible, and amazingly feature-rich.  

<img width="120" src="img/projectSetup/tailwind_logo.png">  
#### 4.1 Tailwind config  
  
Tailwinds config file is used to configure the framework. You can add custom colors, fonts, breakpoints and more.  
This is where you can customize the framework to your needs.  
  
👉 [Tailwind website](https://tailwindcss.com/)  

> aside positive
> Read the [installation guide](https://tailwindcss.com/docs/guides/vite#vue) if you've never used Tailwind before.
  
### 5. ESLint config  
  
ESLint is a tool for identifying and reporting on patterns found in ECMAScript/JavaScript code, with the goal of  
making code more consistent and avoiding bugs. Is helps a lot with code formatting and makes it easier to write code.  
Also in team projects it helps to keep the code consistent.  
  
> aside positive  
> Please make sure you use the Wisemen ESLint config file in your project,   
> you can read how to configure it here: [The Frontend bible ESLint config](https://thefrontendbible.com/eslint-config)  
  
<img width="120" src="img/projectSetup/ESLint_logo.png">  
  
### 6. Internationalization (i18n)  
  
i18n is a short name for internationalization. It is a process of designing and developing a software application so  
that it can be adapted to various languages and regions without engineering changes.  
  
Within the company we use [Vue i18n](https://vue-i18n.intlify.dev/) to translate our applications.  
It's important to understand the power of this tool since it will save you a lot of time when creating multilingual applications.  
  
<img width="120" src="img/projectSetup/vue_i18n_logo.svg">  
  
### 7. What the Typescript  
  
TypeScript is a tool that helps developers write code with fewer bugs. TypeScript is a superset of JavaScript,  
meaning any valid JavaScript code is also valid TypeScript code. It helps a lot with type checking and makes it easier  
to write code.  

> aside positive
> If you're new to typescript, the [typescript handbook](https://www.typescriptlang.org/docs/handbook/2/basic-types.html) is a good place to start

<img width="120" src="img/projectSetup/typescript_logo.png">  
#### 7.1 Typescript config  
The TypeScript config file is used to configure the TypeScript compiler. You can add custom types, change the  
compiler options and more.  
  
### 8. ⚠️ Google fonts ⚠️  
  
It's important to know that we cannot use Google fonts CDN in our projects. This rule is only for public websites of  
our clients.  
We have alternative ways of using Google fonts in our projects.  
<img width="220" src="img/projectSetup/google_fonts_logo.png">  
  
> aside negative   
> Please read more here: [Afstappen van Google Fonts en CDN javascript](https://appwise.atlassian.net/wiki/spaces/FRONT/pages/631734284/Afstappen+van+Google+Fonts+en+CDN+javascript).   
> If you have any questions about this, please contact your team lead.  
  
### 9. @ Alias for src folder  
  
In our vue imports, we can use the @ alias to import files from the src folder. This is a lot easier than using  
relative paths.  
For example:  
  
```js import {Button} from '@/components  
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
  
For this project we will be using a 'split-by-module' folder structure. Although 'split-by-module' is mainly recommended for medium to large applications, we will still use it here. As you won't be working on small applications for long 😉;  
  
You can read more about it here: [Folder structure](https://thefrontendbible.com/project-structure)  
  
### Assets  
  
Assets are files that are used throughout your application. This can be images, fonts, icons, etc.  
  
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
  
### Icons  
  
Icons are used to store the icons that are used throughout your application.  
  
### Libs  
  
Libs are used to store the libraries that are used throughout your application.  
  
### Middlewares  
  
Middlewares acts like a bridge between the backend and the frontend. They are used to transform the data that is  
received from the backend or route protection.  
  
### Models  
  
Models are used to store the types and interfaces that are used throughout your application.  
  
### Modules  
  
Modules are collections of components, views, stores, services, etc. that are used to create a specific feature of your  
application. Here is a list of some important folders inside the modules folder:  
  
- **api**: This folder is used to store the queries, mutations and services that are used to fetch and update data from the backend.  
- **constants**: This folder is used to store the constants that are used throughout the module.  
- **components**: This folder is used to store the components that are used throughout the module.  
- **features**: This folder is used to store the features that are used throughout the module.  
- **routes**: This folder is used to store the routes that are used throughout the module.  
- **stores**: This folder is used to store the stores that are used throughout the module.  
  
### Plugins  
  
Plugins are used to add functionality to your Vue.js application. They can be used to add third-party libraries, add  
global components, etc.  The plugins folder contains the configurations of these plugins (ex. i18n)
  
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
  
### Transformers  
  
Transformers are used to transform the data that is received from, and sent to the backend. This is useful when you want to transform  
the data into a format that is easier to work with. This should be a single file per module.  

You can read more about it here:  
* [Best practices](https://thefrontendbible.com/reusable-code/transformers)
  
### Transitions  
  
Transitions are used to add animations to your application. This is useful when you want to add a smooth transition  
between different views or components.  
  
### Utils  
  
Utils are reusable pieces of code that can be throughout your application.  
They contain no state and are not tied to a specific component.  
  
You can read more about it here: 
* [Utils](https://thefrontendbible.com/reusable-code/utils)  
  
### Views  
  
Views are the pages of your application. They are the components that are rendered when a specific route is visited.  
  
You can read more about it here: 
* [Views](https://v3.vuejs.org/guide/routing.html#basic-routes)  
  
### Worth mentioning  
  
#### Queries & Mutations (Tanstack)  
  
For fetching data from the backend we use [Vue Query](https://tanstack.com/query/v4/docs/vue/overview). Vue Query is a Vue plugin that  
makes it easy to fetch, cache and update asynchronous data in your components without the hassle of setting up a  
dedicated global store.  
  
We also use their mutations to update data in the backend.  
  
You can read more about it here:  
  
- [Best practices queries](https://thefrontendbible.com/reusable-code/queries)  
- [Best practices mutations](https://thefrontendbible.com/reusable-code/mutations)  
  
#### Services & Http  
  
Services are used to fetch data from the backend. These backend calls are made using the Http client.  
  
You can read more about it here:  
  
- [Best practices](https://thefrontendbible.com/reusable-code/services)  
  
### Internationalization (i18n)  
  
Locales are used to store the translations of your application. This is useful when you want to support multiple  
languages.  
  
You can read more about it here: 
* *Todo: Add link*
  
#### Types & Interfaces  
  
At Wisemen we use Typescript to type all of our code.  
This is useful when you want to make sure that your code is correct and leverage the power of intellisense.  
It will also help you to avoid bugs, improve your code quality and make your code more readable.  
  
Lastly, your team will be able to understand your code better and don't have to make assumptions about the code.  
  
Consult the front-end bible to find out more about types and interfaces. [For example](https://thefrontendbible.com/components/props#typescript-constructor)  
  
## PROJECT: Battle plan   
  
Now that we have a basic understanding of the project structure  
and the different kinds of elements that a frontend should contain,  
let's get started with building the actual application.  
  
- Before we can create, update and delete todo's, we need to be able to login to the application.  
There are several components that we need to create before we can start with the authentication flow.   
- We will need to create a view that contains a login form. This form will be used to send the login credentials to the  
backend.  
- We will also need to create a service that will be used to send the login request to the backend.   
- To complete the login flow we will need to create a store that will be used to store the user information when the user is logged in.  
- Once the user is logged in, we will need to create a view that contains a list of todo's.   
- This list will be fetched from the backend using queries and displayed in a list view.   
- Once we can display the todos, we will need to create a modal that contains a form that can be used to create a new todo.   
- Here you will learn about mutations and how to use them to update data in the backend and invalidate your queries.  
- After completing our create form, we will need to update it so that we can edit them.  
- Once we can create and edit them, we will need to add a button to delete them.  
- After we have completed these tasks, we will need to add a button to the list view that can be used to mark a todo as done.  
- To finish the project, we will need to add a logout button to log out the user.  
  
> aside negative  
> The snippets provided in the codelab are **examples** to help you get started and move you in the right direction.   
> It's your own responsibility to make sure that the code is **correct** and that it works as expected.

> aside positive
> **LIFE PRO TIP**: Always be critical about code you copy!
  
## PROJECT: HTTP client  
  
The most important aspect of programming is **separation of concerns.** and **DRY** (Don't Repeat Yourself).  
This means that you should separate your code into different layers and files.  
This will make your code more readable, reusable and easier to maintain. Doing this can be especially powerful in services like the HTTP client because this enforces code reusability.
  
You can easily do your calls in the component itself, but this will make your component less readable and harder to  
maintain in the future.  
  
The HTTP client we're going to make will be *responsible* for sending requests to the backend. The first request we're going to have it do is the *login request*.
### Environment variables  
To make sure that we don't hardcode the base url of the backend in our service, we will use environment variables.  
  
- Create a new file called `.env` in the root of your project.  
- Add a new variable called `VITE_BASE_URL` and set it to the base url of the backend.  
- Do the same for the `VITE_CLIENT_ID` and `VITE_CLIENT_SECRET` variables.
  
```env  
VITE_BASE_URL=https://onboarding-todo-api.development.appwi.se/api/v1  
VITE_CLIENT_ID=ENTER_YOUR_CLIENT_ID_HERE  
VITE_CLIENT_SECRET=ENTER_YOUR_CLIENT_SECRET_HERE  
```  
> aside positive  
> You can find the `client_id` and `client_secret` in the backend documentation.  
### Creating the HTTP client  
  
- Add the `axios` package to the project.  
- Create a new file called `httpClient.ts` in the `src/http` folder.  
- Create a new instance of axios and export it.  
- Add an interceptor that will be used to add the `Authorization` header to all requests.  
  
```typescript  
const httpClient: AxiosInstance = axios.create({  
  baseURL: import.meta.env.VITE_BASE_URL,  headers: {    'Accept': 'application/json',    'Content-Type': 'application/json;charset=UTF-8',  },})  
```  
  
### Creating the auth service  
- Create a new file called `auth.service.ts` in the `src/modules/auth/services` folder.  
- Import the `httpClient` from the `src/http` folder.  
- Create a new function called `login` that takes a `username` and `password` as parameters.  
- Use the `httpClient` to make a `POST` request to the `/login` endpoint.  
  
```typescript  
interface AuthService {  
  login: (username: string, password: string) => Promise<void>  getCurrentUser: () => Promise<CurrentUser>}  
  
export const authService: AuthService = {  
  login: async (username: string, password: string): Promise<AuthTokens> => {    const formData = encodeQueryData({      client_id: import.meta.env.VITE_CLIENT_ID,      client_secret: import.meta.env.VITE_CLIENT_SECRET,      grant_type: 'password',      password: password,      username: username,      scope: "read write"    })  
    const config = {      headers: {'Content-Type': 'application/x-www-form-urlencoded'},    }        const response = await httpClient.post('/auth/token', formData, config)  
    return response.data  },  getCurrentUser: async (): Promise<CurrentUser> => {    const response = await httpClient.get('/users/me')    return response.data  },}  
```  
  
  
💡Don't forget to make a pull request of your work so your buddy can review your code and keep track of your progress. Keeping your PR's small and frequent is a good practice.  
  
## PROJECT: Auth store  
  
### Creating the auth store  
  
The store will help us to save the tokens after a successful login.  
That's why we will always use a store to do our backend calls and never directly use the service in the component. (separation of concerns)  
  
- Create a new file called `auth.store.ts` in the `src/modules/auth/stores` folder.  
- Create a new store using the `defineStore` function from `pinia`.  
- Add a `accessToken` property to the store.  
- Add a `login` function to the store that takes a `username` and `password` as parameters.  
- Use the `AuthService` to make a `POST` request to the `/login` endpoint.  
- Save the `accessToken` in the store after a successful login.  
  
> aside positive  
> **LIFE PRO TIP**: You can use the [useLocalStorage](https://vueuse.org/core/useStorage/) composable from VueUse to store the user information directly in the local storage.  
  
```typescript  
export const useAuthStore = defineStore('auth', () => {  
  const currentUser = ref<User | null>(null)  const accessToken = useLocalStorage<string | null>(null)    const isAuthenticated = computed<boolean>(() => currentUser.value === null)  
    async function getCurrentUser(): Promise<User> {  
    if (currentUser.value !== null) {      return currentUser.value    }        currentUser.value = authService.getCurrentUser()  
    return currentUser.value!  }    function setCurrentUser(user: User | null): void {  
    currentUser.value = user  }    async function login(data: AuthLoginForm): Promise<void> {  
    const response = await authService.login(data.username, data.password)    accessToken.value = response.accessToken  }    function logout(): void {  
    authService.logout()    setCurrentUser(null)  }    return {  
    currentUser,    isAuthenticated,    getCurrentUser,    setCurrentUser,    login,    logout,  }})  
```  
  
> aside negative  t
> You will need to provide the `AuthLoginForm` en `User` model and type for yourself. We use the **zod** library to create our models and types. This library is used to validate and transform data. You can read more about it here: [Frontend bible](https://thefrontendbible.com/reusable-code/models) & [Zod.dev](https://zod.dev/)
  
💡Don't forget to make a pull request of your work so your buddy can review your code and keep track of your progress. Keeping your PR's small and frequent is a good practice.  
  
## PROJECT: Router  
  
The router is the core of Vue.js applications. It is used to navigate between different views.  
It is also used to handle authentication and permissions for specific routes using "guards".  
This is useful when you want to protect a route from being accessed by unauthenticated users.  
  
### Creating the router  
  
- Create a new file `router.ts` in the `src/router` folder.  
- Implement a router using the `createRouter` function from `vue-router`.  
- Create empty components called `AuthLoginView.vue` and `TodoOverviewView.vue` in the `src/views` folder.  
- Add a `login` and `todos` route to the router that lazy loads the `AuthLoginView` and `TodoOverviewView` components.  
  
```typescript  
const routes: RouteRecordRaw[] = [  
  {    path: '/login',    name: 'login',    component: async () => import('@/modules/auth/views/AuthLoginView.vue'),  },  {    path: '/',    name: 'index',    meta: { requiresAuth: true },    children: [      {        path: '/todos',        name: 'todos',      },    ],  },  {    name: 'error',    path: '/:pathMatch(.*)*',    component: async () => import('@/views/ErrorNotFoundView.vue'),  },]  
  
const router = createRouter({  
  history: createWebHistory(),  routes: routes})  
```  
  
### Router guards  
  
- Add a `beforeEach` guard to your router that checks if the user is logged in.  
- If the user is not logged in, redirect the user to the `login` route.  
- If the user is logged in, continue to the `todos` route.  
  
> aside positive  
> **LIFE PRO TIP**: You can use the `useAuthStore` to check if the user is logged in. If the user is not logged in, you can use the `router` to navigate to the `login` route.  
> If the user is logged in, you can use the `router` to navigate to the `todos` route.  
  
> aside positive  
> **LIFE PRO TIP**: You can add meta fields to your routes to check if the user is allowed to access a specific route.  
  
```typescript  
router.beforeEach(async (to, from, next) => {  
  // Add your guards here    next()  
})  
```  
  
💡Don't forget to make a pull request of your work so your buddy can review your code and keep track of your progress. Keeping your PR's small and frequent is a good practice.  
  
## PROJECT: Login view  
  
Now that we have created the store, service and router, we can start with creating the login view.  
Views are the "Smart components" in our application. They are allowed to import stores, routers, dumb components, etc.  

For more information, consult the frontend bible about [Smart and Dumb components](https://thefrontendbible.com/components/smart-dumb)
  
Our Login view will orchestrate the login flow. It will use the `authStore` to login the user and the `router` to  
navigate to the `TodoOverviewView` after a successful login.  
  
### Creating your Login view (smart) component  
  
- Create a view called `AuthLoginView.vue` in the `src/modules/auth/views` folder.  
- Create a new file called `AuthLoginForm.vue` in the `src/modules/auth/components` folder.  
- Add a form that allows the user to enter a `username` and `password`.  
- Add the `AuthLoginForm` component to the `AuthLoginView.vue` view.  

> aside positive
> We use a library called [Formango](https://wisemen-digital.github.io/vue-formango/) to validate our forms for us. If you have any questions while using Formango, don't hesitate to ask your buddy.
  
### Implementing the login flow  
  
- Import the `useAuthStore` and `useRouter` in your `AuthLoginView`.  
- Create a new `authStore` and `router` instance.  
- Use the `router` to navigate to the `TodoOverviewView.vue` view after successfully logging in.  
  
```vue  
<script setup lang="ts">  
const authStore = useAuthStore()  
const router = useRouter()  
  async function handleLogin(data: { username: string; password: string }): Promise<void> {  
  await authStore.login(data)  router.push({ name: 'todos' })}  
</script>  
  
<template>  
<div>  
    <AuthLoginForm @submit="handleLogin" /></div>  
</template>  
```  

> aside negative
> Don't forget to use i18n for all texts that are visible to the user.

💡Don't forget to make a pull request of your work so your buddy can review your code and keep track of your progress. Keeping your PR's small and frequent is a good practice.  
  
## PROJECT: Displaying todo's  
  
Now that we have created the login flow, we can start with creating the todo view.  
After completing the login functionality, you should now have a good understanding of how we're going to create the todo view.  
  
### Model  
We are going to start by creating a file called `todo.model.ts` in the `src/modules/todos/models` folder.  
  
This file will contain an interface that will represent a single todo with the following properties:  
```typescript  
import { z } from 'zod'  
  
const todoSchema = z.object({  
  uuid: z.string().uuid(),  
  title: z.string(),  
  description: z.string(),  
  deadline: z.string().datetime(),  
  isCompleted: z.boolean(),  
})  
  
export type Todo = z.infer<typeof todoSchema> 
```  
  
### Service  
After creating the model that we want to use in our frontend,   
we are going to create a file 'todo.service.ts' in the `src/modules/todos/services` folder.   
  
This service will contain a function `TodoService` that returns another function called `getAll`.  
  
```typescript  
interface TodoService {  
  getAll: () => Promise<Todo[]>}  
  
export const todoService: TodoService = {  
  getAll: async (): Promise<Todo[]> => {    const response = await httpClient.get('/todos')    return response.items  },}  
```  
  
> aside positive  
> In a production project we would add an extra object called a "data transfer object" (DTO)   
> so that we can transform the data that is received from the backend into a format that is easier to work with.   
  
### Query  
Next up we are going to create a query called `useTodoIndexQuery`.  
This query will be used to call the `getAll` function from our service and fetch the todos from the backend.  
  
The reason we use queries is so that we can easily fetch, cache and update asynchronous data in our components without the hassle of setting up a dedicated global store.  
  
```typescript  
export function useTodoIndexQuery() {  
  return useQuery({    queryKey: 'todos',    queryFn: async () => {      const data = await todoService.getAll()      return data    },  })}  
```  
  
> aside positive  
> **LIFE PRO TIP**: If you're not sure how to use `useQuery`, you can take a look at the [Vue Query documentation](https://tanstack.com/query/v4/docs/vue/guides/queries).  
  
### List component  
Once we have created the query, we can start with creating a list component that will be used to display the todo's.  
  
- Create a `TodoList.vue` (dumb) component in the `src/modules/todos/components` folder.  
- Add a list of todo's to the component.  
- Add a message when there are no todo's.  
- Add a loading state when the todo's are being fetched from the backend.  
  
```vue  
<script setup lang="ts">  
const props = defineProps<{  
  todos: Todo[]  isLoading: boolean}>()  
</script>  
  
<template>  
<div>  
  <div v-if="props.todos.length > 0">    <ul>      <li v-for="todo in props.todos" :key="todo.uuid">        {{ todo.title }}      </li>    </ul>  </div>  <p v-else> No todo's found </p>  <p v-if="props.isLoading">Loading...</p></div>  
</template>  
```  
  
### View  
  
The last step is to combine all of our pieces in a (smart) component that will be used to display the todo's.  
This file should be named `TodoOverviewView` and we will put this in our `src/modules/todos/views` folder.  
  
This view will combine the query and list component we have created before.  
```vue  
<script setup lang="ts">  
import { useTodoIndexQuery } from '@/modules/todos/services/todoIndex.query'  
  
const { data: todos, isLoading } = useTodoIndexQuery()  
</script>  
  
<template>  
<div>  
    <TodoList :todos="todos" :is-loading="isLoading" /></div>  
</template>  
```  
  
💡Don't forget to make a pull request of your work so your buddy can review your code and keep track of your progress. Keeping your PR's small and frequent is a good practice.  
  
## PROJECT: Creating Todo's  
  
Now that we have created the todo view and have a list of our existing todo's, we can start with creating new todo's.  
  
The creation of a todo will be done in a modal. This modal will be displayed when the user clicks on the `Create todo`  
button.  
Modals are allowed to be smart components. The modal will contain a form that allows to enter the required information  
for creating a new todo.  
  
### Form model  
We are going to start by creating a file called `todoForm.model.ts` in the `src/modules/todos/models` folder.  
  
This file will contain a form schema that will be used to create a new todo  
```typescript  
export const todoFormSchema = z.object({  
  title: z.string(),  description: z.string(),  deadline: z.string(),})  
  
export type TodoForm = z.infer<typeof formSchema>  
```  

  
### Service  
After creating the model that we want to add a new function to our existing service that will be used to create a new todo.  
  
```typescript  
interface TodoService {  
  ...  create: (form: TodoForm) => Promise<void>}  
  
export const todoService: TodoService = {  
  ...  create: async (form: TodoForm): Promise<void> => {    await httpClient.post('/todos', form)  },}  
```  
  
### Mutation  
Next up we are going to create a mutation called `useTodoCreateMutation`.  
  
This mutation will be used to call the `create` function from our service and create a new todo in the backend.  
  
```typescript  
export function useTodoCreateMutation() {  
  const queryClient = useQueryClient()  return useMutation({    mutationKey: 'createTodo',    mutationFn: async (form: TodoForm) => {      await todoService.create(form)    },    onSuccess: async () => {      await queryClient.invalidateQueries('todos')    },  })}  
```  
  
> aside positive  
> If you're not sure how to use `useMutation`, you can take a look at the [Vue Query documentation](https://tanstack.com/query/v4/docs/vue/guides/mutations).  
  
### Modal (smart) component  
Once we have created the mutation, we can start with creating a modal component that will be used to create the todo's.  
  
- Create a `TodoModal.vue` (smart) component in the `src/modules/todos/components` folder.  
- Add a form that allows the user to enter a `title`, `description` and `deadline`.  
- Add a submit button that will call the `useTodoCreateMutation` mutation.  
  
> aside positive  
>Like before, we'll be using [Formango](https://wisemen-digital.github.io/vue-formango/) for our form validation.
  
```vue  
<script setup lang="ts">  
import { useForm } from 'formango' const todoCreateMutation = useTodoCreateMutation()  
  
const { onSubmitForm, form } = useForm({  
  schema: todoFormSchema,  initialState: {    title: '',    description: '',    deadline: '',  },})  
  
const title = form.register('title')  
  
function onSubmit(): void {  
  form.submit()}  
  
onSubmitForm(async (formData: TodoCreateForm) => {  
  try {    await todoCreateMutation.mutateAsync(formData) // notice the async keyword here, it's very important  } catch (error) {    console.error(error)  }})  
</script>  
  
<template>  
<form @submit.prevent="onSubmit">  
    <AppInput v-bind="title" />    <button type="submit">Submit</button></form>  
```   

### View  
To finish up, we are going to update our `TodoOverviewView` by adding a button that will open the `TodoModal` when clicked.  

> aside positive
> Check out libraries like [Radix](https://www.radix-vue.com/) for easy-to use UI components. (Like showing and using a Modal!) 
  
```vue  
<script setup lang="ts">  
...  
const isModalOpen = ref<boolean>(false) ...  
</script>  
  
<template>  
<div>  
    <TodoList :todos="todos" :is-loading="isLoading" />    <button @click="onCreateButtonClick">Create todo</button>    <TodoModal v-if="isModalOpen" @close="handleClose" /></div>  
</template>  
```  
  
💡Don't forget to make a pull request of your work so your buddy can review your code and keep track of your progress. Keeping your PR's small and frequent is a good practice.  
  
## PROJECT: Updating and deleting todo's  
  
The last step is to allow the user to update and delete existing todo's. This will be done by clicking on the edit button of a todo.  
We are going to extend the functionality of the `TodoModal` component to allow the user to update a todo.  
To achieve this, we need to know if the modal is opened in `create` or `update` mode. The easiest way to do this is to  
check if a todo uuid is passed to the modal.  
  
### Service  
Now it's time to add a new function to our existing service that will be used to update a todo.  
  
```typescript  
interface TodoService {  
  update: (uuid: TodoUuid, form: TodoForm) => Promise<void>  deleteByUuid: (uuid: TodoUuid) => Promise<void>}  
  
export const todoService: TodoService = {  
  update: async (uuid: TodoUuid, form: TodoForm): Promise<void> => {    await httpClient.post(`/todos/${uuid}`, form)  },  deleteByUuid: async (uuid: TodoUuid): Promise<void> => {    await httpClient.delete(`/todos/${uuid}`)  },}  
```  
  
> aside negative  
> You will need to provide the `TodoUuid` type for yourself. Zod allows you to create a custom type for this using **brands**.  
> More info can be found here: [https://zod.dev/?id=brand](https://zod.dev/?id=brand)  
  
### Mutation  
Once we have added the `update` and `deleteByUuid` functions to our service, we can start with creating the mutations.  
  
```typescript  
export function useTodoUpdateMutation() {  
  const queryClient = useQueryClient()    return useMutation({  
    mutationKey: 'updateTodo',    mutationFn: async (uuid: TodoUuid, form: TodoForm) => {      await todoService.update(uuid, form)    },    onSuccess: async () => {      await queryClient.invalidateQueries('todos')    },  })}  
```  
  
### Modal (smart) component  
Now it's time to extend the functionality of the `TodoModal` component to allow the user to update a todo.  
  
- Add a `uuid` prop to the `TodoModal` component.  
- Add a `update` function to the `TodoModal` component that will call the `useTodoUpdateMutation` mutation.  
- Add a `delete` function to the `TodoModal` component that will call the `useTodoDeleteMutation` mutation.  
  
```vue  
<script setup lang="ts">  
  
const props = defineProps<{  
  todo: Todo | null}>()  
  
const updateMutation = useTodoUpdateMutation()  
const deleteMutation = useTodoDeleteMutation()  
  
const { onSubmitForm, form } = useForm({  
  schema: todoFormSchema,  initialValues: {    title: props.todo?.title || '',    description: props.todo?.description || '',    deadline: props.todo?.deadline || '',  },})  
  
const title = form.register('title')  
...  
  
function onSubmit(): void {  
  form.submit()}  
  
onSubmitForm(async (formData: TodoForm) => {  
  try {    if (props.todo) {      await updateMutation.mutateAsync(props.todo.uuid, formData)    } else {      await createMutation.mutateAsnyc(formData)    }  } catch (error) {    console.error(error)  }})  
  
function handleDelete(uuid: TodoUuid): void {  
  deleteMutation.mutateAsync(uuid)}  
  
</script>  
  
<template>  
<div>  
    <form @submit.prevent="onSubmit">        <input v-model="title.value" />        ...        <button type="submit">Submit</button>    </form>    <button @click="handleDelete(props.uuid)">Delete</button></div>  
</template>  
```  
  
💡Don't forget to make a pull request of your work so your buddy can review your code and keep track of your progress. Keeping your PR's small and frequent is a good practice.  
  
## Finishing up  
  
Congratulations! You have successfully completed our Vue.js workshop. 🥳🤩  
  
<img width="600" src="img/the-office-dwight.gif">  
  
Make sure that your project has been pushed to your repository and that you have created a pull request.  
Fix any remarks that you have received from your mentor and wait for the final feedback.  
  
Also make sure your styling is consistent with the designs and adjust where necessary.

> aside positive
> If you have any remarks about this onboarding, don't hesitate to tell your buddy all about them!