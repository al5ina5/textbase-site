---
title: Options - textbase.js
description: Learn how to generate more complex website. Modifying these settings will alter the output contents of `_site` during the build process.

created: 1597455375997
---
| [home](/) | [getting started](/docs/start) | [contact us](/contact) | 
# texbase. js options

The `_textbase.js` enables you to tweak your generation settings. Modifying these settings will alter the output contents of `_site` during the build process.

## Configuration

Create a `_textbase.js` file in the root of your project. It should be adjacent with your `pages` folder.

```
🗂 textbase-app
📂 ——— pages
📄 ——— _textbase.js
```

Populate your `_textbase.js` file with some settings:

```
module.exports = {
  port: 3000,
  minify: true
}
```

## Available Options

#### `publicFolder`

Alters the location of the `public` folder.

```
./public
```

#### `pagesFolder`

Alters the location of the `pages` folder.

```
./pages
```

#### `siteFolder`

Alters the location of the `_site` folder.

```
./_site
```

#### `templateFolder`

Alters the location of the template folder.

```
.../node_modules/textbase/templates/textbase
```

#### `port`

Alter the port of the production and development server.

```
0
```

> **NOTE** Running on port 0 assigns a random port during runtime on most operating systems.

### `minify`

Enables and disables minification and compression of outputted website.

```
false
```

### `showExtensions`

By default, extensions are hidden in urls. Use this option to convert links such as `/docs` to `/docs.html`.

```
false
```

### `dev`

Enable or disable dev mode. Disable by default, but forced when running `textbase dev`.

```
false
```

<br/> [&larr; Back](/docs)
