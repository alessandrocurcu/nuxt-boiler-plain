# nuxt-qrq-boilerplate

> Nuxt.js boilerplate with Tailwind

## Build Setup

```bash
# install dependencies
$ npm install

# serve with hot reload at localhost:3000
$ npm run dev

# build for production and launch server
$ npm run build
$ npm run start

# generate static project
$ npm run generate
```

For detailed explanation on how things work, check out [Nuxt.js docs](https://nuxtjs.org).

# Expose local host to external devices
* Get your IP in the terminal with `ipconfig getifaddr en1`
* In `package.json` update dev script with `HOST=<your ip> nuxt`

# Font Awesome 5 Free
If you want to install Font Awesome from NPM and make it work with Buefy follow these instructions:

1. Install nuxt-fontawesome and some dependencies

```bash
npm i nuxt-fontawesome
npm i @fortawesome/fontawesome-svg-core @fortawesome/vue-fontawesome
```

2. Install an icon set, for example:

```bash
npm i @fortawesome/free-solid-svg-icons
```

3. Edit nuxt.config.js as follows:

```js
modules: [
  'nuxt-buefy',
  'nuxt-fontawesome'
],
buefy: {
  materialDesignIcons: false,
  defaultIconPack: 'fas',
  defaultIconComponent: 'font-awesome-icon'
},
fontawesome: {
  imports: [
    {
      set: '@fortawesome/free-solid-svg-icons',
      icons: ['fas']
    }
  ]
}
```

4. Usage example:
```html
<b-icon pack="fas" icon="home" size="is-large" />
```
