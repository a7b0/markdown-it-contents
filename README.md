# markdown-it-contents

> markdown-it plugin for generation a table of contents

## Installation

```
npm install markdown-it-contents
```

## Usage

```
{!toc}
```

The macros `{!toc}` will generate the table of contents for below headings only.

Example of load the plugin:

```js
var markdown = require('markdown-it')();

markdown.use(require('markdown-it-contents'), {
    ..options
});
```

### Options

```js
var defaults = {
    // the max heading level in table of contents
    depth: 6,
    // a custom slugification function
    slugify: function(name) { /* code */},
    // a class for the container
    className: 'table-of-contents'
}
```