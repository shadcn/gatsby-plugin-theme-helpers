# gatsby-plugin-theme-helpers (Experimental)

An experimental plugin to help with [component shadowing](<(https://www.gatsbyjs.org/docs/themes/shadowing/)>) discovery by annotating React components with the source file and the shadow target.

![gatsby-plugin-theme-helpers](https://i.imgur.com/8V2kGNv.jpg)

## Installation

To test this plugin, install it as a [local plugin](https://www.gatsbyjs.org/docs/loading-plugins-from-your-local-plugins-folder/).

1. Clone this repo to a `plugins` directory in the website’s root directory.

```
site
  ├── content
  ├── plugins
  │   └── gatsby-plugin-theme-helpers <-------
  ├── gatsby-config.js
  └── gatsby-node.js
```

2. Enable the plugin in `gatsby-config.js`

```js
module.exports = {
  siteMetadata: {
    title: `Gatsby`,
  },
  plugins: [`gatsby-plugin-theme-helpers`],
}
```

3. Run `gatsby develop`

## Usage

Inspect your site using Devtools.

The plugin will add `data-source` and `data-shadow` attributes to your components to make it easy to figure out the source of a component and the name of the shadow file to create.

### Starting a new Gatsby site? Check out https://github.com/reflexjs/reflex
