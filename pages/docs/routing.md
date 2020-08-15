---
created: 1597455375999
---# Routing

textbase.js has a file-system based router built on the concept of pages.

When a file is added to the `pages` directory it's automatically available as a route.

The files inside the `pages` directory can be used to define most common patterns.

## Index routes

The router will automatically route files named index to the root of the directory.

- `pages/index.md → /`
- `pages/docs/index.md → /docs`

## Nested routes

The router supports nested files. If you create a nested folder structure files will be automatically routed in the same way still.

`pages/blog/first-post.md → /blog/first-post`
`pages/blog/section/first-post.md → /blog/section/first-post`

## Linking between pages

```md
[About Page](/about)
```

```html
<a href="/about">About Page</a>
```

You can link between pages and routes using markdown or html. For example, this example creates a link titled [About Page](/about) that leads to `pages/about.md`.

# Route Directory

By default, textbase.js websites will be generated with a `/_routes.html` route that shows a list of all the route on the website. You can view this website's [route directory here](/_pages.html).

<br/> [&larr; Back](/docs)
