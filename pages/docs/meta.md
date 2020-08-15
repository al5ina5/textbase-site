---
title: Page Meta & Variables - textbase.js
created: 1597455375996
---

# Page Meta & Variables

Sometimes you'll need to uniqueify parts of the template, such as the `<title>` of each of your pages. textbase.js using a familiar YAML syntax to that get that.

```
---
title: About Us
---
```

## Plug Variables into Your Template

Your templates `index.html` will automatically inject your page options into matching `{{page.key}}` handlebars. To set the documents `<title>` based on the title option above, you'd simply:

```
<title>{{page.title}}</title>
```

<br />[&larr; Back](/docs)
