---
title: Getting Started with MDX
---

The fastest way to get started with Gatsby + MDX is to use the [MDX
starter](https://github.com/ChristopherBiscardi/gatsby-starter-mdx-basic). This
allows you to write .mdx files in `src/pages` in order to create new pages on
your site.

## 🚀 Quick start

1. **Initialize the MDX starter** with the Gatsby CLI

   ```sh
   npx gatsby new my-mdx-starter https://github.com/ChristopherBiscardi/gatsby-starter-mdx-basic
   ```

1. **Run the dev server** by changing directory to the scaffolded site and install dependencies

   ```sh
   cd my-mdx-starter/
   gatsby develop
   ```

1. **Open the site** running at http://localhost:8000

1. **Update the MDX content** by opening the `my-mdx-starter` directory
   in your code editor of choice and edit `src/pages/index.mdx`.
   Save your changes and the browser will update in real time!

## Add MDX to an existing Gatsby site

If you already have a Gatsby site that you'd like to add MDX to, you
can follow these steps for configuring the [gatsby-mdx](/packages/gatsby-mdx/) plugin:

1. **Add `gatsby-mdx`** and MDX as dependencies

   ```sh
   yarn add gatsby-plugin-mdx @mdx-js/mdx @mdx-js/react
   ```

   > **Note:** If you're upgrading from v0, additionally [check out the MDX migration guide](https://mdxjs.com/migrating/v1).

1. **Update your `gatsby-config.js`** to use `gatsby-plugin-mdx`

   ```javascript:title=gatsby-config.js
   module.exports = {
     plugins: [
       // ....
       `gatsby-plugin-mdx`,
     ],
   }
   ```

1. **Restart `gatsby develop`** and add an `.mdx` page to `src/pages

> **Note:** If you want to query for frontmatter, exports, or other fields like
> `tableOfContents` and you haven't previously added a `gatsby-source-filesystem`
> pointing at `src/pages` in your project, you'll want to add one now.

## What's next?

Go check out the [writing MDX guide](/docs/mdx/writing-pages) to find out what else you can do
with Gatsby and MDX.
