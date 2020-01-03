# Billing
	Based on VUE and tailwindcss
## Project setup
```
yarn install
```

### Start Electron development server Compiles and hot-reloads for development
```
$ yarn electron:serve
```
### Build Electron app for distribution
```shell
$ yarn electron:build
```
### Regenerate icons from public/icon.png
```shell
$ yarn electron:generate-icon
```
### Lints and fixes files
```
yarn lint
```
### Customize configuration
See [Configuration Reference](https://cli.vuejs.org/config/).


### Vue CLI Plugin Electron Builder
See [Vue CLI Plugin Electron Builder](https://nklayman.github.io/vue-cli-plugin-electron-builder/).

### Tailwindcss Installation
See [Tailwindcss](https://tailwindcss.com/docs/installation/)

### Directory Structure
```shell
.
├── LICENSE
├── README.md
├── babel.config.js
├── dist_electron
│   ├── index.js
│   └── package.json
├── package-lock.json
├── package.json
├── postcss.config.js
├── public
│   ├── favicon.ico
│   ├── img
│   │   ├── beach-work.jpg
│   │   ├── chicago.jpg
│   │   ├── colorado.jpg
│   │   ├── logo-inverted.svg
│   │   ├── logo.svg
│   │   ├── logo2.svg
│   │   ├── malibu.jpg
│   │   ├── miami.jpg
│   │   ├── seattle.jpg
│   │   └── toronto.jpg
│   └── index.html
├── src
│   ├── App.vue
│   ├── assets
│   │   ├── logo.png
│   │   └── tailwind.css
│   ├── background.js
│   ├── components
│   │   ├── AccountDropdown.vue
│   │   ├── DestinationCard.vue
│   │   ├── HelloWorld.vue
│   │   ├── HomePage.vue
│   │   ├── NavBar.vue
│   │   └── PropertyCard.vue
│   ├── main.js
│   └── store
│       └── PropertiesData.js
├── tailwind.conf.js
└── yarn.lock
 ```

 