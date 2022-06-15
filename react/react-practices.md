# React practices for better developer and user experience.

  I believe every front end application we built need few basic things which makes the development experience very much smoother and easier to scale and develop new features in the future. I believe these are the main aspects I feel we should consider in developing a front end application.

- Configuring Project
- Clean code standard
- Structuring Project
- Styles and Components
- API's
- Managing state
- Testing
- Security (wider area will update in next iteration )
- Performance (wider area will update in next iteration )

## 1. Configuring Project
### 1. Typescript
Especiallly when comes to building large projecs we gotta deal with lots of data which can be highly dynamic. Typescript adds a lot od value for type checking and type safety.

### 2. linting and prettier
As we developers we over see a lot of minor silly syntax mistakes etc.. linting can save quit a good time from such mistakes and prettier enhances the developer experience in its own terms.

### 3. Configuring absolute import paths
As the projects goes and when needs to refactor the any fixes etc. removing and updating files can really be messing and configuring absolute import paths saves a lot of time as we develop. 

## 2. Clean Code standard
While working on a large project with multiple contributions from different team members there has to be clean, abstract, unquie standards to be followed by everyone for seamless deugging and futher development. Here are few standards we can consider to follow for naming conventions, abstraction etc.
1.  [clean code javascript](https://github.com/ryanmcdermott/clean-code-javascript)
2.  [style guide by airbnb](https://github.com/airbnb/javascript)

## 3. Structuring Project
this I see as a ideal way to structure a project.

```
src
|
+-- assets            # assets folder can contain all the static files such as images, fonts, etc.
|
+-- components        # shared components used across the entire application
|
+-- config            # all the global configuration, env variables etc. get exported from here and used in the app
|
+-- features          # feature based modules
|
+-- hooks             # shared hooks used across the entire application
|
+-- lib               # re-exporting different libraries preconfigured for the application
|
+-- providers         # all of the application providers
|
+-- routes            # routes configuration
|
+-- stores            # global state stores
|
+-- test              # test utilities and mock server
|
+-- types             # base types used across the application
|
+-- utils             # shared utility functions
```
### 4. Styles and Components
With react advancement its highly recommended to use functional components. And components has to be more abstracted according to the functionality. It adviceable to use one component library and defined rules for styling all through the project which keeps project clean and easy to refactor and develop.
###### Popularly used component libraries: 
1. [MUI](https://mui.com/)
2. [chakra UI](https://chakra-ui.com/)
3. [Headless UI*](https://headlessui.dev/) headless component library for easy customization.
###### styling ways:
1. [tailwind](https://tailwindcss.com/)
2. [styled-components](https://styled-components.com/)
3. [CSS modules](https://github.com/css-modules/css-modules)

#### [Storybook](https://storybook.js.org/) much about it later

### 5. API's
using an api client which has in hand functionalities will always comes handly one as such is  [react-query](https://react-query.tanstack.com/). which facilitates us with developer friendly features for caching requests, less dependency on global state etc. 

### 6. Managing State
State Management is one the beautiful feature which made scaling very feasible in FE applications. In react there are multiple ways to manage state. component level state management. Global state management. Component level state management is achieved using useState hooks provided by react and global state by context and hooks provided by react. other alternatives for achieving these is using Redux which is quite a popular way to manage state.

other type of statemanagement is to manage server data by caching and maintaing that state. As mentioned above [react-query](https://react-query.tanstack.com/) is on among us which makes development much modular and easier.

### 7. Testing
Testing is way to eradicate lot of forseen error that might occur at production. There are multiple types of testing includes Unit testing, E2E. React is highly compatible with existing testing libraries. 
1. [jest](https://jestjs.io/)
2. [cypress](https://www.cypress.io/) is popular for automating e2e



