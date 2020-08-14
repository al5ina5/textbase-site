# Getting Started

Welcome to the textbase.js documentation!

Rest assure, this'll get you runnin' in no time!

If you have questions, comments, or ideas about anything related to textbase.js, you're always welcome to [contact us](/contact).

### System Requirements

- [NodeJS](http://nodejs.org/)
- MacOS, Windows, and Linux are supported

## Setup

Install `textbase` in your project:

```
npm install textbase
```

Optionally, open `package.json` and add the following `scripts`:

```
"scripts": {
	"start": "textbase",
	"build": "textbase build"
}
```

These scripts refer to the different stages of developing an application:

- `start` - Runs `textbase` which starts textbase.js in development mode.
- `build` - Runs `textbase build` which builds the application for production usage.

textbase.js is built around the concept of pages. A page is a `.md` file that contains a simple mix of plain text, markdown, and HTML in the `pages` directory.

Pages are associated with a route based on their file name. For example `pages/about.md` is mapped to `/about`. You can read more about [routing here](/docs/routing).

Create a `pages` directory inside your project.

Populate `./pages/index.md` with the following contents:

```
# Header
# A moving sub-header.
Your `textbase.js` website is alive.
```

To start developing your application run `npm start`. This starts the development server on a random url, such as `http://localhost:59321`. You can set a specific port by setting [custom options](/docs/options).

So far, we get:

- Automatic compilation based on your active template.
- Live reload, so you can view your website in real-time.
- Static generation of `./pages/`.
- Static file serving. `./public/` is mapped to `/`

In addition, any textbase.js application is ready for production from the start.

## Quick Links

- [FAQ](/docs/faq)
- [Routing](/docs/routing)
- [Templates](/docs/templates)
- [Options](/docs/options)
- [Roadmap](/docs/roadmap)
