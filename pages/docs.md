# Getting Started

Welcome to the textbase.js documentation!

Rest assure, this'll get you runnin' in no time!

If you have questions about anything related to textbase.js, you're always welcome to ask our community on GitHub Discussions.

### System Requirements

- [NodeJS](http://nodejs.org/)
- MacOS, Windows (including WSL), and Linux are supported

# Setup

Install `textbase` in your project:

```
npm install textbase
```

Optionally, open `package.json` and add the following `scripts`:

```
"scripts": {
  "dev": "textbase dev",
  "build": "textbase"
}
```

These scripts refer to the different stages of developing an application:

- `dev` - Runs `textbase dev` which starts textbase.js in development mode
- `build` - Runs `textbuild` which builds the application for production usage

textbase.js is built around the concept of pages. A page is a `.md` file that contains a simple mix of plain text, markdown, and HTML in the `pages` directory.

Pages are associated with a route based on their file name. For example `pages/about.md` is mapped to `/about.html`.

Create a `pages` directory inside your project.

Populate `./pages/index.md` with the following contents:

```
# Header
# A moving sub-header.
Your `textbase.js` website is alive.
```

To start developing your application run `npm run dev`. This starts the development server on a random url, such as `http://localhost:59321`.

So far, we get:

- Automatic compilation based on your active template.
- Live reload, so you can view your website in real-time.
- Static generation of `./pages/`.
- Static file serving. `./public/` is mapped to `/`

In addition, any textbase.js application is ready for production from the start.

## Up next...

[Templates](/templates) in textbase.js.
