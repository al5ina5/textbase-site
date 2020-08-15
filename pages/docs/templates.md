---
title: Templates - textbase.js
created: 1597455376010
---

# Templates

## Templates in textbase.js are really simple.

> **NOTE** You can skip most of this process running `textbase eject` in your project directory. This will spit out textbase's default theme to your project directory, allowing you to dissect it directly. This might be a better option if you know what you're doing.

We tried to make sure theming in textbase.js as easy as possible. We didn't want there to a be a learning curve. We wanted to empower you to use the skills you already know to design your textbase.js webiste—not learn new ones.

Templates in textbase.js are made just like standard html5 websites.

Our templates `index.html` is responsible for the result of every page generated from the `./pages` folder.

```
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Docs</title>

    <link rel="stylesheet" href="./style.css">
</head>

<body>
    {{{html}}}
</body>

</html>
```

Good ol' plain HTML.

You'll notice the `<body>` of the templates `index.html` is nearly empty. During build time, the markdown in your `/pages/*.md` will be plugged into `{{{html}}}` as carefully crafted HTML.

You'll also notice we've linked a stylesheet.

At this point, your template is just 2 files.

```
🗂 templates
📂 ---- yourtemplate
📄 -------- index.html
📄 -------- style.css
```

## Classless Styling

Classless styling is the _new_ hip way to style your pages effectively in the absolutely way possible.

> **NOTE** textbase.js's default is a modified version of the classless css framework [new.css](https://newcss.net/).

Since the markdown you write in your `./pages` will be generated into bare html (no classes by default), we recommend style html's default tags, such as `h1`, `h2`, `p`, `code` and more.

```
h1 {
    font-size: 2.25rem
}

h2 {
    font-size: 1.85rem
}

h3 {
    font-size: 1.55rem
}
```

We suggest starting your textbase.js website with our base css styling, and adding your custom styles as you desire. You can do so by importing `textbase-light` or `textbase-dark` into your `./style.css` file.

```
@import "https://unpkg.com/textbase-light";
@import "https://unpkg.com/textbase-dark";
```

## Importing your template

Once your template is ready to go, you'll need to set it as the active template.

Create a `./_textbase.js` file in you project root. This file should be adjacent to your `./pages` folder.

> **TIP** You can view all the options available in `./_textbase.js` [here](/options.html).

Populate `./pages/index.md` with the following contents:

```
modules.exports = {
    themeFolder: './templates/yourtheme'
}
```

<br/> [&larr; Back](/docs)
