# Personal website

My personal website is built using nuxt3.js

## Pre-requisites

1. Install [nvm](https://github.com/nvm-sh/nvm)

> $ curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.39.1/install.sh | bash

Then open a new terminal and type:

> $ nvm install node

## Install

Open a terminal and type:

> npx nuxi init project_dir

Use the documentation from [here][https://tailwindcss.com/docs/guides/nuxtjs] to:

> $ npm install -D tailwindcss postcss@latest autoprefixer@latest @nuxt/postcss8
> $ npx tailwindcss init

Modify nuxt.config.js to include the following setup:

```js
export default {
  buildModules: [
    '@nuxt/postcss8',
    // ...
  ],
   build: {
    postcss: {
      plugins: {
        tailwindcss: {},
        autoprefixer: {},
      },
    },
  }
}
```

Install content

> $ npm install --save-dev @nuxt/content

