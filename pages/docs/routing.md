# Routing

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

```
[About Page](/about)
```

You can link between pages and routes using markdown or html. For example, this example assumes you would like to link to a page located at `pages/about.md`.

[&larr; Back](/docs)
