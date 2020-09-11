---
title: Page Meta & Variables - textbase.js
description: Sometimes you'll need to uniqueify parts of the template, such as the <title> of each of your pages. textbase.js using a familiar YAML syntax to that get done, enabling you to add variables to your pages.
created: 1597455375996
---

# Page Meta & Variables

Sometimes you'll need to uniqueify parts of the template, such as the `<title>` of each of your pages. textbase.js using a familiar YAML syntax to that get done, enabling you to add variables to your pages.

```
---
title: About Us
favanimal: Cats
---
```

## Plug Variables into Your Template

Your templates `index.html` will automatically inject your page options into matching `{{page.key}}` handlebars. To set the documents `<title>` based on the title option above, you'd simply:

```
<title>{{page.title} {{page.favanimal}}}</title>
```

<br />[&larr; Back](/docs)
