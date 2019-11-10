<p align="center">
    <img src="https://camo.githubusercontent.com/5b54cc5a749519515e15846ac911b094fa762ee5/687474703a2f2f7365616e776174746572732e696f2f696d616765732f616d6265722d7675652e706e67" alt="amber-vue" data-canonical-src="http://seanwatters.io/images/amber-vue.png" height="200">
</p>

<p align="center">
    <a href="https://opensource.org/licenses/MIT"><img src="https://img.shields.io/badge/Version-0.1.0-green.svg" ></a>
    <a href="https://amberframework.org/"><img src="https://img.shields.io/badge/using-amber_framework-orange.svg" ></a>
    <a href="https://opensource.org/licenses/MIT"><img src="https://img.shields.io/badge/License-MIT-brightgreen.svg" ></a>
</p>

<p align="center">
    <i>The Speed and Performance of Amber with the ease of development in Vue</i>
</p>

<br>

# Amber with Vue.js

The goal of the **Amber with Vue.js** recipe is to quickly provide a full stack solution that takes full advantages of the best parts of development using a frontend framework (in the way it was designed to be used), with a powerful backend API.

The intention is to break away from the traditional Rails-y MVC model, without requiring developers to write completely separate frontend/backend codebases.

<br>

## Creating a Project

To create your project with the **Amber with Vue.js** recipe, you will need to run the following command:

```
amber new <your app name> -r progressive-amber/vue-recipe
```

You may also want to specify your database (default is Postgres) by adding the `-d` tag:

```
amber new <your app name> -r progressive-amber/vue-recipe -d <pg | mysql | sqlite>
```

Once your app has been created, you will want to run

```
cd <your app name>
amber w
```

Your application will be running on `localhost:9090`.

<br>

## File Structure

With this recipe, we have modularized the file structure to isolate your frontend code in Vue.js from your Amber API.

```
|- bin
|- config
|- db
|- frontend-vue   // Vue.js file tree structure.
    |- src
        |- assets
        |- components
            |- HelloWorld.vue
        |- App.vue
    |- main.js

|- lib
|- public
|- spec
|- src
    |- controllers
        |- application_controller.cr    // Render method for root is in application_controller.cr

    |- locales
    |- models
    |- views
        |- layouts
        |- application
            |- application.slang   // Location of the root #app <div> Vue will render to.

```

<br>

## CLI

The **amber-vue-cli** is a tool for scaffolding APIs, and components. To use the CLI, you will need to install the tool with `npm install`. You will then need to run:

```
npm run vue-tools
```

When you run the CLI, you should see the following:

```
? select generator
> componenet  // vue component generator
> scaffold  // **currently doesn't have full functionality**
> api  // will generate a full CRUD API in amber
```

Please feel free to also reference the **amber-vue-cli** [docs](https://www.npmjs.com/package/@progressive-amber/amber-vue-cli)!

<br>

## Documentation

For any questions specific to the [Vue.js](https://vuejs.org/) or [Amber](https://amberframework.org/) frameworks, please feel free to refer to their excellent documentation below:

* [Vue.js](https://vuejs.org/v2/guide/)
* [Amber](https://docs.amberframework.org/amber/)

<br>
<br>

## DevTools

When developing Vue.js applications, it is highly recommended to use the [Vue.js devtools](https://github.com/vuejs/vue-devtools). Currently only FireFox and Chrome have support for the devtools extension. Their links are provided below:

* FireFox: [devtools](https://addons.mozilla.org/en-US/firefox/addon/vue-js-devtools/)
* Chrome: [devtools](https://chrome.google.com/webstore/detail/vuejs-devtools/nhdogjmejiglipccpnnnanhbledajbpd?hl=en)

You can also use the standalone Electron app **vue-remote-devtools** for any enviornment:

* Remote: [devtools](https://github.com/vuejs/vue-devtools/blob/master/shells/electron/README.md)

<br>

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details
