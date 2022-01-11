# Project Title

A description of what the project is about. Give a brief description of the project. What was the reason or motivation behind the creation of the project?

## Contents

* [Prerequisites](#prerequisites)
* [Dependencies](#dependencies)
  * [axios](#dependencies)
  * [prop-types](#dependencies)
  * [react-native-config](#dependencies)
  * [react-navigation](#dependencies)
  * [react-native-localization](#dependencies)
  * [react-native-mmkv-storage](#dependencies)
  * [redux](#dependencies)
  * [redux-persist](#dependencies)
  * [redux-thunk](#dependencies)
* [Dev Dependencies](#dev-dependencies)
  * [jest](#dev-dependencies)
  * [react-native-testing-library](#dev-dependencies)
* [Folder Structure](#folder-structure)
* [Usage](#usage)
* [Build](#build)
* [Tests](#tests)
* [Style Guide](#style-guide)
* [Contributing Guide](#contributing-guide)

## Prerequisites

What is needed to set up the dev environment. For instance, global dependencies or any other tools. include download links.

* [Node.js > 16](https://nodejs.org) and npm
* [JDK > 17](https://www.oracle.com/java/technologies/javase-jdk11-downloads.html)
* [Android Studio and Android SDK](https://developer.android.com/studio)

## Dependencies

Additional dependencies for this project. Each item should contain the dependency name, purposes and its download link.

* [axios](https://github.com/axios/axios) for networking.
* [prop-types](https://github.com/facebook/prop-types) to type-check our components exposed properties.
* [react-native-config](https://github.com/luggit/react-native-config) to manage environments.
* [react-navigation](https://reactnavigation.org/) navigation library.
* [react-native-localization](https://github.com/stefalda/ReactNativeLocalization) for string localization.
* [react-native-mmkv-storage](https://github.com/ammarahm-ed/react-native-mmkv-storage#readme) as storage solution.
* [redux](https://redux.js.org/) for state management.
* [redux-persist](https://github.com/rt2zz/redux-persist) as persistance layer.
* [redux-thunk](https://github.com/gaearon/redux-thunk) to dispatch asynchronous actions.

## Dev Dependencies

Additional dev dependencies for this project. Each item should contain the dependency name, purposes and its download link.

* [jest](https://facebook.github.io/jest/) for testing.
* [react-native-testing-library](https://callstack.github.io/react-native-testing-library/) for testing.

## Folder structure

Describe the project structure like the following example:

* `actions`: This folder contains all actions that can be dispatched to redux.
* `assets`: Asset folder to store all images, vectors, etc.
* `components`: Folder to store any common component that you use through your app (such as a generic button)
* `constants`: Folder to store any kind of constant that you have.
* `controllers`: Folder to store all your network logic (you should have one controller per resource).
* `localization`: Folder to store the languages files.
* `navigation`: Folder to store the navigators.
* `reducers`: This folder should have all your reducers, and expose the combined result using its `index.js`
* `screens`: Folder that contains all your application screens/features.
  * `Screen`: Each screen should be stored inside its folder and inside it a file for its code and a separate one for the styles and tests.
    * `Screen.js`
    * `Screen.styles.js`
    * `Screen.test.js`
* `selectors`: Folder to store your selectors for each reducer.
* `storage`: Folder that contains the application storage logic.
* `store`: Folder to put all redux middlewares and the store.
* `test-utils`: Folder to store tests-related utilities and components.
* `theme`: Folder to store all the styling concerns related to the application theme.
* `App.js`: Main component that starts your whole app.
* `index.js`: Entry point of your application as per React-Native standards.

## Usage

Give a detail explanation on how your package is used. For REST APIs, a Swagger api documentation link is needed in this section.

```js
import { Sample } from '@react-native-fihtdc-sample';

const App = () => <Sample title="Hello World!" />;
```

## Build

Describe how to build debug/production version step by step. For instance these are the steps to generate `.apk`, `.aab` and `.ipa` files

### Android

1. Generate an upload key
2. Setting up gradle variables
3. Go to the android folder
4. Execute `./gradlew assemble[Env][BuildType]`

Note: You have three options to execute the project
`assemble:` Generates an apk that you can share with others.
`install:` When you want to test a release build on a connected device.
`bundle:` When you are uploading the app to the Play Store.

For more info please go to <https://reactnative.dev/docs/signed-apk-android>

### iOS

1. Go to the Xcode
2. Select the schema
3. Select 'Any iOS device' as target
4. Product -> Archive

For more info please go to <https://reactnative.dev/docs/publishing-to-app-store>

## Tests

Describe how to test this package and components.

```bash
yarn lint && CI=true yarn test --coverage
```

## Style Guide

Describe what is the coding styles for this project. For coding styling, we decided to go with ESLint and [React Native community's style guide](https://github.com/facebook/react-native/tree/master/packages/eslint-config-react-native-community#readme).

## Contributing Guide

Describe how others may contribute to the project.
See the following example.
If you joined this project, please follow the rules below.

### - Workflow

1. New branch (Format: Date_Introduction) and make functions, example below.

    ```bash
    $ git checkout -b 20220111_FixRouteGPS
    <after patch is made>
    $ git push
    ```

2. Go to GitLab page to `new 'Merge Request'`, set the target branch to `dev`.

3. Request reviewing.

4. Reviewer accept(or reject) the Merge Request.

### - Commit messages

```bash
[tag]: [action]
example. "feat: Fix route GPS bug"
```

The tags are listed below.

```bash
- feat: (a new feature)
- fix: (a bug fix)
- docs: (changes to documentation)
- style: (formatting, missing semi colons, etc; no code change)
- refactor: (refactoring production code)
- tests: (adding tests, refactoring tests; no production code change)
- chore: (updating build tasks, package manager configs, etc; no production code change)
- ci: (CICD flows; no production code change)
```

## Maintainers

* LawrenceWu@mobiledrivetech.com
* JohnJYChen@mobiledrivetech.com
* JackCHLin@mobiledrivetech.com
