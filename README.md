# nuxt-qrq-boilerplate

> Nuxt.js boilerplate with Tailwind, local shared utilities (shared-qrq) and opinionated linting

## Build Setup
* Clone shared-qrq utilities package from [here](https://github.com/alessandrocurcu/shared-qrq) before `npm install`

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
